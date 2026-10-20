<div align="center">

# 💬 Laravel Chat Application

**Eksplorasi aplikasi pesan berbasis Laravel 10 dan Chatify.**

[![Laravel](https://img.shields.io/badge/Laravel-10-FF2D20?logo=laravel&logoColor=white)](https://laravel.com/)
[![PHP](https://img.shields.io/badge/PHP-%5E8.1-777BB4?logo=php&logoColor=white)](https://www.php.net/)
[![Chatify](https://img.shields.io/badge/Package-Chatify-blue)](https://github.com/munafio/chatify)

</div>

## 📖 Tentang Proyek

Repositori ini merupakan proyek eksperimen untuk membangun aplikasi percakapan menggunakan **Laravel 10**, dengan integrasi paket **Chatify**. Cocok sebagai referensi pembelajaran mengenai autentikasi aplikasi web dan integrasi komponen pesan ke dalam ekosistem Laravel.

## 🧩 Teknologi dan Dependensi

Berdasarkan file konfigurasi proyek:

- Laravel `^10.10`
- PHP `^8.1`
- Chatify `^1.6`
- Laravel Sanctum
- Laravel Breeze (dependensi pengembangan)
- Tailwind CSS
- Vite
- Pest (framework testing)

> Penggunaan paket di atas terverifikasi dari file dependensi. Fitur Chatify tertentu, konfigurasi real-time, dan status pengujiannya perlu dicek langsung saat aplikasi dijalankan.

## 📁 Struktur Proyek

```text
chat/
├── app/             # Logika aplikasi Laravel
├── bootstrap/       # Bootstrap framework
├── config/          # Konfigurasi aplikasi
├── database/        # Migration dan seeder
├── public/          # Aset publik
├── resources/       # Views dan aset frontend
├── routes/          # Definisi route
├── storage/         # Penyimpanan aplikasi
├── tests/           # Pengujian
├── composer.json    # Dependensi PHP
├── package.json     # Dependensi frontend
└── .env.example     # Template konfigurasi
```

## 🚀 Instalasi Lokal

### Persyaratan

- PHP 8.1 atau lebih baru (sesuai constraint Composer)
- Composer
- Node.js dan npm
- Database yang kompatibel dengan konfigurasi Laravel

### Langkah

```bash
git clone https://github.com/freyy4/chat.git
cd chat
composer install
cp .env.example .env
php artisan key:generate
npm install
```

Sesuaikan pengaturan database dalam `.env` dan buat database lokal terlebih dahulu. Kemudian:

```bash
php artisan migrate
npm run dev
```

Jalankan Laravel di terminal lain:

```bash
php artisan serve
```

Akses aplikasi melalui `http://127.0.0.1:8000`.

> Jika Chatify memerlukan publikasi aset atau konfigurasi tambahan, ikuti petunjuk paket sesuai versi yang tercatat di `composer.lock`.

## 📸 Screenshot

Tempatkan tangkapan layar yang telah disanitasi pada `docs/screenshots/` untuk memperlihatkan halaman autentikasi dan antarmuka chat.

## 🎯 Tujuan Pembelajaran

- Menerapkan struktur MVC dengan Laravel.
- Mengintegrasikan paket pihak ketiga melalui Composer.
- Memahami alur autentikasi dan pengelolaan data percakapan.
- Mempersiapkan aplikasi untuk pengembangan dan pengujian lanjutan.

## 🔐 Keamanan

Jangan commit file `.env`, token layanan, database pengguna, atau percakapan pribadi. Gunakan data dummy untuk screenshot dan demonstrasi.

## 👨‍💻 Developer

**Farid Syifa Arrahim** — [@freyy4](https://github.com/freyy4)

---

*Personal learning project — Laravel ecosystem and messaging integration.*
