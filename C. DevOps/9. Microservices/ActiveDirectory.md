Active Directory 
==================================

# Mục lục

  - Active Directory là gì ?

  - Azure Active Directory là gì ?

  - Tại sao cần thực thi Active Directory?

  - Những đơn vị cơ bản của Active Directory?

  - Infrastructure Master và Global Catalog

  - Active Directory và LDAP

  - Sự quản lý Group Policy và Active Directory

  
# I. Active Directory là gì

  - AD là 1 dạng cơ sở dữ liệu với mục đích rõ ràng và riêng biệt (không thể thay thế cho `Registry`). Các phần dữ liệu trong Active Directory đều có tính kế thừa, nhân rộng, cấp bậc... rõ ràng và linh hoạt.

# II. Azure Active Directory là gì ?

  - 


## III. Tại sao cần thực thi Active Directory?

  - AD tự động quản lí sự truyền thông giữa các domain controller để bảo đảm mạng được duy trì

  - Người dùng có thể truy cập vào tất cả tài nguyên trên mạng thông qua cơ chế đăng nhập một lần

  - Tất cả các tài nguyên trong mạng được bảo vệ bởi một cơ chế bảo mật khá mạnh, cơ chế bảo mật này có thể kiểm tra nhận dạng người dùng và quyền hạn của mỗi truy cập đối với tài nguyên.

# IV. Những đơn vị cơ bản của Active Directory?

  - Các mạng Active Directory được tổ chức bằng cách sử dụng 4 kiểu đơn vị hay cấu trúc mục. Bốn đơn vị này được chia thành: forest, domain, organizational unit và site.

    > ![rexray-storage-provider.png](imgaes/donvicuaAD.JPG)

    + `Forests`: Nhóm các đối tượng, các thuộc tính và cú pháp thuộc tính trong `Active Directory`.
    
    + `Domain`: Nhóm các máy tính chia sẻ một tập chính sách chung, tên và một cơ sở dữ liệu của các thành viên của chúng.
    
    + `Organizational unit (OU)`: Nhóm các mục trong miền nào đó. Chúng tạo nên một kiến trúc thứ bậc cho miền và tạo cấu trúc công ty của Active Directory theo các điều kiện tổ chức và địa lý.
    
    + `Sites`: Nhóm vật lý những thành phần độc lập của miền và cấu trúc OU. Các Site phân biệt giữa các location được kết nối bởi các kết nối tốc độ cao và các kết nối tốc độ thấp, và được định nghĩa bởi một hoặc nhiều `IP subnet`.

  - Các `Forest`:
      +  Không bị hạn chế `theo địa lý hoặc topo mạng`. Một `forest` có thể gồm nhiều miền, mỗi miền lại chia sẻ một lược đồ chung. 
      
      + Các thành viên miền của cùng một forest thậm chí không cần có kết nối `LAN` hoặc `WAN` giữa chúng. Mỗi một mạng riêng cũng có thể là một gia đình của nhiều forest độc lập. 
      
      + Cột forest nên được sử dụng cho mỗi một thực thể. Mặc dù vậy, vẫn cần đến các forest bổ sung cho việc thực hiện test và nghiên cứu các mục đích bên ngoài forest tham gia sản xuất.

  - Các `miền - Domain`:
  
      + Phục vụ như các mục trong chính sách bảo mật và các nhiệm vụ quản trị.

      + Tất cả các đối tượng bên trong một miền đều là chủ đề cho` Group Policies` miền rộng

      + Bất cứ quản trị viên miền nào cũng có thể quản lý tất cả các đối tượng bên trong một miền

      + Mỗi miền cũng đều có cơ sở dữ liệu các tài khoản duy nhất của nó

      + Chính vì vậy tính xác thực là một trong những vấn đề cơ bản của miền

      + Khi một tài khoản người dùng hoàn toàn xác thực đối với một miền nào đó thì tài khoản người dùng này có thể truy cập vào các tài nguyên bên trong miền.
    
  - `Active Directory` yêu cầu một hoặc nhiều domain để hoạt động.
  
  - Một miền `Active Directory` là một bộ các máy tính chia sẻ chung một tập các chính sách, tên và cơ sở dữ liệu các thành viên của chúng. 
  
  - Một miền phải có một hoặc nhiều máy `domain controller (DC)` và lưu cơ sở dữ liệu, duy trì các chính sách và cung cấp sự thẩm định cho các đăng nhập vào miền.
 
   - `Organizational units`:
      +  tỏ ra linh hoạt hơn và cho phép quản lý dễ dàng hơn so với các miền. OU cho phép bạn có được khả năng linh hoạt gần như vô hạn, bạn có thể chuyển, xóa và tạo các OU mới nếu cần. Mặc dù các miền cũng có tính chất mềm dẻo. 
     
      + Chúng có thể bị xòa tạo mới, tuy nhiên quá trình này dễ dẫn đến phá vỡ môi trường so với các OU và cũng nên tránh nếu có thể.

# V. Infrastructure Master và Global Catalog
  
   - Một thành phần chính khác bên trong `Active Directory` là `Infrastructure Master`. `Infrastructure Master (IM)` là một `domain-wide FSMO (Flexible Single Master of Operations)` có vai trò đáp trả trong quá trình tự động để sửa lỗi (`phantom`) bên trong `cơ sở dữ liệu Active Directory`.

   - Phantom được tạo ra trên các DC, nó yêu cầu một sự tham chiếu chéo cơ sở dữ liệu giữa một đối tượng bên trong cơ sở dữ liệu riêng và một đối tượng từ miền bên trong forest. 
  
   - Ví dụ có thể bắt gặp khi bạn bổ sung thêm một người dùng nào đó từ một miền vào một nhóm bên trong miền khác có cùng forest. Phantom sẽ bị mất hiệu lực khi chúng không chứa dữ liệu mới cập nhật, điều này xuất hiện vì những thay đổi được thực hiện cho đối tượng bên ngoài mà Phantom thể hiện, ví dụ  như khi đối tượng mục tiêu được đặt lại tên, chuyển đi đâu đó giữa các miền, hay vị xóa. 
  
   - `Infrastructure Master` có khả năng định vị và khắc phục một số `phantom`. Bất cứ thay đổi nào xảy ra do quá trình sửa lỗi đều được tạo bản sao đến tất cả các DC còn lại bên trong miền.

   - Infrastructure Master đôi khi bị lẫn lộn với `Global Catalog (GC)`, đây là thành phần duy trì một copy chỉ cho phép đọc đối với các domain nằm trong một forest, được sử dụng cho lưu trữ nhóm phổ dụng và quá trình đăng nhập,… 
   
   - Do GC lưu bản copy không hoàn chỉnh của tất cả các đối tượng bên trong forest nên chúng có thể tạo các tham chiếu chéo giữa miền không có nhu cầu phantom.

# VI. Active Directory và LDAP:

   - `LDAP (Lightweight Directory Access Protocol)` là một phần của `Active Directory`, nó là một giao thức phần mềm cho phép định vị các tổ chức, cá nhân hoặc các tài nguyên khác như file và thiết bị trong mạng, dù mạng của bạn là mạng Internet công cộng hay mạng nội bộ trong công ty.

   - Trong một mạng, một thư mục sẽ cho bạn biết được nơi cất trữ dữ liệu gì đó. Trong các mạng `TCP/IP (gồm có cả Internet)`, `domain name system (DNS)` là một hệ thống thư mục được sử dụng gắn liền tên miền với một địa chỉ mạng cụ thể (`vị trí duy nhất trong mạng`). Mặc dù vậy, bạn có thể không biết tên miền nhưng LDAP cho phép bạn tìm kiếm những cụ thể mà không cần biết chúng được định vị ở đâu.

   - Thư mục LDAP được tổ chức theo một kiến trúc cây đơn giản gồm có các mức dưới đây:

      + `Thư mục gốc` có các nhánh con
      + `Country`, mỗi Country lại có các nhánh con
      + `Organizations`, mỗi Organization lại có các nhánh con
      + `Organizational units` (các đơn vị, phòng ban,…), OU có các nhánh
      + `Individuals` (cá thể, gồm có người, file và tài nguyên chia sẻ, chẳng hạn như printer)

   - Một thư mục LDAP có thể được phân phối giữa nhiều máy chủ. Mỗi máy chủ có thể có một phiên bản sao của thư mục tổng thể và được đồng bộ theo chu kỳ.

   - Các quản trị viên cần phải hiểu LDAP khi tìm kiếm các thông tin trong Active Directory, cần tạo các truy vấn LDAP hữu dụng khi tìm kiếm các thông tin được lưu trong cơ sở dữ liệu Active Directory.

# VII. Sự quản lý Group Policy và Active Directory
  
   - Khi nói đến `Active Directory` chắc chắn chúng ta phải đề cập đến `Group Policy`. Các quản trị viên có thể sử dụng `Group Policy` trong Active Directory để định nghĩa các thiết lập người dùng và máy tính trong toàn mạng. 
   
   - Thiết lập này được cấu hình và được lưu trong `Group Policy Objects (GPOs)`, các thành phần này sau đó sẽ được kết hợp với các đối tượng Active Directory, gồm có các domain và site. 
   
   - Đây chính là cơ chế chủ yếu cho việc áp dụng các thay đổi cho máy tính và người dùng trong môi trường Windows.
 
   - Thông qua quản lý Group Policy, các quản trị viên có thể cấu hình toàn cục các thiết lập desktop trên các máy tính người dùng, hạn chế hoặc cho phép truy cập đối với các file hoặc thư mục nào đó bên trong mạng.

   - Thêm vào đó chúng ta cũng cầm phải hiểu GPO được sử dụng như thế nào. `Group Policy Object` được áp dụng theo thứ tự sau: Các chính sách máy nội bộ được sử dụng trước, sau đó là các chính sách site, chính sách miền, chính sách được sử dụng cho các `OU` riêng. 
   
   - Ở một thời điểm nào đó, một đối tượng người dùng hoặc máy tính chỉ có thể thuộc về một site hoặc một miền, vì vậy chúng sẽ chỉ nhận các GPO liên kết với site hoặc miền đó.

   - Các GPO được phân chia thành hai phần riêng biệt: `Group Policy Template (GPT)` và `Group Policy Container (GPC)`. `Group Policy Template` có trách nhiệm lưu các thiết lập được tạo bên trong GPO. Nó lưu các thiết lập trong một cấu trúc thư mục và các file lớn. Để áp dụng các thiết lập này thành công đối với tất cả các đối tượng người dùng và máy tính, GPT phải được tạo bản sao cho tất cả các DC bên trong miền.

   - `Group Policy Container` là một phần của GPO và được lưu trong Active Directory trên các DC trong miền. GPC có trách nhiệm giữ tham chiếu cho `Client Side Extensions (CSEs)`, đường dẫn đến GPT, đường dẫn đến các gói cài đặt và những khía cạnh tham chiếu khác của GPO. GPC không chứa nhiều thông tin có liên quan đến GPO tương ứng với nó, tuy nhiên nó là một thành phần cần thiết của `Group Policy`. Khi các chính sách cài đặt phần mềm được cấu hình, GPC sẽ giúp giữ các liên kết bên trong GPO. Bên cạnh đó nó cũng giữ các liên kết quan hệ khác và các đường dẫn được lưu trong các thuộc tính đối tượng. Biết được cấu trúc của GPC và cách truy cập các thông tin ẩn được lưu trong các thuộc tính sẽ rất cần thiết khi bạn cần kiểm tra một vấn đề nào đó có liên quan đến GP.