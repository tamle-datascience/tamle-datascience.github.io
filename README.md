# my-website-r

Website cá nhân viết bằng **Quarto + Markdown thuần** (không cần biết HTML).

## Cách chỉnh sửa nội dung

Mở các file `.qmd` và sửa phần văn bản Markdown:
- `index.qmd` — Trang chủ
- `about.qmd` — Giới thiệu bản thân
- `publications.qmd` — Danh sách publications
- `consulting.qmd` — Khoá đào tạo
- `posts/*/index.qmd` — Các bài blog (thêm bài mới = tạo thư mục mới trong posts/)

**Không cần đụng vào `styles.css`** — toàn bộ thiết kế đã nằm trong đó.

## Cú pháp đặc biệt (chỉ vài cái đơn giản)

- Nút: `[Văn bản](link){.btn-primary}` hoặc `{.btn-outline}`
- Thẻ tag: `[R]{.tag}` (hoặc `.tag-green`, `.tag-orange`, `.tag-yellow`)
- Chữ gradient: `[chữ]{.grad}`
- Card: bọc nội dung trong `::: {.card-soft}` ... `:::`
- Nhãn nhỏ: `[NHÃN]{.label}`

## Thêm bài blog mới

1. Tạo thư mục mới: `posts/ten-bai-viet/`
2. Tạo file `index.qmd` với phần header:
   ```
   ---
   title: "Tiêu đề"
   description: "Mô tả ngắn"
   date: "2025-04-01"
   categories: [R]
   ---
   ```
3. Viết nội dung bằng Markdown bên dưới.
Trang Blog sẽ **tự động** cập nhật danh sách.

## Chạy & deploy

```bash
quarto preview    # Xem thử
quarto render     # Build ra /docs
```
Sau đó push lên GitHub Pages (xem deploy-guide.pdf).

## Thay thông tin cá nhân

Tìm và thay các placeholder: `[Tên của bạn]`, `email@example.com`, `username`, `[Họ và tên đầy đủ]`, `202X`, ảnh `img/avatar.jpg`, file `cv.pdf`.
