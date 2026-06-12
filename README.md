# E-Library System - UAS Pemrograman Web 2

Repositori ini berisi sistem informasi pengelolaan data buku (E-Library) yang dikembangkan untuk memenuhi tugas akhir mata kuliah Pemrograman Web 2. Proyek ini menggunakan arsitektur **Decoupled** dengan pemisahan penuh antara *Backend API* dan *Frontend SPA*.

## 👤 Identitas Mahasiswa
* **Nama**: Fajar Fawwaz Atallah
* **NIM**: 312410357
* **Kelas**: TI.24.A4

## 🏗️ Struktur Proyek
* `backend-api/`: RESTful API Server dibangun dengan CodeIgniter 4, menerapkan fitur keamanan JWT (JSON Web Token).
* `frontend-spa/`: Frontend Single Page Application (SPA) dibangun dengan VueJS 3, TailwindCSS (Ultra-Modern UI), dan Axios untuk komunikasi API.

## 🖼️ Dokumentasi Visual & Pengujian

### 1. Skema Relasi Database
![Relasi Database](path/ke/screenshot_db.png)
*Lampiran: Visualisasi relasi tabel (users, kategori, buku) pada database.*

### 2. Uji Coba Keamanan API (Backend)
![Postman Error 401](path/ke/postman_error_401.png)
*Lampiran: Pengujian endpoint `POST` pada Postman tanpa token. Sistem berhasil memblokir akses dan mengembalikan status **401 Unauthorized** sebagai bukti `AuthFilter` bekerja dengan baik.*

### 3. Antarmuka Aplikasi (Frontend)
* **Halaman Login**: ![Login](path/ke/login.png)
* **Dashboard Admin**: ![Dashboard](path/ke/dashboard.png)
* **Tabel Data**: ![Tabel](path/ke/tabel.png)
*Antarmuka mengimplementasikan konsep Glassmorphism dan desain Ultra-Modern.*

## 🚀 Petunjuk Instalasi & Menjalankan

### Backend
1. Masuk ke folder `backend-api/`.
2. Salin file `.env` dan atur konfigurasi database serta `JWT_SECRET_KEY`.
3. Jalankan server lokal:
```bash
   php spark serve
