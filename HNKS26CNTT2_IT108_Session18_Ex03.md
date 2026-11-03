# <h1 align="center">Bài 3: Xử lý lỗi bố cục giao diện hệ thống theo dõi xe</h1>
## Phần 1. Phân tích
- Khung "Thông tin tài xế" và khung "Danh sách trạm" đang bị chồng lấn do thuộc tính margin hoặc position bị thiết lập chồng chéo.

- Kích thước thực tế của phần tử lỗi bị cộng dồn kích thước vùng đệm (Padding) và khoảng cách ngoài (Margin), khiến khung trên đè lên khung dưới trong cây DOM Tree.
## Phần 2. Triển khai
Thông số CSS mới
```
- Thông tin tài xế
margin-bottom: 20px
position: Relative
- Danh sách chạm
margin-top: 10px
```
## Phần 3. Kiểm thử
Do phần tử bị gán thuộc tính !important

=> Kiếm tra tab styles trong F12, tìm dòng thuộc tính bị gạch ngang, điều chỉnh lại thuộc tính position (chuyển về **relative** hoặc **static**)
