## Tech Stack

- PHP 8 
- MySQL / MariaDB , engine InnoDB
- HTML, CSS, dan JavaScript murni 


## Instalasi (XAMPP)

1. Pasang dan jalankan **XAMPP**, lalu aktifkan modul **Apache** dan **MySQL** pada XAMPP Control Panel.
2. Salin folder `kafe-pos` ke `C:\xampp\htdocs\` (hasilnya `C:\xampp\htdocs\kafe-pos (Ahmad Dhava Fahrezi)`).
3. Buka `http://localhost/phpmyadmin`, pilih tab **Import**, pilih file `database.sql`, lalu klik **Import**.
   Database `kafe_pos` beserta data awal akan dibuat otomatis.
4. Jika MySQL Anda memakai password atau port berbeda, sesuaikan `includes/config.php`
   (`DB_HOST`, `DB_NAME`, `DB_USER`, `DB_PASS`). Pengaturan bawaan XAMPP: user `root`, password kosong.
5. Buka `http://localhost/kafe-pos/` pada browser.

## Akun Uji Coba

| Role | Username | Password |
|---|---|---|
| Administrator / Manager | `admin` | `admin123` |
| Kasir / Waiter | `kasir1` | `kasir123` |
| Kasir / Waiter | `kasir2` | `kasir123` |

## Struktur Folder

```
kafe-pos/
|-- index.php, login.php, logout.php
|-- dashboard.php
|-- transaksi.php, struk.php, riwayat.php
|-- laporan.php, laporan_export.php
|-- produk.php, pengguna.php
|-- includes/       config, bootstrap (helper, sesi, CSRF, guard), header, footer, report
|-- assets/css/     style.css
|-- assets/js/      app.js, transaksi.js
|-- database.sql    skema 5 tabel + data awal
`-- README.md
