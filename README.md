# Technical Assessment Yuda Satria
Technical Assessment for Solution Analyst posision

Jawaban
# 1. High-Level Design Architecture (gambar 1. Arsitektur)

Arsitektur untuk aplikasi mobile fintech PT. XYZ dapat dibagi menjadi tiga lapisan utama:

Presentation Layer: Bertanggung jawab untuk antarmuka pengguna (UI/UX) dan logika tampilan. Menggunakan teknologi seperti React Native atau Flutter untuk pengembangan aplikasi mobile lintas platform.

Application Layer: Ini adalah lapisan bisnis utama yang mengatur logika bisnis, termasuk proses peminjaman, autentikasi, dan pengelolaan data pengguna. Menggunakan bahasa pemrograman seperti Golang atau Node.js untuk backend.

Data Layer: Ini berhubungan dengan penyimpanan dan pengelolaan data, termasuk database pengguna, permohonan pinjaman, dan informasi lainnya. Database relasional seperti PostgreSQL atau MySQL bisa digunakan.

# 2. Screen Flow dan ERD (gambar 2. Screenflow dan 2. ERD)

Aplikasi ini akan memiliki beberapa layar utama:
Layar Registrasi: Pengguna memasukkan data diri, email, nomor telepon, dan mengunggah foto KTP.
Layar Login: Pengguna dapat masuk dengan username dan kata sandi atau autentikasi biometrik jika didukung.
Layar Dashboard: Menampilkan informasi sisa hutang dan tagihan per bulan jika ada.
Layar Peminjaman: Pengguna dapat mengajukan pinjaman dengan memasukkan jumlah dan tenor.
Layar Status Peminjaman: Pengguna dapat melihat status pinjaman saat ini (diterima atau ditolak).
