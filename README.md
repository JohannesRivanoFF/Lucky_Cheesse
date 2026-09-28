# 🧀 Lucky Cheese Kediri — Korean Cheese Coin Pancake

Website resmi **Lucky Cheese Kediri** — toko Korean Cheese Coin Pancake (코인빵) dengan mozzarella premium yang meleleh di setiap gigitan.

## 🌐 Tech Stack

| Layer | Teknologi |
|-------|-----------|
| **HTML** | HTML5 Semantic + SEO-optimized |
| **CSS** | Tailwind CSS v3 (CDN) + Custom CSS |
| **JavaScript** | Vanilla JS (ES6+) |
| **Icons** | Font Awesome 6 |
| **Fonts** | Google Fonts (Cormorant Garamond, Playfair Display, Plus Jakarta Sans) |
| **Deploy** | Vercel (Static Site) |

> ℹ️ Ini adalah **Static HTML Site** murni — tidak memerlukan build step atau framework backend.  
> PHP Laravel dapat diintegrasikan untuk fitur backend seperti order management di masa mendatang.

---

## 🚀 Deploy ke Vercel

### Cara 1 — Import dari GitHub (Rekomendasi)

1. Push repo ini ke GitHub
2. Login ke [vercel.com](https://vercel.com)
3. Klik **"Add New Project"** → Import dari GitHub
4. Pilih repo `Lucky_Cheesse`
5. **Framework Preset**: pilih **"Other"**
6. **Build Command**: kosongkan (atau `echo done`)
7. **Output Directory**: `.` (titik — folder root)
8. Klik **Deploy** ✅

### Cara 2 — Via Vercel CLI

```bash
npm i -g vercel
vercel login
vercel --prod
```

### Konfigurasi Vercel (`vercel.json`)

File `vercel.json` sudah dikonfigurasi:
- **No build command** — serve langsung dari root
- **Cache headers** optimal untuk gambar
- **SPA rewrite** fallback

---

## 📁 Struktur Proyek

```
Lucky_Cheesse/
├── index.html          ← Main website (HTML + Tailwind + Vanilla JS)
├── public/
│   └── images/         ← Gambar produk (served sebagai /images/...)
│       ├── lucky_cheese_hero_*.jpg
│       ├── double_mozzarella_*.jpg
│       ├── nutella_choco_coin_*.jpg
│       └── pistachio_kunafa_*.jpg
├── vercel.json         ← Konfigurasi Vercel deployment
├── package.json        ← Project metadata
└── README.md
```

---

## 🛠️ Development Lokal

### Dengan XAMPP (PHP)
Akses langsung via: `http://localhost/Lucky_Cheesse/`

### Dengan Node.js / Vite Dev Server
```bash
npm install
npm run dev
# Buka http://localhost:3000
```

### Dengan Python (Quick)
```bash
python -m http.server 3000
# Buka http://localhost:3000
```

---

## ✨ Fitur Website

- 📱 **Responsive** — Mobile-first design
- 🛒 **Shopping Cart** — Keranjang belanja dengan promo Buy 2 Free 1
- 💬 **WhatsApp Pre-Order** — Generate pesan otomatis ke WA penjual
- 💳 **QRIS Payment** — Simulasi pembayaran via QR code
- 🔍 **Filter & Search Menu** — Filter kategori + live search
- 🌙 **Dark Mode** — Luxury dark culinary design
- ⚡ **Animasi Premium** — Glassmorphism, ambient glow, hover effects

---

## 🔧 Customization

### Ubah Nomor WhatsApp
Di `index.html`, cari:
```javascript
const waNumber = "6281234567890";
```
Ganti dengan nomor WA aktif (format: 62xxxxxxxxxx, tanpa +).

### Ubah Alamat Gerai
Cari teks `Jl. Dhoho No. 88` dan ganti sesuai lokasi aktual.

### Tambah/Ubah Menu
Cari array `menuData` di `<script>` tag dalam `index.html` dan edit datanya.

---

## 📜 Lisensi

© 2026 Lucky Cheese Kediri. All rights reserved.
