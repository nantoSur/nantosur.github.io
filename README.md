# Portofolio UI

Web portofolio statis terinspirasi dari bahasa visual halaman Apple Music: tipografi besar, latar gelap, gradasi biru, kartu melayang, dan interaksi halus. Profil saat ini ditujukan untuk nanto — Senior VoIP Engineer — dengan produk di bawah brand NORZ.

## Struktur

```text
portfolio-ui/
├── index.html   # konten & struktur
├── styles.css   # styling, animasi, responsive
├── script.js    # menu, reveal, parallax, tilt, player demo
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
- Bahasa Indonesia / English bisa diganti lewat tombol **ID / EN** di navigasi. Pilihan tersimpan di `localStorage`. Kamus terjemahan ada di bagian `translations` pada `script.js`.

## Catatan

Desain ini **terinspirasi** oleh Apple Music, bukan salinan aset atau identitas Apple.
