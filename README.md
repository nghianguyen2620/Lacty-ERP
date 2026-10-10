# LY ERP – Sơ đồ hệ thống & quy trình (tài liệu nội bộ)

Trang `index.html` là sơ đồ tương tác của LY ERP: 17 hệ thống, quy trình vận hành theo mã menu, quy trình từng nhà máy, tra cứu bảng và cột.

- **Nội dung đã được mã hóa** (AES-256-GCM, khóa sinh từ mật khẩu bằng PBKDF2-SHA256 250.000 vòng) và giải mã ngay trong trình duyệt. Không có mật khẩu thì không đọc được dữ liệu.
- Các địa chỉ IP nội bộ, đường dẫn mạng và tên người phát triển đã được che trước khi mã hóa.
- Mật khẩu **không** nằm trong repo; người quản lý gửi riêng cho người cần xem.
- Trang có thẻ `noindex, nofollow` để công cụ tìm kiếm không lập chỉ mục.

## Xem
Mở link GitHub Pages của repo (hoặc mở file `index.html` bằng Chrome/Edge), nhập mật khẩu.

## Cập nhật
Bản nội bộ đầy đủ, file Excel và script phân tích chỉ lưu ở máy (thư mục `work/`, đã được `.gitignore`). Sau khi dựng lại dữ liệu:

```
node work/publish.mjs
```

Lệnh trên tạo lại `index.html` (đã che & mã hóa) và bản nội bộ `ERP_SoDo_HeThong_NoiBo.html` (không đưa lên git).
