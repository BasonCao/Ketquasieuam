# Dr Cao Bá Sơn – Ultrasound 5D PWA

Web/PWA offline-first dành cho nhập liệu và tạo phiếu kết quả siêu âm 5D.

## Mục tiêu
- Một hồ sơ bệnh nhân có nhiều lần siêu âm.
- Một form chung cho mốc 12 tuần, hình thái và tăng trưởng.
- Chạy offline bằng IndexedDB + Service Worker.
- Xuất/ in phiếu kết quả.
- Gemini AI chỉ là tính năng tùy chọn khi online; app cốt lõi không phụ thuộc AI.

## Nguồn dữ liệu
Cấu trúc trường được hợp nhất từ 3 mẫu DOCX người dùng cung cấp:
1. Thai5D.Moc12.Tuan.doc
2. Thai5DTangTruong.doc
3. Thai5D.HinhThai.doc

Không tự thêm tiêu chí chẩn đoán ngoài các trường có trong mẫu.

## Quy tắc
- 12 tuần: ưu tiên CRL, BPD, HC, BOD, NBL, NT và khảo sát cơ bản.
- Hình thái: hiển thị nhóm khảo sát não, tim, phổi, thành bụng, dạ dày, thận, bàng quang, dây rốn, chi.
- Tăng trưởng: hiển thị sinh trắc BPD/HC/AC/FL, EFW, percentile, Doppler và cổ tử cung khi có dữ liệu.
- Tổng hợp: cho phép hiển thị toàn bộ nhóm.

## Cảnh báo
Đây là phần mềm nhập liệu/tạo báo cáo, không tự động đưa ra chẩn đoán y khoa nếu chưa được bác sĩ xác nhận.
