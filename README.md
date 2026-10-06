# PAW Week 2 — Kelompok 5 Kelas B

Landing page ringkasan jurnal: **Implementasi Algoritma Genetika untuk Otomatisasi Penjadwalan Akademik Guna Menghindari Conflict of Schedule**.

Branch: `yuum` — refactor tampilan ke **mobile-first responsif**, simpel, tanpa AI slop (ikut panduan `impeccable adapt`).

## Tampilan

### Desktop (1280px)

![Tampilan desktop](docs/screenshots/desktop.png)

### Mobile (390px)

![Tampilan mobile](docs/screenshots/mobile.png)

## Perubahan di branch `yuum`

- Mobile-first CSS: base 1 kolom untuk 320px+, `min-width: 640px` (tablet), `min-width: 1024px` (desktop 2 kolom).
- Nav bisa geser horizontal di ponsel (tanpa JS), rata tengah + wrap di tablet/desktop. Target sentuh min 44px.
- `viewport-fit=cover` + `env(safe-area-inset-*)`, `text-wrap: balance/pretty`, skip-link, `prefers-reduced-motion`, hover hanya di `(hover: hover)`.
- Pertahankan identitas warna navy yang sudah ada (tidak ganti palet, tidak tambah gradient/glassmorphism).
- Meta `description` + `theme-color`, favicon inline agar tidak 404, daftar anggota jadi grid responsif (1 → 2 → 3 kolom).

## Cara lihat

```bash
git checkout yuum
python -m http.server 8123
# buka http://localhost:8123/index.html
```
