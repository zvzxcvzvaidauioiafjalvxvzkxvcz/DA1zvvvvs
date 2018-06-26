Tổng quan về trình biên dịch
===========================================

  - Trình biên dịch là một chương trình(thường viết bằng ngôn ngữ đích) dùng để dịch 1 chương trình nguồn thành 1 chương trình tương đương ở 1 ngôn ngữ khác. Quá trình chuyển đổi như vậy gọi là quá trình dịch và có các điểm chú ý sau:
    
    + Trong quá trình dịch luôn có cơ chế để phát hiện khắc phục lỗi

    + Tốc độ dịch phụ thuộc vào ngôn ngữ xây dựng nên nó và sự thông thoáng của thuật toán

    + Sự chính xác của trình biên dịch là tuyệt đối. Mọi sai lầm dù nhỏ nhất cũng sẽ gây lỗi nghiêm trọng
  
  - Mô hình phân tích và tổng hợp của trình biên dịch
   
    + Một trình biên dịch thường bao gồm 2 quá trình:

      - Phân tích -> đặc tả trung gian

      - Tổng hợp -> chương trình đích
    
    + Khi phân tích chương trình nguôn sẽ bị phân rã thành cây cú pháp (syntax tree) và mỗi nút là 1 toán tử còn các nhánh con là các toán hạn

  - Môi trường của trình biên dịch

    + Ngoài trình biên dịch chúng ta còn nhiều chương trình khác trong môi trường biên dịch bao gồm: 

      - Bộ tiền xử lý

      - Trình dịch hợp ngữ

      - Bộ tải và soạn thảo liên kết

  - Sự phân tích chương trình nguồn bao gồm:

    + Phân tích từ vựng (Lexical Analysis)
      
    + Phân tích cú pháp (Syntax Analysis)

    + Phân tích ngữ nghĩa ((Semantic Analysis)

  - Các giao đoạn biên dịch

    + Quản lý bảng ký hiệu

    + Xử lý lỗi

    + Các giai đoạn phân tích

    + Sinh mã trung gian

    + Tối ưu mã

    + Sinh mã

  - Chia thành 2 kì:

    + Kì đầu: Bao gồm các quas trình phân tích

    + Kì sau: Bao gồm sinh mã trung gian, tối ưu mã, sinh mã

  - Trong mọi quá trình không được bỏ qua kiểm tra lỗi và luôn luôn tìm các khắc phục lỗi có thể khắc phục