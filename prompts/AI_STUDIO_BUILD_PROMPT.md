# PROMPT DÙNG TRONG GOOGLE AI STUDIO

Bạn là kỹ sư phần mềm senior chuyên xây dựng PWA offline-first cho phòng khám.

Hãy xây dựng một Web App/PWA tên:
**Dr Cao Bá Sơn – Siêu âm 5D**

Đọc `schemas/ultrasound_schema.json`, `rules/ultrasound_rules.json` và `README.md` trước khi code.

## Yêu cầu kỹ thuật
- React + TypeScript + Vite.
- PWA cài được trên Android/Chrome.
- Offline-first.
- IndexedDB để lưu bệnh nhân, thai kỳ, lần siêu âm và ảnh.
- Service Worker cache app shell để mở và dùng khi mất mạng.
- Không bắt buộc backend.
- Không bắt buộc Gemini để app hoạt động.
- Responsive, ưu tiên màn hình điện thoại.
- Giao diện tiếng Việt.
- Có tìm kiếm bệnh nhân.
- Một bệnh nhân có nhiều lần siêu âm.
- Có tạo/sửa/xóa bản nháp.
- Có autosave.
- Có nút Xuất PDF/In.
- Có thể nhập ảnh siêu âm và xem thumbnail.
- Khi online có thể thêm module Gemini nhưng phải tách khỏi logic offline.

## Form
Tạo một form chung. Người dùng chọn:
1. Mốc 12 tuần
2. Hình thái
3. Tăng trưởng
4. Tổng hợp

Dựa vào `ultrasound_rules.json` để tự động hiện/ẩn nhóm trường.

Không tự ý thêm các tiêu chí chẩn đoán hoặc giá trị tham chiếu y khoa không có trong các file nguồn.

## Kết quả
Phiếu phải có:
- Header: BS CAO BÁ SƠN - SIÊU ÂM 5D CHUYÊN SÂU
- HD57 Hải Đăng 9 - Vinhomes Ocean Park
- Hotline 0967.275.799
- Thông tin bệnh nhân
- Thông tin thai
- Sinh trắc
- Hình thái
- Doppler
- Kết luận
- Hình ảnh
- Bác sỹ chuyên khoa / Cao Bá Sơn

## Quy tắc an toàn
Không tự động biến một giá trị đo thành chẩn đoán bệnh.
Kết luận do bác sĩ nhập hoặc xác nhận.
Nếu thiếu dữ liệu, để trống hoặc cảnh báo thiếu dữ liệu; không tự suy đoán.

## Tiêu chí hoàn thành
1. `npm install`
2. `npm run dev`
3. `npm run build`
4. `npm run preview`
đều hoạt động.
Tạo README hướng dẫn chạy.
