# <h1 align="center">Bài 5 : Tối ưu tiện ích mở rộng cho hệ thống điều phối vận tải</h1>
## Phần 1: Phân tích
Dữ liệu GPS trả về từ máy chủ thường là một chuỗi JSON thô (Raw JSON) rất khó đọc, không phân cấp màu sắc và dễ gây sót lỗi khi theo dõi vị trí phương tiện.

JSON Viewer tự động định dạng lại cấu trúc JSON theo dạng cây (Tree view) có phân cấp màu sắc trực quan, giúp kỹ sư dễ dàng kiểm tra tọa độ vĩ độ/kinh độ, trạng thái xe và phát hiện nhanh các lỗi định dạng hoặc dữ liệu trả về sai lệch từ API.
## Phần 2: Triển khai
5 tiện ích thiết yếu:

Dev Suite: JSON Viewer Pro (soi JSON), Postman Interceptor (test API).

Productivity: ColorPick Eyedropper (chấm mã màu), GoFullPage (chụp màn hình).

Security: uBlock Origin (chặn quảng cáo & mã độc).
Nhấp vào biểu tượng Extensions (hình mảnh ghép) ở góc trên bên phải Chrome => Tìm tên tiện ích => Nhấp biểu tượng Pin (ghim) tương ứng.
## Phần 3: Kiểm thử
Nhập chrome://extensions vào thanh địa chỉ => Bật Developer mode => Nhấn Task Manager (hoặc dùng phím tắt Shift + Esc) => Quan sát cột Memory footprint để tìm và tắt extension gây lag.
