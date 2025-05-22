# 💈 Sistem Informasi Manajemen Barbershop

Sistem ini dikembangkan sebagai proyek tugas mata kuliah **System Analysis and Design (SAD)** untuk mendukung digitalisasi layanan di barbershop (tukang cukur). Proyek ini menerapkan prinsip-prinsip analisis kebutuhan, perancangan sistem, pengembangan, dan pengujian perangkat lunak.

## 📚 Latar Belakang

Banyak barbershop yang masih menjalankan operasional secara manual, mulai dari pencatatan pelanggan hingga pengelolaan stok barang. Oleh karena itu, dibutuhkan sistem informasi yang dapat membantu mengotomatisasi proses tersebut dan meningkatkan efisiensi layanan.

## 🎯 Tujuan Sistem

- Menyediakan sistem manajemen layanan, pelanggan, dan stok barang secara terintegrasi
- Menerapkan algoritma penjadwalan untuk mengatur antrean layanan
- Menyediakan laporan harian/bulanan dalam bentuk digital dan cetak PDF
- Menerapkan pengujian sistem sesuai metode **Black Box** dan **White Box**

## ⚙️ Fitur Sistem

- ✅ **Login & Register**: Autentikasi admin dan pegawai
- ✂️ **Manajemen Layanan**: Tambah, ubah, hapus layanan cukur
- 📦 **Manajemen Barang**: Tambah, ubah, hapus stok barang
- 📅 **Sistem Antrian Otomatis**: Menggunakan algoritma **Shortest Job First (SJF)** dan **Priority Scheduling**
- 🧍‍♂️ **Pemesanan Layanan oleh Pelanggan**: Pelanggan dapat memilih layanan dan masuk ke antrean
- 📦 **Pemesanan Barang oleh Pelanggan**: Pelanggan dapat memesan produk (misalnya minyak rambut, pomade, dll)
- 🧑‍💼 **Penanganan Pesanan Layanan oleh Admin**: Admin memproses dan menyelesaikan pesanan layanan dari pelanggan
- 🧑‍💼 **Penanganan Pesanan Barang oleh Admin**: Admin memverifikasi dan menyelesaikan pesanan barang
- 📊 **Laporan Otomatis**:
  - Laporan layanan harian
  - Laporan barang bulanan
  - Laporan pendapatan
  - Laporan stok barang
- 🖨️ **Cetak PDF**: Semua laporan dapat diunduh dalam format PDF

## 🛠 Teknologi yang Digunakan

- **Frontend**: HTML, CSS, JavaScript, Bootstrap
- **Backend**: PHP
- **Database**: MySQL
- **PDF Generator**: TCPDF

## 📐 Proses Pengembangan (SAD)

- 📋 **Requirement Gathering**: Melalui observasi dan diskusi internal
- 📊 **Perancangan Sistem**: UML (Use Case, Activity, Class Diagram), ERD
- 🏗 **Implementasi**: Berdasarkan hasil perancangan dan dokumen kebutuhan
- 🧪 **Pengujian Sistem**:
  - **Black Box Testing**: Validasi input-output sistem
  - **White Box Testing**: Pengujian logika fungsi (login, register, cetak laporan, dll.)
- ✅ **Evaluasi & Dokumentasi**: Diuji oleh pengguna, divalidasi, dan dilaporkan

## 🚀 Instalasi

### Prasyarat

- PHP 7.4+
- Apache / Nginx
- MySQL / MariaDB
- Composer (opsional)
- Node.js & npm (jika diperlukan)

### Langkah Instalasi

1. Clone repositori:
    ```bash
    git clone https://github.com/username/barbershop-sad.git
    ```

2. Buat database:
    ```sql
    CREATE DATABASE barbershop;
    ```

3. Import file `barbershop.sql` ke database.

4. Konfigurasi koneksi database di `config/database.php`.

5. Jalankan server lokal dan akses aplikasi melalui:
    ```
    http://localhost/barbershop-sad/
    ```

## 📁 Struktur Direktori

```bash
├── assets/            # CSS, JS, gambar
├── config/            # Konfigurasi database
├── controllers/       # Logika backend
├── templates/         # Tampilan frontend
├── src/               # Fungsi sistem
├── database/          # SQL dan migrasi
├── .gitignore         # File ignore
├── README.md          # Dokumentasi proyek
