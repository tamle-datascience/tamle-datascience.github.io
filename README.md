# my-website-modern

Website cá nhân phong cách Modern Editorial, xây dựng bằng Quarto.

## Thiết kế
- Font: Syne (display) + Manrope (body)
- Màu chủ: Indigo (#6366F1) + Coral (#F97316)
- Theme: Modern Editorial — clean, bold, animated

## Cấu trúc
```
my-website-modern/
├── _quarto.yml
├── styles.css
├── index.qmd
├── blog.qmd
├── publications.qmd
├── consulting.qmd
├── about.qmd
├── cv.pdf          ← Thay bằng CV thật
├── img/avatar.jpg  ← Thay bằng ảnh thật
└── .nojekyll
```

## Chạy local
```bash
quarto preview
```

## Deploy
```bash
quarto render
git add . && git commit -m "update" && git push
```
