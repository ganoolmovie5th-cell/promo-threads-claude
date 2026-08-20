# PromoIndo

Kumpulan promo, kode voucher, dan cashback Indonesia. Update otomatis setiap hari dari 21 akun Threads.

**Tech Stack:** HTML · CSS · JavaScript · Python (scraper) · GitHub Actions · Vercel

## Features

- Agregasi promo dari 21 akun Threads
- Update otomatis harian (08:00 WIB via GitHub Actions)
- Frontend statis (tanpa build step)
- Auto-deploy ke Vercel on push

## Getting Started

```bash
# Jalankan scraper manual
python scripts/scraper.py

# Serve frontend
cd public && python -m http.server 3000
```

## Project Structure

```
scripts/
  scraper.py          → Fetch promo dari 21 akun Threads
public/
  index.html          → Frontend
  data/promos.json    → Data promo (auto-generated)
.github/workflows/    → Daily scraper cron
```

## Deploy

Connected to Vercel. Auto-deploy on push to main.

## License

MIT
