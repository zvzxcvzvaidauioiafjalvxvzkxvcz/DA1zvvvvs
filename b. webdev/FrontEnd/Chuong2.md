Chương 2: CSS
====================

# Mục lục

  - 1. CSS là gì

  - 2. Tác dụng của CSS

  - 3. Quá trình phát triển

  - 4. Các framework của css và ví dụ

    - 4.1. Boostrap

    - 4.2. Foundation

    - 4.3. Bulma

    - 4.4. Ulkit

    - 4.5. Semantic UI

    - 4.6. Materialize css 

  - 5. Responsive

  - 6. Kế nhiệm

    - SASS

    - LESS

    - SCSS

    - Stylus

    - PostCSS
  
  - 7. Phương pháp, mô hình

    + SuitCSS

    + OOCSS

    + Bem

    + SMaCSS

    + Systematic CSS

  - 8. CSS 3

    + Flexbox

    + Gradients

    + Grids

    + Rotate

    + Transform

    + Skew

    + Scale

    + Transition


# 1: CSS là gì ?

  - CSS là chữ viết tắt của Cascading Style Sheets, nó là một ngôn ngữ được sử dụng để tìm và định dạng lại các phần tử được tạo ra bởi các ngôn ngữ đánh dấu (ví dụ như HTML). 
  
  - Phương thức hoạt động của CSS là nó sẽ tìm dựa vào các vùng chọn, vùng chọn có thể là tên một thẻ HTML, tên một ID, class hay nhiều kiểu khác. Sau đó là nó sẽ áp dụng các thuộc tính cần thay đổi lên vùng chọn đó.

# 2. Tác dụng của CSS ?
  
  - Bạn có thể hiểu đơn giản rằng, nếu HTML đóng vai trò định dạng các phần tử trên website như việc tạo ra các đoạn văn bản, các tiêu đề, bảng,…thì CSS sẽ giúp chúng ta có thể thêm một chút “phong cách” vào các phần tử HTML đó như đổi màu sắc trang, đổi màu chữ, thay đổi cấu trúc,…rất nhiều.

# 3. Quá trình phát triển của CSS
  
  - Css liên tục cập nhật gồm nhiều phiên bản. Mỗi phiên bản là 1 framework.

  - Các phiên bản của CSS bao gồm: 

    + CSS 1:  
      
      - Được xuất bản vào ngày 17 tháng 12 năm 1996

      - Các tính năng:

        + Kiểu chữ như in đậm, phong chữ

        + Màu chữ, hình nền

        + Các thuộc tính văn bản như khoảng cách giữa các từ, chữ cái và dòng văn bản

        + Căn chỉnh văn bản, hình ảnh, bảng và các yếu tố khác

        + Lề, đường viền, phần đệm và vị trí cho hầu hết các phần tử

        + Nhận dạng duy nhất và phân loại chung các nhóm thuộc tính

    + CSS 2:

      - Đặc tả CSS 2 được phát triển bởi W3C và được công bố như là một khuyến nghị vào tháng 5 năm 1998. 
      
      - Một phần lớn CSS 1, CSS 2 bao gồm một số khả năng mới như định vị tuyệt đối, tương đối và cố định của các phần tử và  z-index. 
      
      - Các loại phương tiện truyền thông, hỗ trợ cho các bảng định kiểu âm thanh (sau này được thay thế bằng mô-đun giọng nói CSS 3) và văn bản hai chiều và các thuộc tính phông chữ mới.

    + CSS 3:

      - Vậy CSS3 là một chuẩn mới nhất của CSS, hay nói cách khác nó là một Version mới của CSS. Nó được chia ra làm nhiều module và mỗi module sẽ có những nhiệm vụ khác nhau, khi 
      kết hợp chúng với nhau sẽ tạo nên những hiệu ứng tuyệt vời.

      - Với CSS3 nếu bạn kết hợp với jQuery nữa thì website của bạn sẽ trở nên sinh động, điển hình là các hiệu ứng Paralax, Landing Page, ...
      

# 4. Các framework của CSS

  - 4.1. Bootstrap: 
    
    + a. Khái quát:
    
        + Đây là 1 framework hỗ trợ thiết kế giao diện rất tốt. 
        
        + Phiên bản hiện tại là bootstrap 4.
        
        + Bootstrap được sinh ra tại Twitter hồi đầu có tên là Twitter Bootstrap hiện nay là FrameWork số 01, dễ dùng phổ biến và đầy đủ
        
        + Đây là FrameWork bạn nên chọn vì được khá nhiều đơn đặt hàng từ các trang FreeLancer trên thế giới.
        
        + Giao diện sẽ được xây dựng dể dàng nhờ vào bootstrap
        
    + b. Các vấn đề cần chú ý về bootstrap:
        
        + Tính năng Responsive: Mặc đinh, Bootstrap sẽ tự động thay đổi các trang của bạn cho phù hợp với các kích thước màn hình khác nhau. Tuy nhiên
        bạn có thể vô hiệu hóa nó
        
        + Hỗ trợ nhiều trình duyệt và thiết bị: 
            
            - Bootstrap được xây dựng để hoạt động ổn định nhất với các trình duyệt mới nhất trên máy tính để bàn và các thiết bị di động, điều đó có nghĩa 
            là các trình duyệt cũ có thể hiển thị các style khác đi mặc dù vẫn có đầy đủ chức năng khi các thành phần được tạo ra.
        
        + Hỗ trợ bên thứ ba:
        
            - Mặc dù chúng tôi không hỗ trợ bất kỳ plugin hoặc add-on nào của bên thứ 3 một cách chính thức, chúng tôi vẫn có một vài lời khuyên 
            hỗ trợ bạn tránh khỏi các lỗi tiềm tàng trong các dự án của bạn.
            
        + Vấn đề truy nhập:
            
            - Bootstrap được xây dựng tuân theo các chuẩn Web nói chung và—với một ít nỗ lực—có thể được sử dụng để tạo ra các site mà có thể truy cập được bằng cách sử dụng AT.
            
    + c. Cài đặt bootstrap:
    
        + CDN: Các bạn có thể dùng google CDN để chèn boostrap vào dự án của mình
        
        + Tải thư viện tại getbootstrap.com
        
    + d. Các component và các tính năng về JS: Xem tại getbootstrap.com
    
  - 4.2. Foundation
  
    - a. Foundation là gì ?
    
       + Foundation (theo như quảng cáo trên trang của họ) là một front-end framework đầu tiên và tiên tiến nhất thế giới, giúp chúng ta dễ dàng xây dựng các bản prototype, 
       các sites và các ứng dụng (apps) hoạt động trên hầu hết các thiết bị (từ các màn hình loại nhỏ như smartphone tới các màn hình cỡ trung và lớn như PC và TV) với bộ 
       thư viện mà họ cung cấp.
    
       + Foundation hướng tới kiến trúc mobile-first, tức là ban đầu bạn sẽ phải thiết kế ứng dụng cho các thiết bị có màn hình nhỏ đầu tiên, sau đó mở rộng ra những loại 
       kích cỡ màn hình lớn hơn. Tuy nhiên bạn cũng không bắt buộc phải đi theo kiến trúc đó, chỉ là họ khuyên nên làm theo kiến trúc này sẽ đạt được hiệu quả tốt về thiết kế.
    
    - b. Front-end framework là gì?
    
       + Tương tự như các frameworks dùng để xây dựng giao diện ứng dụng native (kiểu Xcode cho iOS), Foundation là một framework để xây dựng giao diện front-end, 
       giao diện người dùng của website hoặc các ứng dụng web. Foundation hoạt động trên browser, bởi vậy chúng ta có thể chủ động thiết kế các View riêng lẻ mà không 
       cần quan tâm đến vấn đề logic, hay Server xử lý ra sao.
    
    - c. Các kỹ thuật sử dụng trong Foundation:
    
       + Foundation được xây dựng và đóng gói với bộ HTML, CSS và Javascript, cung cấp cho người dùng các thành phần cơ bản nhất của ứng dụng Web.
       Ngoài ra các kỹ thuật như jQuery, HTML5 Boilerplate và Normalizr cũng được sử dụng để hỗ trợ thêm sức mạnh cho Foundation.
         
       + Kết hợp lại chúng ta sẽ có một bộ thư viện gồm các thành phần (components) và các plugins giúp làm việc dễ dàng hơn với các loại trình duyệt (browsers) và các loại thiết bị (devices) khác nhau.
    
    - d. Vì sao nên sử dụng Foundation
    
       + Foundation được phát triển và hỗ trợ bởi ZURB - công ty sử dụng framework này cho hầu hết các dự án của họ từ những startup nhỏ tới các doanh nghiệp lớn. 
       Foundation đã được dùng và kiểm thử trong nhiều năm.
       
       + Hiện tại Foundation đã ra phiên bản 5 và nhiều lần release với những cải tiến đáng kể để chắc chắn rằng nó có thể hoạt động tốt và tương thích với nhiều môi trường khác nhau.
    
    - e. Cài đặt:
    
       + Với 3 lựa chọn:
         
         - Download Everything - Trọn bộ framework (gồm các components và plugins).
        
         - Download Essentials - Light version của framework bao gồm các thành phần: grid, typography, interchange, buttons và Reveal.
        
         - Custom Download - Tùy chọn những thành phần muốn tích hợp vào hệ thống, đồng thời có thể chủ động định nghĩa màu sắc (color), độ rộng cột (column size) hay font size, ...
    
    
    
    