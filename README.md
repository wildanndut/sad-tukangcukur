# Sistem Aplikasi Tukang Cukur

Sistem aplikasi tukang cukur ini dibangun menggunakan PHP untuk backend dan JavaScript untuk frontend. Aplikasi ini dirancang untuk mempermudah manajemen jadwal, pencatatan pelanggan, serta sistem pembayaran untuk usaha tukang cukur.

## Deskripsi Proyek

Aplikasi ini memiliki berbagai fitur, antara lain:
- **Manajemen jadwal**: Menjadwalkan waktu cukur pelanggan.
- **Manajemen pelanggan**: Menyimpan data pelanggan seperti nama, nomor telepon, dan riwayat layanan.
- **Sistem pembayaran**: Mengelola transaksi dan tagihan cukur.
- **User authentication**: Fitur login untuk admin dan pegawai untuk mengakses sistem.

Proyek ini dikerjakan oleh tim sebagai bagian dari tugas kelompok di GitHub.

## Fitur

- **Jadwal Cukur**: Menjadwalkan waktu kunjungan tukang cukur dan menampilkan daftar antrian.
- **Manajemen Pelanggan**: Menambah, mengedit, dan menghapus data pelanggan.
- **Transaksi Pembayaran**: Mencatat transaksi pembayaran pelanggan setelah cukur.
- **Login dan Hak Akses**: Hanya admin yang dapat mengakses fitur tertentu (misalnya, pengaturan sistem, laporan).

## Teknologi yang Digunakan

- **PHP**: Sebagai bahasa pemrograman untuk backend dan pengolahan data.
- **JavaScript**: Untuk interaktivitas di sisi frontend.
- **HTML5 & CSS3**: Untuk tampilan antarmuka pengguna.
- **MySQL**: Sebagai database untuk menyimpan data pelanggan, jadwal, dan transaksi.
- **Bootstrap**: Untuk mendesain tampilan responsif.

## Instalasi

Untuk menjalankan aplikasi ini di komputer lokal Anda, ikuti langkah-langkah berikut:

### Persyaratan Sistem

- PHP 7.4 atau lebih tinggi
- Web server (Apache atau Nginx)
- MySQL atau MariaDB
- Composer (untuk manajemen dependensi PHP)
- Node.js dan npm (untuk mengelola dependensi frontend)

### Langkah-langkah Instalasi

1. **Clone repositori ini**:
    ```bash
    git clone https://github.com/username/repo-nama.git
    ```

2. **Masuk ke direktori proyek**:
    ```bash
    cd repo-nama
    ```

3. **Instal dependensi backend dengan Composer**:
    ```bash
    composer install
    ```

4. **Instal dependensi frontend dengan npm**:
    ```bash
    npm install
    ```

5. **Buat database MySQL** dan sesuaikan konfigurasi database di `config.php`:
    - Buat database baru di MySQL:
      ```sql
      CREATE DATABASE tukang_cukur;
      ```
    - Sesuaikan kredensial database di file `config.php`.

6. **Jalankan aplikasi**:
    - Pastikan Apache/Nginx berjalan dan dapat mengakses file index.php.
    - Akses aplikasi melalui browser di `http://localhost/[nama_proyek]`.

## Struktur Direktori

```bash
├── assets/              # File statis (gambar, CSS, JS)
├── config/              # File konfigurasi database dan aplikasi
├── controllers/         # File controller PHP
├── database/            # Skrip database dan migrasi
├── public/              # Folder public untuk file yang dapat diakses secara langsung
├── src/                 # Logika backend aplikasi
├── templates/           # Template frontend HTML
├── .gitignore           # File untuk mengecualikan file tertentu dari Git
├── composer.json        # Konfigurasi dependensi PHP
└── README.md            # Dokumentasi proyek
