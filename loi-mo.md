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
- Staging: đơn nghỉ "QA-TEST-FAKE" của Cô Lan 10/10
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
| U10 | P1 | Bấm "Đã giao bé" → tự báo PH: ai đón, mấy giờ, ảnh. Trước mắt: thông báo đẩy + trong app; sau: Zalo ZNS/SMS (cần Zalo OA + chi phí, chờ anh/chị duyệt) | BE + FE | API đạt staging; chờ designer xem thông báo; Zalo/SMS: anh/chị chốt KHÔNG làm, chỉ báo trong app |
| B25 | P0 | Staging kẹt "Đang tải…": /health/ping 404 (Render chưa deploy 7757ea6), ServerWake thử lại mãi | BE + FE | Đã đóng (tester staging 09/10) |
| U11 | P3 | Nút "Con nghỉ hôm nay" chưa nổi (cần nền peach, cao 56px) | FE | Đã đóng (tester local 2d65984; chờ chạy lại staging) |

## Góp ý UX đợt 4 – Giáo viên (10/10 VN, staging)
| ID | Mức | Mô tả | Người | Trạng thái |
|---|---|---|---|---|
| G1 | P2 | Điểm danh: lưu xong không có "Đã lưu" | FE | Đã đóng (merge 215e89a) |
| G2 | P2 | Nhật ký: đang tải hiện "Lớp chưa có bé" → "Đang tải…"; hiện họ tên + ảnh bé | FE | Đóng (tester 09/10) |
| G3 | P3 | Nhật ký: giờ ngủ nhập phút; thêm mục uống nước | BE + FE | Đã đóng (merge e75c480) |
| G4 | P1 | Giao bé: bỏ tick bắt buộc "đối chiếu ảnh và căn cước" → "Đúng người đón"; thống nhất chữ "Đón bé"/"Giao bé" | FE | Đã đóng (tester local 2d65984; chờ chạy lại staging) |
| G5 | P2 | Chấm công GV: đưa Vào ca/Ra ca ra trang đầu; đổi "Ca sáng" → "Ca ngày" | FE + BE | Đã đóng (tester local 2d65984; chờ chạy lại staging) |
| G6 | P1 | Nghỉ phép: loại nghỉ (ốm, phép năm, việc riêng) + nửa ngày; "BGH" → "Ban giám hiệu" | BE + FE | Đã đóng (tester local 2d65984; chờ chạy lại staging) |
| G7 | P1 | Luồng nghỉ phép → trông thay: GV gửi đơn → báo BGH duyệt + nhắc phân trông thay; duyệt/từ chối → báo GV; GV ghi chú bàn giao lớp cho cô trông thay | BE + FE | Đã đóng (tester local 2d65984; chờ chạy lại staging) |
| G8 | P1 | Ngày có cô trông thay: báo PH lớp tên cô trông thay; dặn thuốc tự chuyển sang cô trông thay, "Đã cho uống" ghi giờ + báo PH | BE + FE | Đã đóng (tester local 2d65984; chờ chạy lại staging) |

## Góp ý UX đợt 4 – Hiệu trưởng (10/10 VN)
| ID | Mức | Mô tả | Người | Trạng thái |
|---|---|---|---|---|
| H1 | P1 | Bấm thông báo đơn nghỉ chỉ đánh dấu đã đọc → mở thẳng trang duyệt (Duyệt/Từ chối + phân trông thay); gộp vào G7 | FE + BE | Đã đóng (tester local 2d65984; chờ chạy lại staging) |
| H2 | P2 | Nhật ký thao tác hiện chữ kỹ thuật (finance.expense.create, amount, out), tiền thiếu dấu chấm | FE | Đóng (tester 09/10) |
| H3 | P2 | Nhiều trang hiện "0 trẻ"/"Lớp chưa có bé"/"0 tài khoản" khi đang tải → "Đang tải…" (gộp G2) | FE | Đóng (merge main web 834eec2) |
| H4 | P1 | Đã đăng nhập, mở trang chủ vẫn ra trang đăng nhập → chuyển thẳng vào trang theo vai trò | FE | Đã đóng (tester local 2d65984; chờ chạy lại staging) |

## Góp ý PH lần 2 (10/10 VN)
| ID | Mức | Mô tả | Người | Trạng thái |
|---|---|---|---|---|
| P1 | P2 | Trang học phí khi đã đóng đủ vẫn hiện "Còn nợ 0đ · Quá hạn 0đ · Số dư 0đ" → chỉ ghi "Đã đóng đủ"; ẩn dòng 0đ | FE | Đã đóng (merge e75c480) |
| P2 | P2 | Còn chữ "căn cước", lỗi chính tả "Cabin cước chưa có", "BMI" ở trang PH | FE | Đã đóng (merge e75c480) |
| P3 | P2 | Bảng "Bạn đã chặn thông báo…" nằm mãi trên trang đầu → nói dễ hiểu + nút ẩn | FE | Đã đóng (merge e75c480) |
| P4 | P3 | Báo nghỉ khi bé đã có mặt: "Hôm nay bé đã đi học rồi" | FE | Đã đóng (merge e75c480) |
| P5 | P3 | "ĐÃ QUA"/"không được hoàn tiền ăn" → "Báo trước 8 giờ sáng thì trường trả lại tiền ăn" | FE | Đã đóng (merge e75c480) |
| P6 | P3 | Trên máy tính PH vẫn có menu bên 10 mục → dùng cùng 5 mục như điện thoại | FE | Đã đóng (merge e75c480) |
| P7 | — | Ảnh lớp là ảnh mẫu: chờ R2 + trường đăng ảnh thật | — | Chờ R2 |

## Ảnh lớp & đồng ý (10/10 VN)
| ID | Mức | Mô tả | Người | Trạng thái |
|---|---|---|---|---|
| A1 | P1 | Lúc GV chọn ảnh: hiện danh sách + ảnh bé CHƯA đồng ý; ảnh gắn bé chưa đồng ý bị đánh dấu/làm mờ, chặn đăng nếu chưa xử lý | BE + FE + design | Đóng (tester 09/10) |
| A2 | P1 | PH: câu rõ "Cho cô đăng hình con lên nhóm lớp: Có / Không"; hỏi ngay lần đầu mở app; đổi được ở Tài khoản (ghi lịch sử B18) | FE + BE | Đóng (tester 09/10) |
| G9 | P2 | Ca trong DB vẫn tên "Ca sáng" (hiện trong tin trông thay, trang duyệt) → migration đổi "Ca ngày" | BE | Đã đóng (tester staging) |
| G10 | P2 | Khung lỗi hiện tiếng Anh ("Failed to fetch", "Internal server error") → câu tiếng Việt, vd "Chưa lưu được, kiểm tra mạng rồi bấm Lưu lại" (msgErrorText, toàn app) | FE | Đã đóng (merge 6284d6e) |

## Góp ý Hiệu trưởng – thử lại luồng nghỉ phép (09/10)
| ID | Mức | Mô tả | Người | Trạng thái |
|---|---|---|---|---|
| H5 | P1 | Đóng tab mở lại vẫn bị đòi đăng nhập (phải nhớ phiên) | FE + BE | Dev đang làm |
| H6 | P1 | Chấm công tuần 12/10: không hiện cô Mai trông thay; "Cần trông thay"/"Nghỉ phép" = 0. Cần ghi "Trông thay Mầm 1" trên dòng cô Mai + cộng đúng ngày nghỉ | BE + FE | Đóng (tester staging 09/10) |
| H7 | P2 | Tổng quan hiện "Số lớp 0" trước khi tải xong → "Đang tải…" | FE | Đóng (merge main web 834eec2) |

## Góp ý Cô giáo – thử lại (09/10)
| ID | Mức | Mô tả | Người | Trạng thái |
|---|---|---|---|---|
| G11 | P1 | Nút Vào ca/Ra ca trang đầu chỉ hiện giờ, bấm không ăn | FE + BE | Đóng (tester staging 09/10) |
| G12 | P2 | Thống nhất chữ "Giao bé" (mục Thêm còn ghi "Đón bé") | FE | Đóng (merge main web 834eec2) |
| G13 | P2 | Điểm danh hiện 0/danh sách trống khi tải → "Đang tải…" | FE | Đóng (merge main web 834eec2) |
| G14 | P1 | Điểm danh: bấm 1 lần đổi Có mặt/Vắng, lý do ghi sau (không bật hộp lý do) | FE | Đóng (tester 25/25, web 0a25df9) |

## Góp ý Phụ huynh – thử lại (09/10)
| ID | Mức | Mô tả | Người | Trạng thái |
|---|---|---|---|---|
| P8 | P1 | Học phí: ngoài "Đã đóng đủ" nhưng trong vẫn "Còn nợ 0đ · Quá hạn 0đ" → khi đủ thì ẩn dòng nợ, chỉ ghi "Đã đóng đủ" | FE | Đóng (merge main web 834eec2) |
| P9 | P2 | Trang đầu hiện thẻ cô trông thay ("Thứ Hai cô Mai trông con") thay vì chỉ "Bạn có 3 thông báo" | FE + BE | Đóng (tester 18/18, merge web 0a25df9) |
| P10 | P2 | Hỏi đồng ý đăng hình: hiện ở trang đầu; chỉnh lại được trong Tài khoản (đang chỉ ở Hồ sơ bé) | FE | Đóng (merge main web 834eec2) |
| P11 | P2 | Tài khoản: "Cài đặt thông báo" trông như nút mà bấm không ăn | FE | Đóng (tester staging 09/10) |
| P12 | P2 | Nhắn cô: cảnh báo "Đã quá 08:00…" chỉ hiện sau khi chọn ngày hôm nay | FE | Đóng (merge main web 834eec2) |
| P13 | P1 | Ô điểm danh trang đầu lúc "Chưa điểm danh" lúc "Bé đã đến lớp" (không nhất quán) | FE + BE | Mở lại: dòng ngày trang Hôm nay chưa theo giờ VN (today/page.tsx:57), dev sửa |
| A3 | P3 | Lịch sử thay đổi: cột "Người sửa" hiện tên đăng nhập thay vì tên hiển thị | BE | Đóng (tester staging 09/10) |
| H8 | P3 | Nhật ký thao tác BGH còn nhãn "Đón bé" (audit-api.ts:35) → "Giao bé" | FE | Mở |
| G15 | P3 | /home lúc tải hiện "✓ Vào ca" khoá dù đã ra ca → "Đang tải…" | FE (designer) | Mở |
| H9 | P3 | API /staff/attendance trả pending thay vì sub cho ngày trông thay; Ra ca đồng thời trả alreadyCheckedOut sai | BE | Mở |
| P14 | P3 | Thông báo PH "có mặt dù đã báo vắng" ghi ngày 2026-10-10 → "Thứ Bảy 10/10" | BE | Mở |
