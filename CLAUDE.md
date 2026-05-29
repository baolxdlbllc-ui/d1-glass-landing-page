# CLAUDE.md — D1 Glass Landing Page (Thai)

Landing page cho sản phẩm **D1 Glass Polishing Liquid** — thị trường Thái Lan.

## Thông tin dự án

- **GitHub:** `github.com/baolxdlbllc-ui/d1-glass-landing-page` (public)
- **Vercel:** connect tới repo này → auto-deploy khi push lên `main`
- **Ngôn ngữ:** Tiếng Thái

## Chạy local

```bash
python3 -m http.server 8322 --directory "/Users/lexuanbao/Downloads/Khách hàng/c Thúy/Landing page D1 Thai"
# Mở: http://localhost:8322
```

## Kiến trúc

Single file: `index.html` (~1100 dòng)
- **CSS:** inline `<style>` — design tokens TikTok Shop style
- **JS:** inline `<script>` — gallery, scrollspy, countdown, popup form
- **Ảnh:** `./assets/images/` — commit vào git → Vercel serve được

## Các giá trị quan trọng

| Mục | Giá trị |
|---|---|
| Facebook Pixel | `1602655537448756` |
| Facebook Page | `https://www.facebook.com/profile.php?id=61588706097943` |
| Facebook Chat | `https://m.me/61588706097943` |
| Google Apps Script webhook | `PLACEHOLDER_WEBHOOK_D1_THAI` ← **cần thay** |
| Điện thoại | 0823.691.555 |

## Giá sản phẩm

| Combo | Giá |
|---|---|
| ซื้อ 1 แถม 1 (2 ขวด) | 299 บาท + ส่งฟรี |
| ซื้อ 2 แถม 1 (3 ขวด) | 399 บาท + ส่งฟรี |

## Workflow

```bash
# 1. Sửa index.html
# 2. Commit và push
git add index.html assets/
git commit -m "mô tả thay đổi"
git push origin main
# Vercel tự deploy
```

## Placeholder cần thay trước khi live

1. **`PLACEHOLDER_WEBHOOK_D1_THAI`** → URL Google Apps Script webhook nhận đơn hàng
   - Tạo Google Apps Script mới, deploy as web app
   - Copy URL dán vào thay thế placeholder trong `index.html`

## Ảnh trong dự án

| File | Vị trí |
|---|---|
| `d1-hero1.png` | Hero gallery slide 1 — ảnh sản phẩm chính |
| `d1-hero2.png` | Hero gallery slide 2 — features |
| `d1-beforeafter.png` | Hero slide 3 + section before/after |
| `d1-pain1.png` | Hero slide 4 + section pain points |
| `d1-usage.png` | Hero slide 5 + section usage guide |
| `d1-hero3.png` | Hero slide 6 + section feature |
| `d1-pain2.png` | Pain section image |
| `d1-product.png` | How-it-works section |
