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
| B9 | P2 | Hẹn giờ + đính kèm ảnh thông báo | BE + FE | Đã đóng (tester API 18/18 + designer UI 09/10) |
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
| B24 | P3 | B9 UI: giờ 12h→24h, ô ngày đè icon 390px, thiếu nhãn "✓ Đã gửi" + số người xem | FE | Đã đóng (designer xác minh 0ce058b) |

## Dữ liệu test cần xoá khi dọn DB
- Khoản chi QA 11tr, "QA chờ duyệt" 10,5tr, "QA chi lớn"
- Tin "QA hẹn giờ (sửa)" (2 bản), "Lễ hội Trung thu 2026" (gửi 2 lần)
- Bé "QA Học Phí 47d8"
- Chụp lại ảnh hướng dẫn sử dụng sau khi dọn

Trạng thái 09/10 22:40 VN: không còn lỗi mở. Chờ deploy staging (Render kẹt captcha).

## Góp ý UX đợt 4 – Phụ huynh (09/10, staging)
| ID | Mức | Mô tả | Người | Trạng thái |
|---|---|---|---|---|
| U1 | P1 | Mở app chậm ~20s (Render ngủ), trang trắng khi tải → cần skeleton/"Đang tải…" + giữ backend thức | BE + FE | Đã đóng (ping 200, chốt an toàn 3e56ac0) |
| U2 | P1 | Trang đầu: "Học phí còn nợ" mâu thuẫn "Đã đóng đủ" | FE + BE | Đã đóng (tester staging: đóng đủ + còn nợ) |
| U3 | P1 | Ô Thực đơn / Nhật ký / Học phí / "Chưa điểm danh" trông như nút nhưng bấm không được | FE | Đã đóng (tester staging 10/10) |
| U4 | P1 | Báo nghỉ 1 chạm "Con nghỉ hôm nay" (lý do tuỳ chọn) | FE + BE | Đã đóng (tester staging 10/10) |
| U5 | P2 | Người đón hộ: PH chỉ nhập tên + SĐT; ảnh tuỳ chọn, GV chụp ở lần đón đầu; thẻ bé hiện ảnh + tên + nút gọi nhanh PH | BE + FE + design | API đạt staging 13/13; chờ designer chụp thẻ giao bé |
| U6 | P2 | Bỏ thuật ngữ: CCCD→"Số căn cước", BMI, HH:MM, album; "–kg"→"Chưa cân" | FE | Đã đóng (staging) |
| U7 | P2 | PH chỉ 1 menu (thanh dưới ≤5 mục), bỏ menu bên | FE + design | Đã đóng (designer staging 390px) |
| U8 | P2 | Chữ to hơn cho PH (≥17px), Đăng xuất tách xa tên; lời mời bật thông báo dễ hiểu | FE + design | Đã đóng (staging) |
| U9 | P3 | Staging thiếu dữ liệu mẫu (ảnh, thực đơn, thông báo, học phí) | BE | Đã xong (dữ liệu mẫu staging; xoá bằng npm run demo:purge) |
| U10 | P1 | Bấm "Đã giao bé" → tự báo PH: ai đón, mấy giờ, ảnh. Trước mắt: thông báo đẩy + trong app; sau: Zalo ZNS/SMS (cần Zalo OA + chi phí, chờ anh/chị duyệt) | BE + FE | API đạt staging; chờ designer xem thông báo; Zalo/SMS chờ anh/chị duyệt |
| B25 | P0 | Staging kẹt "Đang tải…": /health/ping 404 (Render chưa deploy 7757ea6), ServerWake thử lại mãi | BE + FE | Đã đóng (tester staging 09/10) |
| U11 | P3 | Nút "Con nghỉ hôm nay" chưa nổi (cần nền peach, cao 56px) | FE | Dev sửa trước 17:20 UTC |

## Góp ý UX đợt 4 – Giáo viên (10/10 VN, staging)
| ID | Mức | Mô tả | Người | Trạng thái |
|---|---|---|---|---|
| G1 | P2 | Điểm danh: lưu xong không có "Đã lưu" | FE | Mở |
| G2 | P2 | Nhật ký: đang tải hiện "Lớp chưa có bé" → "Đang tải…"; hiện họ tên + ảnh bé | FE | Mở |
| G3 | P3 | Nhật ký: giờ ngủ nhập phút; thêm mục uống nước | BE + FE | Mở |
| G4 | P1 | Giao bé: bỏ tick bắt buộc "đối chiếu ảnh và căn cước" → "Đúng người đón"; thống nhất chữ "Đón bé"/"Giao bé" | FE | Mở |
| G5 | P2 | Chấm công GV: đưa Vào ca/Ra ca ra trang đầu; đổi "Ca sáng" → "Ca ngày" | FE + BE | Mở |
| G6 | P1 | Nghỉ phép: loại nghỉ (ốm, phép năm, việc riêng) + nửa ngày; "BGH" → "Ban giám hiệu" | BE + FE | Mở |
| G7 | P1 | Luồng nghỉ phép → trông thay: GV gửi đơn → báo BGH duyệt + nhắc phân trông thay; duyệt/từ chối → báo GV; GV ghi chú bàn giao lớp cho cô trông thay | BE + FE | Mở |
| G8 | P1 | Ngày có cô trông thay: báo PH lớp tên cô trông thay; dặn thuốc tự chuyển sang cô trông thay, "Đã cho uống" ghi giờ + báo PH | BE + FE | Mở |
