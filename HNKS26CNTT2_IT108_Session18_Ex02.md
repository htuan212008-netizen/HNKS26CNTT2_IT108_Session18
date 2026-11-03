# <h1 align="center">Bài 2 : Sự cố phiên làm việc trên hệ thống vận tải</h1>
## Phần 1. Phân tích
- **Cache**: Lưu trữ dữ liệu lớn (dung lượng từ MB đến GB) như tệp hình ảnh, CSS, JavaScript, HTML để tải trang nhanh hơn nhưng dễ bị lưu đệm (cần Hard Reload để làm mới).
- **Cookies**: Lưu trữ dữ liệu nhỏ (giới hạn tối đa ~4KB) như token định danh người dùng, phiên đăng nhập, truyền tải dữ liệu trực tiếp cùng HTTP request.
- ## Phần 2. Triển khai
- **Token**: Chuỗi định danh phiên làm việc của shipper.
- **Max-Age**: Thời gian sống của Cookie
- **Secure**: Đảm bảo Cookie chỉ được truyền tải qua giao thức HTTPS được mã hóa an toàn.
- **HttpOnly**: Ngăn chặn hoàn toàn mã JavaScript phía Client (như XSS scripts) truy cập vào Cookie, bảo vệ tài khoản khỏi Session Hijacking.
## Phần 3. Kiểm thử
**Xoá cache**
- Mở công cụ lập trình bằng phím `F12` (hoặc `Ctrl + Shift + I` trên Windows / `Cmd + Option + I` trên Mac).
- Nhấp chuột phải vào nút `Reload` cạnh thanh địa chỉ trình duyệt.
- Chọn dòng `Empty Cache and Hard Reload` để ép trình duyệt tải lại toàn bộ tài nguyên mới nhất, loại bỏ màu cũ từ giao diện cũ.