# <h1 align="center">Bài 1: SỰ CỐ KHÔNG TRUY CẬP ĐƯỢC HỆ THỐNG QUẢN TRỊ</h1>
## Phần 1. Phân tích
- Input: phong-dieu-phoi.greenlog.vn
- Output: Địa chỉ IP của máy chủ (VD: 192.0.2.1)
- Sơ đồ luồng dữ liệu DNS:

`Brower Cache => OS Cache => Resolver (ISP) => Root DNS severs => Authoritative Name Server`

## Phần 2. Triển khai
- Lỗi **DNS_PROBE_FINISHED_NXDOMAIN** là lỗi ở Client/mạng (Máy chủ k bị sập)
- Lỗi **500 Internal Server Error** là lỗi ở sever (Yêu cầu đã đến máy chủ nhưng code/hệ thống phía sever gặp sự cố
=> Kiểm tra HTTP status code: Nhấn **F12** => Chọn tab **Network** => Tải lại trang (**F5**) để kiếm tra mã trạng thái (5xx hay lỗi kết nối)
## Phần 3. Kiếm thử
- Nếu sửa đúng tên miền mà nhận mã 404 Not Found: Tiến trình DNS và kết nối đến máy chủ đã thành công, nhưng đường dẫn (URL / trang web) Nam truy cập không tồn tại trên hệ thống