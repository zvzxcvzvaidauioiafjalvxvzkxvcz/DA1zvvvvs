Giới thiệu ngôn ngữ lập trình mới
=================================================

# Mục lục

  - 1. Tổng quan về trình viên dịch
  
  - 2. Các trình biên dịch
  
  - 3. công cụ

  - 4. Tổng quan về các ngôn ngữ lập trình

    + 4.1. Cú pháp

    + 4.2. Thế mạnh

    + 4.3. Điểm yếu

  - 5. Các framework trong các ngôn ngữ lập trình
   
    + 5.1. Khái niệm

    + 5.2. Ví dụ

  - 6. So sánh tổng quan về các ngôn ngữ

  - 7. Đề xuất ngôn ngũ mới

# I. Tổng quan về trình biên dịch

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

## II. Các trình biên dịch

  - 1. Ada compilers

  - 2. ALGOL compilers

  - 3. Assemblers (Intel *86)

  - 4. Assemblers (Motorola 68*)

  - 5. Assemblers (Zilog Z80)

  - 6. Assemblers (other)

  - 7. BASIC Compilers

  - 8. BASIC interpreters

  - 9. Batch compilers

  - 10. C compilers

  - 11. Source-to-source compilers

  - 12. C++ compilers

  - 13. C# compilers

  - 14. COBOL compilers

  - 15. Common Lisp compilers

  - 16. D compilers

  - 17. DIBOL/DBL compilers

  - 18. ECMAScript interpreters

  - 19. Eiffel compilers

  - 20. Fortran compilers

  - 21. Go compilers

  - 22. Haskell compilers

  - 23. Java compilers

  - 24. Pascal compilers

  - 25. Perl Interpreters

  - 26. PL/I compilers

  - 27. Python compilers

  - 28. Scheme compilers and interpreters

  - 29. Smalltalk compilers

  - 30. Tcl Interpreters

  - 31. VMS Interpreters

  - 32. Rexx Interpreters

  - 33. CLI compilers

  - 34. Open source compilers

  - 35. Research compilers

  - 36. See also

  - 37. Footnotes

  - 38. References

  - 39. External links

# III. Các công cụ hỗ trợ:

  - 1. Parser generators.

  - 2. Scanner generators.

  - 3. Syntax-directed translation engines.

  - 4. Automatic code generators.

  - 5. Data-flow analysis engines.
  
  - 6. Compiler-construction toolkits
