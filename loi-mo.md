# Bảng lỗi mở (cập nhật 19:14 VN, 09/10)

| ID | Mức | Mô tả | Người sửa | Trạng thái |
|---|---|---|---|---|
| B1 | P1 | Trang đăng nhập hiện tài khoản demo / seed production tạo TK 123456 | FE + BE | Đã đóng (tester xác minh 19:13) |
| B2 | P1 | GV không thấy/xóa thông báo mình tạo | BE | Đã đóng (tester xác minh 19:13) |
| B3 | P1 | Xóa thông báo vẫn còn trong hộp thư phụ huynh | BE | Đã đóng (tester xác minh 19:13) |
| B4 | P2 | Thanh điều hướng mobile tràn (>5 tab) | FE | Đã đóng (tester xác minh 19:13) |
| B5 | P2 | Tổng quan BGH thiếu điểm danh theo lớp + "Cần chú ý" | BE + FE | Đã đóng (tester xác minh 19:13) |
| B6 | P2 | "Bé hôm nay" chưa có thẻ vàng "Đang chờ xác nhận" (dữ liệu test tên "Chờ") | FE | Đã đóng (tester xác minh 19:13) |
| B7 | P2 | Cờ quan trọng + gửi từng phụ huynh | BE + FE | Đã đóng (tester xác minh 19:13) |
| B8 | P2 | `/settings/school`, bỏ tên trường viết cứng | BE + FE | Chờ thông tin trường |
| B9 | P2 | Hẹn giờ + đính kèm ảnh thông báo | BE + FE | Sau khi lên server |
| B10 | P3 | Nút "Ghi thu" lệch, ô Quá hạn 2 số | FE | Đang sửa |
| B11 | P3 | Nhật ký ngủ trưa tràn ở 390px | FE | Đang sửa |
| B12 | P2 | Nhập học lại cho bé đã nghỉ | BE + FE | Sau tuần 3 |

Đã đóng: lỗi ảnh P0 (3), lỗi số dư khi chốt nghỉ P0.
Sẵn sàng khi: không còn P0/P1 và tester chạy lại toàn bộ sau lần build gộp.

## Sau nghiệm thu 1.0 (19:25)
| B13 | P1 | Nhập Excel: file lưu từ openpyxl/LibreOffice/Google Sheets bị 400 INVALID_FILE | BE | Mở |
| B14 | P1 | Nhập Excel: dòng có nhiều lỗi chỉ báo lỗi đầu (bỏ qua kiểm tra lớp) | BE | Mở |
| B15 | P3 | preview: dòng bỏ qua vẫn account "create" | BE | Mở |
| B16 | P3 | README thiếu 413; .env.example thiếu API_INTERNAL_URL | BE | Mở |
| B17 | P0 | Nhập Excel gắn nhầm phụ huynh khi SĐT trùng khác tên | BE + FE | Đã đóng (tester xác minh 19:37) |
| B18 | P1 | Lịch sử thay đổi nhạy cảm (gỡ liên kết, SĐT, đồng ý ảnh) lưu DB + màn xem cho BGH, không chỉ file log | BE + FE | Đang làm |
| B19 | P1 | API nhật ký ghi đè/xóa trường không gửi lên; cần PATCH từng phần | BE | Mở lại (tester 09/10: PATCH vẫn xóa trường không gửi), dev sửa trước 16:00 UTC |
