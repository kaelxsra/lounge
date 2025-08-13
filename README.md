# Aplikasi Peminjaman Ruangan & Fasilitas (PHP)

Aplikasi ini digunakan untuk mengelola proses peminjaman ruangan dan fasilitas di sekolah, kampus, atau instansi. Dibangun menggunakan **PHP Native** dan **MySQL**, aplikasi ini memudahkan pengguna untuk melakukan pemesanan online serta membantu admin dalam mengelola data ruangan, fasilitas, dan peminjaman.

---

## 🚀 Fitur Utama
- ✅ **Login & Registrasi Pengguna**
- ✅ **Manajemen Ruangan** (Tambah, Edit, Hapus)
- ✅ **Manajemen Fasilitas**
- ✅ **Pemesanan/Peminjaman Ruangan**
- ✅ **Persetujuan Peminjaman oleh Admin**
- ✅ **Riwayat & Status Peminjaman**
- ✅ **Dashboard Admin**

---

## 🛠 Teknologi yang Digunakan
- **Bahasa Pemrograman**: PHP (7.x atau lebih baru)
- **Database**: MySQL
- **Frontend**: HTML5, CSS3, JavaScript, Bootstrap
- **Server**: Apache (XAMPP/Laragon)
- **Tools Pendukung**: phpMyAdmin

---

## 📂 Struktur Folder

```
/peminjaman-ruangan
│
├── /assets # CSS, JS, dan gambar
├── /config # File koneksi database
├── /pages # Halaman aplikasi (dashboard, login, dsb.)
├── /process # File proses CRUD dan logika peminjaman
├── index.php # Halaman awal (Landing Page)
└── README.md # Dokumentasi proyek
```

---

## ⚙️ Cara Instalasi
### 1. **Clone Repository**
```bash
git clone https://github.com/username/peminjaman-ruangan.git
cd peminjaman-ruangan

2. Konfigurasi Database
Buka phpMyAdmin

Buat database baru, misalnya peminjaman_db

Import file peminjaman.sql yang ada di folder /database

Edit file konfigurasi database config/koneksi.php:

<?php
$host = "localhost";
$user = "root";
$pass = "";
$db   = "peminjaman_db";

$conn = mysqli_connect($host, $user, $pass, $db);
if (!$conn) {
    die("Koneksi gagal: " . mysqli_connect_error());
}
?>

3. Jalankan Aplikasi
Pindahkan folder ke htdocs (jika pakai XAMPP)

Aktifkan Apache & MySQL di XAMPP

Akses melalui browser:

http://localhost/peminjaman-ruangan/

🔑 Akun Default
Admin

Username: admin

Password: admin123

User

Registrasi melalui halaman sign-up

🖼 Screenshot (Opsional)
Tambahkan gambar tampilan halaman login, dashboard admin, dan form peminjaman.

✅ Fitur yang Akan Dikembangkan
📅 Integrasi dengan kalender (FullCalendar)

📧 Notifikasi Email untuk persetujuan

🔒 Peningkatan Keamanan (CSRF, OTP)

📱 Desain Responsif untuk Mobile

📜 Lisensi
Proyek ini menggunakan lisensi MIT. Silakan gunakan dan kembangkan sesuai kebutuhan.
