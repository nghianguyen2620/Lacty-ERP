# LY ERP – Sơ đồ hệ thống & quy trình (tài liệu nội bộ)

Trang `index.html` là sơ đồ tương tác của LY ERP: 17 hệ thống, quy trình vận hành theo mã menu, quy trình từng nhà máy, tra cứu bảng và cột.

- **Xem bằng link chia sẻ** (dạng `…/Lacty-ERP/#k=…`): bấm là mở, không cần gõ mật khẩu; trình duyệt tự nhớ cho lần sau.
- Dữ liệu trong repo **được mã hóa** (AES-256-GCM, PBKDF2-SHA256 250.000 vòng). Phần `#k=…` của link không bao giờ được gửi lên máy chủ GitHub, nên ai không có link thì không đọc được nội dung.
- Địa chỉ IP nội bộ, đường dẫn mạng và tên người phát triển đã được che trước khi mã hóa. Trang có `noindex, nofollow`.
- Link chia sẻ **không** nằm trong repo; người quản lý gửi riêng cho người cần xem.

## Cập nhật
Bản nội bộ đầy đủ, file Excel và script phân tích chỉ lưu ở máy (thư mục `work/`, đã `.gitignore`). Sau khi dựng lại dữ liệu:

```
node work/publish.mjs
```

Lệnh trên tạo lại `index.html` (đã che & mã hóa), bản nội bộ `ERP_SoDo_HeThong_NoiBo.html` (không đưa lên git) và file link chia sẻ ở ngoài repo.
