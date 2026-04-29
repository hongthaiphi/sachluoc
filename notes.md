Được. Update `_config.yml` thêm `permalink`:

```yaml
theme: jekyll-theme-tactile
baseurl: /sachluoc
url: https://hongthaiphi.github.io
permalink: /:title/
```

Options:
- `/:title/` → `/welcome-to-sachluoc/`
- `/posts/:title/` → `/posts/welcome-to-sachluoc/`
- `/blog/:year/:month/:title/` → `/blog/2026/04/welcome-to-sachluoc/`
- `/:year/:month/:title/` → `/2026/04/welcome-to-sachluoc/`

File `_posts/` vẫn giữ nguyên format `YYYY-MM-DD-*.md`, chỉ URL đầu ra thay đổi.