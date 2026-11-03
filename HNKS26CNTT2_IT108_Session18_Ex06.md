# <h1 align="center">Bài 5 : Tối ưu tiện ích mở rộng cho hệ thống điều phối vận tải</h1>
## Phần 1: Phân tích
Nút thắt cổ chai: Do file ảnh bản đồ dung lượng quá lớn chưa nén kết hợp với các Request lỗi (Status 404) gây tốn thời gian chờ (timeout).
## Phần 2: Triển khai
**3 bước tối ưu:**

1. Sửa lỗi 404: Cập nhật lại chính xác URL các liên kết hỏng.
2. Nén hình ảnh: Chuyển sang định dạng WebP/AVIF và giảm dung lượng.
3. Bật Cache: Cấu hình Cache-Control trên server cho các tài nguyên tĩnh.
## Phần 3: Kiểm thử
**Mã 304 Not Modified:** Tín hiệu tốt vì tài nguyên trên trình duyệt trùng khớp với server, giúp tiết kiệm băng thông, giảm tải và tăng tốc độ tải trang gần như tức thì.
