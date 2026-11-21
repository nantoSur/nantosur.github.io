# Portofolio UI

Web portofolio statis terinspirasi dari bahasa visual halaman Apple Music: tipografi besar, latar gelap, gradasi biru, kartu melayang, dan interaksi halus. Profil saat ini ditujukan untuk nanto — Senior VoIP Engineer — dengan produk di bawah brand NORZ.

## Struktur

```text
portfolio-ui/
├── index.html   # konten & struktur
├── styles.css   # styling, animasi, responsive
├── script.js    # menu, reveal, parallax, tilt, player demo
├── assets/
│   └── brands/  # logo brand (PNG dari Google Favicon + 3 monogram SVG)
├── robots.txt   # izin crawl & lokasi sitemap
├── sitemap.xml  # daftar URL untuk Google
└── README.md
```

## Menjalankan

Cukup buka `index.html` di browser. Proyek ini tidak memerlukan build dan tidak memakai dependensi eksternal.

Jika ingin menjalankannya lewat server lokal dan Python tersedia:

```bash
cd portfolio-ui
python -m http.server 8000
```

Lalu buka `http://localhost:8000`.

## Yang bisa diganti

- `nanto`, `surnanto.blogs@gmail.com`, WhatsApp `081315347158`, dan tautan sosial di `index.html`.
- Teks hero, deskripsi proyek, keahlian, dan timeline.
- Warna utama lewat variabel di bagian `:root` pada `styles.css` (saat ini palet biru terinspirasi kartu Northstar Dashboard).
- Ilustrasi kartu dibuat murni dengan CSS (tanpa gambar eksternal), jadi aman diganti dengan screenshot proyek asli.
- Logo brand ada di `assets/brands/`. `atcom.svg`, `witek.svg`, dan `escene.svg` sengaja dibuat monogram karena favicon resminya tidak ditemukan; ganti dengan file logo resmi jika tersedia.
- Bahasa Indonesia / English bisa diganti lewat tombol **ID / EN** di navigasi. Pilihan tersimpan di `localStorage`. Kamus terjemahan ada di bagian `translations` pada `script.js`.

## Agar masuk indeks Google

1. Pastikan repo `nantosur.github.io` public dan Pages aktif di branch `main` / `/(root)`.
2. Buka Google Search Console → **Add property** → pilih **URL prefix** → masukkan `https://nantosur.github.io/`.
3. Verifikasi kepemilikan dengan metode **HTML file** (letakkan file verifikasi di root repo) atau **HTML tag**.
4. Setelah terverifikasi, buka **Sitemaps** → masukkan `sitemap.xml` → **Submit**.
5. Buka **URL Inspection** → masukkan `https://nantosur.github.io/` → **Request indexing**.

`robots.txt`, `sitemap.xml`, canonical, meta description, dan data terstruktur `Person` sudah disiapkan di repo ini. Indexing biasanya memakan waktu beberapa hari sampai beberapa minggu.

File `google*.html` adalah file verifikasi Search Console. **Jangan dihapus** selama property masih aktif, atau verifikasi bisa dicabut.

## Catatan

Desain ini **terinspirasi** oleh Apple Music, bukan salinan aset atau identitas Apple.
