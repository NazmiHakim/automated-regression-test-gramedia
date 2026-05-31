# Gramedia Regression Testing Automation

Repositori ini berisi *Automated Regression Test Suite* untuk situs web [Gramedia.com](https://www.gramedia.com/), yang dikembangkan sebagai bagian dari Tugas Mata Kuliah Pengujian dan Penjaminan Kualitas Perangkat Lunak (PPKPL).

## 🚀 Deskripsi Proyek
Proyek ini mengotomatiskan 40 skenario pengujian (20 Positif dan 20 Negatif) untuk memverifikasi fungsionalitas utama dari platform Gramedia, termasuk:
- Fungsionalitas Login & Register
- Pencarian Produk (Buku, Penulis, Penerbit, ISBN)
- Interaksi Keranjang Belanja (Cart)
- Validasi Link Footer & Promo
- Penanganan input tidak valid dan skenario *error handling* (Skenario Negatif)

Script Python dikembangkan menggunakan **Selenium WebDriver** dan mengimplementasikan mekanisme tangguh untuk menangani *Dynamic DOM*, *Cookie Banners*, dan *Pop-up Overlays* khas aplikasi berbasis React (Next.js).

## 🛠️ Persyaratan (Prerequisites)
Pastikan Python 3.x telah terinstal di sistem Anda beserta Google Chrome versi terbaru.

1. Clone repositori ini.
2. Instal dependensi yang dibutuhkan:
```bash
pip install -r requirements.txt
```

## 🏃 Cara Menjalankan (How to Run)
Jalankan file utama melalui terminal:
```bash
python automation_test.py
```

Script akan secara otomatis membuka jendela Chrome, menjalankan 40 skenario secara berurutan dengan sesi yang saling terisolasi (`driver.delete_all_cookies()`), dan mencetak hasil pengujian (*Pass/Fail*) langsung di konsol.

## 📝 Dokumen Laporan
Rincian dokumen perancangan *Test Cases*, tahapan *Pre-Condition*, langkah uji, hingga *Expected/Actual Results* dapat dilihat pada berkas laporan PDF/Word yang terlampir di repositori ini.
