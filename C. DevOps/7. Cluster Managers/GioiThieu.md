Giới thiệu Cluster 
==========================================

# I. Tổng quan

  - cần có một giải pháp để đảm bảo cho hệ thống vẫn hoạt động tốt ngay cả khi có sự cố xảy ra đối với máy chủ mạng, và công nghệ clustering là câu trả lời cho vấn đề này
  
# II. Cluster là gì ?

  - Clustering là một kiến trúc nhằm đảm bảo nâng cao khả năng sẵn sàng cho các hệ thống mạng máy tính
  
  - Clustering cho phép nhiều máy chủ có thể liên kết với nhau theo dạng song song hoặc phân tán và được sử dụng như một tài nguyên thống nhất. 
    
  - Nếu một máy chủ ngừng hoạt động do bị sự cố hoặc để nâng cấp, bảo trì, thì toàn bộ công việc mà máy chủ này đảm nhận sẽ được tự động chuyển sang cho một máy chủ khác `(trong cùng một cluster)` 
  mà không làm cho hoạt động của hệ thống bị ngắt hay gián đoạn. Quá trình này gọi là `fail-over`; và việc phục hồi tài nguyên của một máy chủ trong hệ thống (cluster) 
  được gọi là `fail-back`.
  
  - Việc thiết kế và lắp đặt các cluster cần thoả mãn các yêu cầu sau:
  
    + `Yêu cầu về tính sẵn sàng cao (High availability)` : Các tài nguyên mạng phải luôn sẵn sàng cung cấp và phục vụ người dùng cuối và giảm thiểu sự ngưng hoạt động ngoài ý muốn
    
    + `Yêu cầu về độ tin cậy cao (reliability)` : Giảm thiểu tần số xảy ra sự cố, và nâng cao khả năng chịu đựng sai sót của hệ thống.
    
    + `Yêu cầu về khả năng mở rộng được (scalability)` :  Hệ thống phải có khả năng dễ dàng cho việc nâng cấp, mở rộng trong tương lai bao gồm các nâng cấp và mở rộng sau:
        
       - các thiết bị, máy tính vào hệ thống để nâng cao chất lượng dịch vụ
       
       - số lượng người dùng, thêm ứng dụng, dịch vụ và thêm các tài nguyên mạng khác
       
    + Ba yêu cầu trên được gọi tắt là `RAS (Reliability–Availability–Scalability)`, những hệ thống đáp ứng được ba yêu cầu trên được gọi là hệ thống `RAS`
     (cần phân biệt với `Remote Access Service` là dịch vụ truy cập từ xa).
     
     
  - Kỹ thuật Clustering được chia làm 2 loại gồm Cluster và Network Load Balancing (NLB)