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
| B8 | P2 | `/settings/school`, bỏ tên trường viết cứng | BE + FE | Đã đóng (tester xác minh 09/10, TT trường thật) |
| B9 | P2 | Hẹn giờ + đính kèm ảnh thông báo | BE + FE | Code xong (BE 46bc523, web f678401), chờ tester + designer |
| B10 | P3 | Nút "Ghi thu" lệch, ô Quá hạn 2 số | FE | Đã đóng (designer xác minh 390px 09/10) |
| B11 | P3 | Nhật ký ngủ trưa tràn ở 390px | FE | Đã đóng (designer xác minh 390px 09/10) |
| B12 | P2 | Nhập học lại cho bé đã nghỉ | BE + FE | Đã đóng (tester 09/10; HP cả tháng, tiền ăn theo ngày – chờ BGH xác nhận) |

Đã đóng: lỗi ảnh P0 (3), lỗi số dư khi chốt nghỉ P0.
Sẵn sàng khi: không còn P0/P1 và tester chạy lại toàn bộ sau lần build gộp.

## Sau nghiệm thu 1.0 (19:25)
| B13 | P1 | Nhập Excel: file lưu từ openpyxl/LibreOffice/Google Sheets bị 400 INVALID_FILE | BE | Đã đóng (tester xác minh trên master 09/10) |
| B14 | P1 | Nhập Excel: dòng có nhiều lỗi chỉ báo lỗi đầu (bỏ qua kiểm tra lớp) | BE | Đã đóng (tester xác minh trên master 09/10) |
| B15 | P3 | preview: dòng bỏ qua vẫn account "create" | BE | Đạt khi đọc code (tester 09/10) |
| B16 | P3 | README thiếu 413; .env.example thiếu API_INTERNAL_URL | BE | Đã đóng (tester 09/10) |
| B17 | P0 | Nhập Excel gắn nhầm phụ huynh khi SĐT trùng khác tên | BE + FE | Đã đóng (tester xác minh 19:37) |
| B18 | P1 | Lịch sử thay đổi nhạy cảm (gỡ liên kết, SĐT, đồng ý ảnh) lưu DB + màn xem cho BGH, không chỉ file log | BE + FE | Đã đóng (tester + designer xác minh 09/10, đủ 3 loại) |
| B19 | P1 | API nhật ký ghi đè/xóa trường không gửi lên; cần PATCH từng phần | BE | Đã đóng (tester xác minh trên master 09/10) |

Lưu ý: nhánh chuẩn của backend là `master` (không phải `hotfix/import`).
| B20 | P2 | Lịch sử đổi SĐT: giá trị trước trống, cả 2 số dồn vào "sau" | BE | Đã đóng (tester xác minh 09/10) |
| B21 | P3 | Lịch sử SĐT: nhãn "đã đổi" (sky-500) vì che số làm 2 số khác nhau trông giống nhau; chữ tab /fees gãy dòng 390px | BE + FE | Đã đóng (tester API + designer 390px 09/10) |

Trạng thái 09/10: không còn P0/P1. Chờ tester chạy e2e trên bản build cuối.

## Đợt 3 – còn lại (09/10)
| Hạng mục | Trạng thái |
|---|---|
| Quản lý GV /staff (chấm công, ca, trông thay, nghỉ phép) | Code xong (BE 350bd9d, web cf9e612), chờ tester + designer |
| Thu chi /finance (chi >10tr BGH duyệt) | Code xong, chờ tester + designer |
| B9 hẹn giờ + ảnh thông báo | Chờ server |
| B22 | P3 | Bé học lại vẫn gợi ý hoàn tiền số dư | BE | Đã đóng (tester 09/10) |
| — | P3 | /staff "1 lớp · 2 ngày", /finance items-start | FE | Đã đóng (designer 09/10) |
| B23 | P2 | B9: ảnh đính kèm hiện sai thứ tự phía phụ huynh (nghi vấn) | BE + FE | Không phải lỗi (dev nhìn nhầm), đã thêm test f9ec1dc – đóng |
