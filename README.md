Aplikasi Peminjaman Ruangan & Fasilitas (PHP)
Aplikasi ini dibuat untuk mengelola proses peminjaman ruangan dan fasilitas di sekolah, kampus, atau instansi menggunakan teknologi PHP. Pengguna dapat melihat ketersediaan ruangan, melakukan peminjaman, dan admin dapat mengelola data serta menyetujui permintaan.

Fitur Utama
✅ Autentikasi Pengguna: Login, registrasi, dan manajemen akun.

✅ Manajemen Ruangan: Tambah, edit, dan hapus data ruangan.

✅ Manajemen Fasilitas: Kelola fasilitas tambahan untuk peminjaman.

✅ Peminjaman Online: Pengguna dapat memesan ruangan dengan jadwal tertentu.

✅ Persetujuan Admin: Admin dapat menyetujui atau menolak peminjaman.

✅ Riwayat Peminjaman: Lihat status pemesanan dan histori.

✅ Dashboard Admin: Statistik dan manajemen data.

Teknologi yang Digunakan
Bahasa Pemrograman: PHP (versi 7.4+)

Database: MySQL/MariaDB

Frontend: HTML5, CSS3, JavaScript (Bootstrap untuk UI)

Server: Apache (XAMPP/Laragon)

Tools: Composer (jika menggunakan Laravel), VS Code, phpMyAdmin

Struktur Proyek
Jika tanpa framework:

bash
Salin
Edit
/peminjaman-ruangan
│
├── /assets         # CSS, JS, gambar
├── /config         # Koneksi database
├── /pages          # Halaman utama (dashboard, login, dsb.)
├── /process        # File proses (CRUD, login, peminjaman)
├── index.php       # Halaman awal
└── README.md
Jika dengan Laravel:

bash
Salin
Edit
/peminjaman-ruangan
│
├── /app
├── /database
├── /public
├── /resources
├── /routes
├── .env
└── README.md
Instalasi & Konfigurasi
1. Clone Repository
bash
Salin
Edit
git clone https://github.com/username/peminjaman-ruangan.git
cd peminjaman-ruangan
2. Konfigurasi Database
Buat database di MySQL, misal peminjaman_db.

Import file SQL yang ada di folder /database atau peminjaman.sql.

Sesuaikan pengaturan database di file config.php (atau .env jika Laravel):

ini
Salin
Edit
DB_HOST=localhost
DB_USER=root
DB_PASS=
DB_NAME=peminjaman_db
3. Jalankan di Localhost
Jika pakai XAMPP:

Taruh folder proyek di htdocs

Jalankan Apache & MySQL di XAMPP

Akses via browser:

arduino
Salin
Edit
http://localhost/peminjaman-ruangan/
Jika pakai Laravel:

bash
Salin
Edit
composer install
php artisan key:generate
php artisan migrate --seed
php artisan serve
Lalu akses:

cpp
Salin
Edit
http://127.0.0.1:8000
Akun Default
Admin

Email: admin@mail.com

Password: admin123

User

Registrasi melalui halaman sign-up

Screenshot (Opsional)
[Tambahkan gambar tampilan dashboard, halaman login, dsb.]

Fitur yang Akan Dikembangkan
📅 Integrasi dengan kalender (FullCalendar)

📧 Notifikasi email saat peminjaman disetujui

📱 Desain responsif untuk mobile

🔐 Peningkatan keamanan (CSRF, OTP)

Lisensi
Proyek ini menggunakan lisensi MIT – bebas digunakan dan dikembangkan.
