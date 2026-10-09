# Danh sách kiểm thử tổng & nghiệm thu – Web quản lý trẻ mầm non

Điều kiện xong: 8 tính năng có giao diện chạy trên API thật, toàn bộ test qua, 0 lỗi P0/P1, triển khai bằng 1 lệnh.

| # | Tính năng | Kiểm tra chính | Vai trò thử |
|---|---|---|---|
| 1 | Hồ sơ trẻ | Tạo/sửa/tìm không dấu, phân trang, ảnh có quyền, avatar mặc định, bé nghỉ (withdraw) bị ẩn + nhãn "Đã nghỉ" | admin, gv1, ph1, ketoan |
| 2 | Lớp & giáo viên | Tạo lớp, gán GV, GV chỉ thấy lớp mình (403 lớp khác) | admin, gv1 |
| 3 | Điểm danh & đón | 4 trạng thái, sửa lùi ≤3 ngày + lịch sử, yêu cầu đón chờ/duyệt/từ chối/hết hạn 2h, cấm đón 403 | gv1, admin, ph1, ph2 |
| 4 | Sức khỏe & dinh dưỡng | Chiều cao/cân nặng/BMI + biểu đồ, thực đơn tuần + món thay thế dị ứng, nhật ký ngày | gv1, admin, ph1, ketoan(403) |
| 5 | Học phí | Tạo hóa đơn (không trùng hoàn tiền ăn), trả trước/số dư, giảm trừ ≤0đ + cảnh báo, quá hạn 00:01 ngày 11, hủy có lý do, bé nghỉ + phiếu chi, biên lai bằng chữ + thông tin trường thật | ketoan, admin, ph1, gv1(403) |
| 6 | Liên lạc phụ huynh | Thông báo toàn trường/lớp/cá nhân, hẹn giờ, hộp thư, thông báo yêu cầu đón | admin, gv1, ph1 |
| 7 | Báo cáo | Chuyên cần, sĩ số, thu chi, xuất Excel, số liệu khớp dữ liệu thật | admin, ketoan |
| 8 | Tài khoản & bảo mật | Tạo TK, bắt đổi MK lần đầu, khóa 5 lần/15 phút + giờ VN, mở khóa, phụ huynh do trường tạo | admin, mọi vai trò |

Phi chức năng: mobile 390px không tràn, ô chạm ≥48px; Docker Compose 1 lệnh; sao lưu DB hằng ngày + thử khôi phục; HTTPS; `.env` mẫu; không reset dữ liệu khi khởi động lại.

Buổi nghiệm thu (khi front end xong tuần 3): tester chạy lại toàn bộ script + Playwright; mỗi vai trò đi trọn 1 ngày mẫu (điểm danh sáng → nhật ký → đón chiều → kế toán thu tiền cuối tháng → phụ huynh xem "Bé hôm nay"); ghi lỗi theo P0–P3; chốt khi 0 P0/P1.
