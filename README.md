# Luyện Đề Cùng Tớ 🐣 — Nhật ký IELTS

Website cá nhân theo dõi quá trình luyện đề IELTS Listening & Reading, giúp
nhận diện lỗi sai lặp lại và theo dõi tiến bộ band theo thời gian.

- 1 file HTML/CSS/JS duy nhất (`index.html`), không cần backend.
- Dữ liệu lưu trong `localStorage` của trình duyệt (chỉ trên máy/thiết bị bạn dùng).
- Mục tiêu: Listening 8.0 · Reading 7.5 · Ngày thi 27/12.

## Chạy thử ở máy

Chỉ cần mở trực tiếp file `index.html` bằng trình duyệt, hoặc chạy một server tĩnh bất kỳ, ví dụ:

```bash
npx serve .
```

## Đưa lên GitHub

```bash
git init
git add .
git commit -m "Init IELTS tracker"
git branch -M main
git remote add origin <URL_repo_github_cua_ban>
git push -u origin main
```

## Deploy lên Vercel

1. Vào https://vercel.com → **Add New Project** → chọn repo GitHub vừa tạo.
2. Vercel tự nhận đây là site tĩnh (Framework Preset: **Other**) — không cần Build Command,
   không cần Output Directory (root chứa sẵn `index.html`). Bấm **Deploy** là xong.
3. Mỗi lần bạn `git push`, Vercel sẽ tự deploy bản mới.

## Lưu ý về dữ liệu

Vì dữ liệu lưu ở `localStorage` (theo từng trình duyệt/thiết bị), khi đổi máy hoặc xóa cache
trình duyệt, dữ liệu sẽ không tự đồng bộ. Dùng nút 🎨 (góc trên bên phải) → **Xuất file sao lưu**
để tải file JSON, và **Nhập file sao lưu** ở máy khác để khôi phục.
