# SIPAMAS

SIPAMAS adalah aplikasi web pengaduan masyarakat berbasis Laravel yang digunakan untuk membantu masyarakat dalam membuat laporan, memantau status pengaduan, serta menerima tindak lanjut dari admin.

## Akun Login Admin

Gunakan akun berikut untuk login sebagai admin:

- Email: `redacted`
- Password: `redacted`

Halaman login:
- `/login`

## Fitur Utama

- Login dan registrasi pengguna
- Login admin
- Login dengan Google
- Login guest menggunakan nomor WhatsApp
- CRUD pengaduan masyarakat
- Upload bukti gambar
- Input lokasi manual atau GPS
- Dashboard admin
- Tindak lanjut laporan oleh admin
- Riwayat status pengaduan
- Chat antara admin dan user
- Notifikasi sistem
- Export data CSV
- Manajemen role user

## Teknologi yang Digunakan

- Laravel 10
- PHP 8.1 atau lebih baru
- MySQL / MariaDB
- Vite
- Tailwind CSS
- Laravel Socialite

## Cara Install Project

1. Download atau extract project SIPAMAS.
2. Buka terminal atau command prompt pada folder project.
3. Install dependency backend:

```bash
composer install
Install dependency frontend:
bash

npm install
Copy file environment:
bash

cp .env.example .env
Jika menggunakan Windows dan perintah cp tidak tersedia, salin manual file .env.example menjadi .env.

Generate application key:
bash

php artisan key:generate
Atur konfigurasi database pada file .env.
Contoh:

env

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=sipamas
DB_USERNAME=root
DB_PASSWORD=
Pastikan database sipamas sudah dibuat.
Jalankan migration:
bash

php artisan migrate
Jalankan seeder:
bash

php artisan db:seed
Jalankan frontend:
Untuk mode development:

bash

npm run dev
Untuk build production:

bash

npm run build
Jalankan server Laravel:
bash

php artisan serve
Buka aplikasi di browser:
bash

http://127.0.0.1:8000
Cara Login
Setelah aplikasi berjalan, masuk menggunakan akun admin berikut:

Email: redacted
Password: redacted
Struktur Fitur Penting
/login : halaman login
/register : halaman registrasi
/dashboard : dashboard utama
/complaints : daftar pengaduan
/complaints/create : tambah pengaduan
/notifications : daftar notifikasi
/admin/complaints : pengelolaan pengaduan admin
/admin/users : manajemen user
Catatan Penting
File .env tidak disertakan demi keamanan.
Folder vendor dan node_modules mungkin tidak ikut dalam paket ZIP, jadi harus di-install ulang.
Jika login Google digunakan, isi konfigurasi berikut pada .env:
GOOGLE_CLIENT_ID
GOOGLE_CLIENT_SECRET
GOOGLE_REDIRECT_URI
Deploy
Panduan deploy tersedia pada file berikut:

docs/INFINITYFREE.md
