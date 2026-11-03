# P99 · Sổ Tiến Độ

App theo dõi tiến độ bài hát và truyện của App P99, từ 1/11 đến 22/11/2026.
Hạn làm xong = giờ lên bài trừ 3 tiếng, tính theo giờ Bỉ. Giờ lên bài hiện cả giờ Bỉ và giờ Việt Nam.

- Bài hát: Viết bài → Sửa hoà thanh → Thu âm → Làm video → Upload
- Truyện: Viết truyện → Thu âm → Upload (mỗi phần một thẻ)

## Đưa lên GitHub Pages

1. Tạo repo mới trên GitHub, ví dụ `p99-tiendo`.
2. Bấm **Add file → Upload files**, kéo toàn bộ các file trong thư mục này vào, rồi bấm **Commit changes**.
3. Vào **Settings → Pages**. Ở mục *Source* chọn **Deploy from a branch**, chọn nhánh `main`, thư mục `/ (root)`, rồi bấm **Save**.
4. Đợi khoảng 1 phút. Link app sẽ có dạng `https://<tên-github>.github.io/p99-tiendo/`.

## Cài lên điện thoại

- **iPhone (Safari):** mở link → nút Chia sẻ → **Thêm vào MH chính**.
- **Android (Chrome):** mở link → menu ⋮ → **Cài đặt ứng dụng** (hoặc *Thêm vào màn hình chính*).

App mở toàn màn hình như app thật và vẫn dùng được khi mất mạng.

## Lưu ý về dữ liệu

- Những gì bạn tích được **lưu ngay trên máy đó** (bộ nhớ trình duyệt). Điện thoại và máy tính không đồng bộ với nhau.
- Nếu xoá dữ liệu trình duyệt hoặc gỡ app, các dấu tích sẽ mất và lịch quay về trạng thái ban đầu.
- Lịch gốc nằm trong `index.html`, ở dòng `window.P99_SEED = …`. Giờ ở đó là **giờ Việt Nam** (`date`, `time`).

## Các file

| File | Dùng để |
|---|---|
| `index.html` | Toàn bộ app và lịch |
| `manifest.webmanifest` | Tên, màu và icon khi cài lên điện thoại |
| `sw.js` | Cho phép mở app khi không có mạng |
| `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` | Icon app |
