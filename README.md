# Technical Assessment Yuda Satria
Technical Assessment untuk posisi Solution Analyst

Jawaban:
# 1. High-Level Design Architecture (gambar 1. Arsitektur)

Arsitektur untuk aplikasi mobile fintech PT. XYZ dapat dibagi menjadi tiga lapisan utama:

Presentation Layer: Bertanggung jawab untuk antarmuka pengguna (UI/UX) dan logika tampilan. Menggunakan teknologi seperti React Native atau Flutter untuk pengembangan aplikasi mobile lintas platform.

Application Layer: Ini adalah lapisan bisnis utama yang mengatur logika bisnis, termasuk proses peminjaman, autentikasi, dan pengelolaan data pengguna. Menggunakan bahasa pemrograman seperti Golang atau Node.js untuk backend.

Data Layer: Ini berhubungan dengan penyimpanan dan pengelolaan data, termasuk database pengguna, permohonan pinjaman, dan informasi lainnya. Database relasional seperti PostgreSQL atau MySQL bisa digunakan.

# 2. Screen Flow dan ERD (gambar 2. Screenflow dan 2. ERD)

Aplikasi ini akan memiliki beberapa layar utama:
Layar Registrasi: Pengguna memasukkan data diri, email, nomor telepon, dan mengunggah foto KTP.
Layar Login: Pengguna dapat masuk dengan email dan kata sandi atau autentikasi biometrik jika didukung.
Layar Dashboard: Menampilkan informasi sisa hutang dan tagihan per bulan jika ada.
Layar Peminjaman: Pengguna dapat mengajukan pinjaman dengan memasukkan jumlah dan tenor.
Layar Status Peminjaman: Pengguna dapat melihat status pinjaman saat ini (diterima atau ditolak).

# 3 Detail API dan Flowchart (gambar 3. Detail API & Flowchart)

Entity-Relationship Diagram (ERD):
Tabel Pengguna (User): ID, Nama, Email, Nomor Telepon, Kata Sandi, dll.
Tabel Peminjaman (Loan): ID, ID Pengguna, Jumlah, Tenor, Status, dll.

API Endpoints:
POST /api/register: Untuk registrasi pengguna.
POST /api/login: Untuk masuk.
GET /api/dashboard: Untuk mengambil informasi sisa hutang dan tagihan.
POST /api/loan: Untuk mengajukan pinjaman.
GET /api/loan/{loan_id}: Untuk mendapatkan status peminjaman tertentu.
POST /api/notifications/{loan_id}: Untuk mengirim notifikasi.

# 4 Detail untuk screen behavior

Berikut adalah detail screen behavior untuk aplikasi mobile PT. XYZ berdasarkan screen flow yang telah dijelaskan sebelumnya:

Layar Registrasi:
Pengguna memasukkan data diri, email, nomor telepon, dan mengunggah foto KTP.
Validasi input data (nama, email, nomor telepon, format foto KTP, dll.).
Mengirim data ke server untuk pendaftaran.
Jika berhasil, pengguna diarahkan ke layar masuk. Jika gagal, tampilkan pesan kesalahan.

Layar Login:
Pengguna memasukkan email dan kata sandi atau menggunakan autentikasi biometrik jika didukung.
Validasi input dan autentikasi pengguna.
Jika berhasil, pengguna diarahkan ke layar dashboard. Jika gagal, tampilkan pesan kesalahan.

Layar Dashboard:
Mengambil data sisa hutang dan tagihan per bulan dari server.
Menampilkan informasi sisa hutang dan tagihan per bulan kepada pengguna.
Tampilkan tombol untuk mengajukan pinjaman.

Layar Peminjaman:
Pengguna memasukkan jumlah peminjaman dan tenor.
Validasi jumlah peminjaman dan tenor (maksimal 12 juta dan 1 tahun).
Mengirim permohonan pinjaman ke server.
Menampilkan hasil permohonan (diterima atau ditolak).
Jika diterima, tampilkan notifikasi melalui email dan nomor telepon yang terdaftar.

Layar Status Peminjaman:
Mengambil status peminjaman dari server.
Menampilkan status peminjaman kepada pengguna (dalam proses, diterima, atau ditolak).

Pengguna dapat mengonfirmasi notifikasi melalui email atau nomor telepon yang terdaftar.
Dalam pemetaan screen behavior ini berguna memastikan bahwa setiap tindakan pengguna dikelola dengan baik, validasi data dilakukan secara ketat, dan respons yang jelas diberikan kepada pengguna.