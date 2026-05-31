# Laporan Skenario Pengujian (Test Cases) - Gramedia.com

## Skenario Positif (20 Test Cases)

| No | Test Scenario | TestCase_ID | Test Case Description | Pre-Condition | Test Case Step | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|---|---|---|
| 1 | Verifikasi Title Homepage | TC-POS-01 | Memastikan title halaman beranda benar | URL Gramedia diakses | 1. Buka URL website<br>2. Cek `<title>` halaman | Title mengandung kata "Gramedia" | Title memuat kata "Gramedia" | **Pass** |
| 2 | Pencarian Buku Valid | TC-POS-02 | Mencari judul buku yang spesifik ("Laskar Pelangi") | Berada di Homepage | 1. Input "Laskar Pelangi" di search bar<br>2. Tekan Enter | Menampilkan hasil pencarian buku Laskar Pelangi | Muncul daftar buku Laskar Pelangi | **Pass** |
| 3 | Pencarian Penulis | TC-POS-03 | Mencari nama penulis spesifik ("Tere Liye") | Berada di Homepage | 1. Input "Tere Liye" di search bar<br>2. Tekan Enter | Menampilkan buku karya Tere Liye | Muncul buku karya Tere Liye | **Pass** |
| 4 | Klik Dropdown Kategori | TC-POS-04 | Mengecek apakah menu kategori bisa diklik/dibuka | Berada di Homepage | 1. Klik menu Kategori di header | Dropdown menu kategori muncul | Dropdown menu kategori muncul | **Pass** |
| 5 | Scroll ke Footer | TC-POS-05 | Memastikan fungsi scroll ke bagian paling bawah (footer) berjalan | Halaman terload sempurna | 1. Scroll halaman ke paling bawah | Bagian footer website terlihat | Footer terlihat dengan benar | **Pass** |
| 6 | Verifikasi Link 'Tentang Kami' | TC-POS-06 | Mengecek keberadaan dan validitas URL 'Tentang Kami' | Berada di Footer | 1. Cari tautan 'Tentang Kami'<br>2. Periksa atribut href | Tautan 'Tentang Kami' memiliki URL yang valid | Tautan memiliki URL yang valid | **Pass** |
| 7 | Verifikasi Link 'Bantuan' | TC-POS-07 | Mengecek tautan 'Bantuan' atau 'FAQ' di footer | Berada di Footer | 1. Cari tautan 'Bantuan' | Tautan 'Bantuan' memiliki URL yang valid | Tautan memiliki URL yang valid | **Pass** |
| 8 | Navigasi Login | TC-POS-08 | Berpindah ke halaman Login (Masuk) | Berada di Homepage | 1. Klik tombol 'Masuk' di kanan atas | Sistem mengarahkan ke form /login | Sistem mengarahkan ke form /login | **Pass** |
| 9 | Navigasi Register | TC-POS-09 | Berpindah ke halaman Register (Daftar) | Berada di Homepage | 1. Klik tombol 'Daftar' | Sistem mengarahkan ke form /register | Sistem mengarahkan ke form /register | **Pass** |
| 10 | Klik Logo Home | TC-POS-10 | Memastikan klik logo Gramedia mengembalikan ke beranda | Berada di halaman kategori | 1. Klik logo Gramedia di header | Sistem meredirect ke Homepage awal | Sistem meredirect ke Homepage | **Pass** |
| 11 | Detail Produk | TC-POS-11 | Masuk ke halaman rincian produk | Hasil pencarian/Homepage terload | 1. Klik salah satu cover/judul produk | Masuk ke halaman detail produk tersebut | Masuk ke detail produk sukses | **Pass** |
| 12 | Tombol Keranjang | TC-POS-12 | Verifikasi adanya tombol 'Keranjang'/'Beli' di detail produk | Berada di detail produk | 1. Cari elemen tombol "Beli" atau "Keranjang" | Tombol beli/keranjang terlihat | Tombol beli/keranjang terlihat | **Pass** |
| 13 | Buka Halaman Keranjang | TC-POS-13 | Masuk ke halaman keranjang belanja | Berada di Homepage | 1. Klik icon keranjang di header | Diarahkan ke halaman /cart | Diarahkan ke halaman /cart | **Pass** |
| 14 | Pencarian Penerbit | TC-POS-14 | Mencari buku berdasarkan penerbit | Berada di Homepage | 1. Input "Gramedia Pustaka Utama"<br>2. Tekan Enter | Menampilkan list buku dari GPU | Menampilkan buku penerbit terkait | **Pass** |
| 15 | Pencarian ISBN | TC-POS-15 | Menggunakan kode ISBN untuk mencari buku | Berada di Homepage | 1. Input nomor ISBN<br>2. Tekan Enter | Menampilkan spesifik 1 buku yang relevan | Menampilkan buku sesuai ISBN | **Pass** |
| 16 | Link Sosial Media | TC-POS-16 | Memastikan link medsos (FB/IG) ada di footer | Berada di Footer | 1. Cek icon Facebook/Instagram | Terdapat elemen icon dengan link yang valid | Ditemukan link socmed (Facebook/IG) | **Pass** |
| 17 | Logo Pembayaran | TC-POS-17 | Mengecek ikon bank/metode pembayaran | Berada di Footer | 1. Lihat bagian daftar metode pembayaran | Terdapat logo/text metode pembayaran | Logo/Text pembayaran ditemukan | **Pass** |
| 18 | Halaman Promo | TC-POS-18 | Mengakses daftar promo aktif | Berada di Homepage | 1. Klik menu "Promo" di header | Dialihkan ke halaman kumpulan promo | Dialihkan ke halaman kumpulan promo | **Pass** |
| 19 | Section Buku Terbaru | TC-POS-19 | Memeriksa adanya *section* buku terbaru/rekomendasi | Berada di Homepage | 1. Cek judul section "Buku Terbaru" | Section tersebut muncul (visible) | Section tersebut muncul (visible) | **Pass** |
| 20 | Banner Mobile App | TC-POS-20 | Memastikan link download aplikasi seluler tersedia | Berada di Homepage | 1. Cari tautan Google Play / App Store | Tautan atau icon store muncul di web | Icon toko aplikasi tersedia | **Pass** |

<br>

## Skenario Negatif (20 Test Cases)

| No | Test Scenario | TestCase_ID | Test Case Description | Pre-Condition | Test Case Step | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|---|---|---|
| 1 | Pencarian Karakter Invalid | TC-NEG-01 | Input karakter aneh di search bar (`@#$%`) | Berada di Homepage | 1. Input karakter invalid<br>2. Tekan Enter | Menampilkan teks "Tidak ditemukan" (0 hasil) | Muncul pesan "Tidak ditemukan" | **Pass** |
| 2 | Pencarian Kosong | TC-NEG-02 | Submit form pencarian tanpa isi apa-apa | Berada di Homepage | 1. Kosongkan search bar<br>2. Tekan Enter | Sistem mengabaikan / URL tetap (bukan form kosong) | URL tetap di homepage (Pencarian diabaikan) | **Pass** |
| 3 | Login Kosong | TC-NEG-03 | Menekan tombol masuk tanpa mengisi email/password | Halaman Login terbuka | 1. Kosongkan email & password<br>2. Klik 'Masuk' | Muncul peringatan form required (tidak bisa disubmit) | Muncul peringatan form required | **Pass** |
| 4 | Format Email Salah (Login) | TC-NEG-04 | Login menggunakan email tanpa '@' atau domain | Halaman Login terbuka | 1. Input "email_tanpa_domain"<br>2. Klik 'Masuk' | Muncul error format email tidak sesuai | Muncul error format email | **Pass** |
| 5 | Email Tidak Terdaftar | TC-NEG-05 | Login menggunakan email yang tidak ada di DB | Halaman Login terbuka | 1. Input email acak baru<br>2. Klik 'Masuk' | Muncul error "Akun belum terdaftar/Email salah" | Muncul error validasi | **Pass** |
| 6 | Password Salah | TC-NEG-06 | Login menggunakan email valid namun password salah | Halaman Login terbuka | 1. Input email benar<br>2. Input password acak | Muncul error "Password yang dimasukkan salah" | Muncul error validasi | **Pass** |
| 7 | Register Form Kosong | TC-NEG-07 | Klik daftar tanpa mengisi apapun | Halaman Register terbuka | 1. Biarkan form kosong<br>2. Klik 'Daftar' | Sistem memunculkan validasi error tiap kolom wajib | Validasi error tiap kolom wajib muncul | **Pass** |
| 8 | Register Email Invalid | TC-NEG-08 | Daftar menggunakan format email yang salah | Halaman Register terbuka | 1. Isi form lain benar<br>2. Email = "bukanemail" | Form divalidasi gagal, registrasi ditolak | Gagal karena format email tidak diizinkan | **Pass** |
| 9 | Password Terlalu Pendek | TC-NEG-09 | Mendaftar dengan password 3 karakter | Halaman Register terbuka | 1. Input password "123"<br>2. Klik 'Daftar' | Terdapat error validasi minimum karakter | Password ditolak karena terlalu pendek | **Pass** |
| 10 | Konfirmasi Pass Salah | TC-NEG-10 | Menulis konfirmasi password yang tidak cocok | Halaman Register terbuka | 1. Pass: "Satu123!"<br>2. Konfirmasi: "Dua321!" | Error "Konfirmasi password tidak cocok" muncul | Peringatan validasi ketidakcocokan muncul | **Pass** |
| 11 | Promo Kosong | TC-NEG-11 | Menerapkan kode promo kosong di keranjang | Berada di halaman Keranjang | 1. Kosongkan kolom promo<br>2. Klik Apply | Tombol disabled / error field required | Mencegah submit form promo kosong | **Pass** |
| 12 | Promo Invalid | TC-NEG-12 | Menggunakan kode "INVALID123" | Berada di halaman Keranjang | 1. Ketik promo "INVALID123"<br>2. Klik Apply | Error "Promo tidak ditemukan / Tidak berlaku" | Error validasi kode promo tampil | **Pass** |
| 13 | Checkout Keranjang Kosong| TC-NEG-13 | Mencoba lanjut ke pembayaran tanpa barang | Berada di halaman Keranjang | 1. Pastikan keranjang kosong<br>2. Cek tombol Lanjut | Tombol Checkout seharusnya *disabled* / tidak ada | Tombol checkout terkunci / dinonaktifkan | **Pass** |
| 14 | Kuantitas Negatif | TC-NEG-14 | Menginputkan angka kuantitas negatif (jika bisa) | Terdapat barang di keranjang | 1. Ganti value qty jadi -1 | Value direset otomatis ke 1 / dicegah | Sistem tidak mengizinkan input negatif | **Pass** |
| 15 | Akses Profile Terkunci | TC-NEG-15 | Membuka URL /profile langsung tanpa login | Belum login, tab kosong | 1. Buka `gramedia.com/profile` | Dialihkan otomatis secara paksa ke `/login` | Dialihkan otomatis ke /login | **Pass** |
| 16 | Lupa Password Kosong | TC-NEG-16 | Mengajukan lupa sandi dengan email kosong | Halaman Lupa Sandi terbuka | 1. Biarkan kolom kosong<br>2. Klik 'Kirim' | Menampilkan validasi field tidak boleh kosong | Muncul validasi field wajib diisi | **Pass** |
| 17 | Lupa Password Invalid | TC-NEG-17 | Mengajukan lupa sandi dengan format tak valid | Halaman Lupa Sandi terbuka | 1. Isi email "abcde"<br>2. Klik 'Kirim' | Menampilkan pesan error format email tidak valid | Form menolak disubmit (format email salah) | **Pass** |
| 18 | Pencarian Super Panjang | TC-NEG-18 | Mengisi bar pencarian dengan > 255 karakter huruf | Berada di Homepage | 1. Ketik "A" sebanyak 300x<br>2. Tekan Enter | Sistem membatasi input atau menampilkan "0 Hasil" | Menampilkan peringatan / 0 hasil penelusuran | **Pass** |
| 19 | Newsletter Kosong | TC-NEG-19 | Berlangganan info (*subscribe*) dengan field kosong | Berada di bagian Footer | 1. Kosongkan form langganan<br>2. Klik Subscribe | Validasi required muncul | Validasi isian wajib email muncul | **Pass** |
| 20 | Newsletter Email Salah | TC-NEG-20 | Mendaftarkan langganan newsletter dengan asal | Berada di bagian Footer | 1. Isi teks asal tanpa `@`<br>2. Klik Subscribe | Validasi email requirement gagal / pesan error | Sistem memblokir email dengan format asal | **Pass** |
