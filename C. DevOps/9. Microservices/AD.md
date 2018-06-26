Tổng quan
============================================

# I. Active Directory là gì ?
   
   - Active Directory (AD) là một kiến trúc độc quyền của Microsoft. Đây là một kiến trúc không thể thiếu được trên Windows Server, được hiểu nôm na là một dịch vụ thư mục. 
   
   - Active Directory là một hệ thống được chuẩn hóa với khả năng quản trị tập trung hoàn hảo về người dùng cũng như các nguồn tài nguyên trong một hệ thống mạng. 
   
   - Active Directory được sử dụng trong mô hình mạng “Server - Client”.

   - Active Directory dùng để lưu trữ dữ liệu của domain như các đối tượng user, computer, group cung cấp những dịch vụ (directory services) tìm kiếm, kiểm soát truy cập, ủy quyền, 
   
   - Active Directory có dịch vụ chứng thực được xây dựng dựa trên giao thức Keberos hỗ trợ cơ chế single sign-on, cho phép các user chỉ cần chứng thực một lần duy nhất khi đăng nhập vào domain 
   và có thể truy cập tất cả những tài nguyên và dịch vụ chia sẻ của hệ thống với những quyền hạn hợp lệ

   - Active Directory đã làm giảm nhẹ công việc quản lý và nâng cao hiệu quả hoạt động, những công việc mà hầu như không thể thực hiện được trên một hệ thống mạng ngang hàng, 
   phân tán thì giờ đây chúng ta có thể tiến hành một cách dễ dàng thông qua mô hình quản lý tập trung như đưa ra các chính sách chung cho toàn bộ hệ thống nhưng đồng thời 
   có thể ủy quyền quản trị để phân chia khả năng quản lý trong một môi trường rộng lớn.


# II. Những tính năng của Active Directory

   - `Centralized Data Store` - Lưu trữ dữ liệu tập trung: 
      
       + Toàn bộ dữ liệu, thông tin trong hệ thống được lưu trữ một cách tập trung, cho phép người dùng có thể truy cập dữ liệu từ bất cứ nơi đâu, bất cứ lúc nào 
       
       + Nâng cao hiệu năng quản trị của hệ thống, giảm thiếu độ rủi ro cho tài nguyên.

   - `Scalability` - Khả năng linh hoạt với nhu cầu: 
      
        + Active Directory cung ứng một cách linh hoạt các giải pháp quản trị khác nhau cho từng nhu cầu cụ thế trên nền tảng hạ tầng xác định của các doanh nghiệp.
        
   - `Extensibility`:
        
        + Cơ sở dữ liệu của Active Directory cho phép nhà quản trị có thể customize và phát triển
        
        + Ta còn có thể phát triển các ứng dụng sử dụng cơ sở dữ liệu này, giúp tận dụng hết khả năng, hiệu năng của Active Directory.
        
   - `Manageability` - Khả năng quản trị linh hoạt dễ dàng: 
   
        + Active Directory được tổ chức theo cơ chế của Directory Service dưới mô hình tổ chức Directory giúp các nhà quản trị có cái nhìn tổng quan nhất đối với cả hệ thống 
        
        + Giúp user có thể dễ dàng truy xuất và sử dụng tài nguyên hệ thống.   
        
   - `Integration` with `Domain Name System` (DNS): 
        
        + DNS là một partner rất cần thiết đối với Active Directory, trong một hệ thống mạng, các dịch vụ của Active Directory chỉ hoạt động được khi dịch vụ DNS được cài đặt. 
        
        + DNS có trách nhiệm dẫn đường, phân giải các Active Directory Domain Controller trong hệ thống mạng, và càng quan trọng hơn trong môi trường Multi Domain. 
         
        + DNS được dễ dàng tích hợp vào Active Directory để nâng cao độ bảo mật và khả năng đồng bộ hóa giữa các Domain Controller với nhau trong môi trường nhiều Domain.     
   
   - `Client Configuration Management`: 
   
        + Active Directory cung cấp cho chúng ta một khả năng quản trị các cấu hình phía client, giúp quản trị hệ thống dễ dàng hơn và nâng cao khả năng di động của user.
        
   - `Policy - based administration`: 
        
        + Trong Active Directory, việc quản trị hệ thống mạng được đảm bảo một cách chắn chắc thông qua các chính sách quản trị tài nguyên, các quyền truy xuất trên các site, domain và các organization unit. 
        
        + Đây là một trong những tính năng quan trọng nhất được tích hợp vào Active Directory.
        
   - `Replication of information`: 
   
        + Active Directory cung cấp khả năng đồng bộ dữ liệu thông tin giữa các domain, trên nền tảng, môi trường nhiều domain nhằm mục đích giảm thiếu đến mức tối đa rủi ro và nâng cao khả năng họat động của hệ thống mạng.
        
   - `Flexible, secure authentication and authorization`: 
   
        + Active Directory cung cấp nhiều cơ chế authentication như Kerberos, Secure Socket Layer và Transport Layer Security giúp cho việc bảo mật thông tin của user khi xác thực thông tin truy xuất tài nguyên.
        
   - `Security integration`: 
   
        + Active Directory được tích hợp mặc định trong các phiên bản `Windows Server`, do đó Active Directory làm việc rất dễ dàng và linh hoạt, truy xuất điều khiển trên hệ thống được định nghĩa trên từng đối tượng, từng thuộc tính của đối tượng. 
        
        + Các chính sách bảo mật được áp dụng không phải đơn thuần trên local mà còn được áp dụng trên các site, `domain` hay `OU` xác định.
        
   - `Directory - enable applications and infrastructure`: 
   
        + Active Directory là một môi trường tuyệt hảo cho các nhà quản trị thiết lập các cấu hình và quản trị các ứng dụng trên hệ thống. 
        
        + Active Directory cung cấp một hướng mở cho các nhà phát triển ứng dụng (developer) xây dựng các ứng dụng trên nền tảng Active Directory thông qua Active Directory Service Interfaces.
        
   - `Interoperability with other directory services`: 
   
        + Active Directory được xây dựng trên giao thức directory service chuẩn gồm 2 giao thức là Lightweight Directory Access Protocol (LDAP) và Name Service Provider Interface (NSPI), 
        do đó Active Directory có khả năng tương thích với các dịch vụ khác được xây dựng trên nền tảng directory service thông qua các giao thức này. 
        Vì LDAP là một giao thức directoy chuẩn, do đó ta có thể phát triển, tích hợp các sản phẩm ứng dụng trao đổi, chia sẻ thông tin với Active Directory thông qua giao thức LDAP. 
        Còn giao thức NSPI được hỗ trợ bởi Active Directory nằm mục đích đảm bảo và nâng cao khả năng tương thích với directoy của Exchange.
   
   - `Signed and encrypted LDAP traffic`: 
   
        + Mặc định là công cụ Active Directoy trong windows server sẽ tự động xác thực và mã hóa thông tin, dữ liệu truyền tải trên giao thức LDAP. 
        
        + Việc xác thực giao thức nhằm đảm bảo thông tin được gửi đến từ 1 nguồn chính thức và không bị giả mạo.
   
   
KIến trúc của Active Directory
============================================
 