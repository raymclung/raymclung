## Ray McLung

Mahasiswa, sekaligus developer paruh waktu. Hampir semua yang saya bangun berhubungan
dengan catur — bukan karena direncanakan, tapi karena dari sanalah tugas-tugas pertama
saya datang.

Saya cenderung memulai tanpa framework. Bukan karena anti, tapi karena ingin tahu dulu
apa yang sebenarnya terjadi sebelum menyerahkannya ke pustaka orang lain. Belakangan
sedang belajar C dan Python.

### Yang sedang dan pernah saya kerjakan

**[wa-bot-grup-catur](https://github.com/raymclung/wa-bot-grup-catur)** — Bot moderasi
grup WhatsApp untuk komunitas catur, berjalan sejak Juni 2026.

Bagian yang paling banyak mengajari saya justru bukan kodenya, melainkan WhatsApp itu
sendiri. Bot ini pernah kena blokir 403 karena mengirim terlalu banyak pesan, jadi saya
tambahkan batas 50 pesan per jam, ubah jawaban puzzle dari gambar papan menjadi teks,
dan buat jeda sambung-ulang yang makin lama makin panjang. Ada juga mode "capek" dan jam
tenang pukul 1–5 pagi.

Arsitekturnya dipisah: `gateway` (Node.js) hanya mengurus koneksi, `brain` (C# .NET 10)
memegang seluruh logika. Dengan begitu aturan moderasi bisa diuji tanpa perlu terhubung
ke WhatsApp sama sekali.

**[RubyRa Stays](https://github.com/raymclung/RubyRa)** ·
[demo](https://raymclung.github.io/RubyRa/) — Prototipe pemesanan penginapan. Tiga belas
layar dalam satu berkas HTML, tanpa dependensi.

Versi pertamanya berukuran 31,6 MB karena semua gambar saya tanam sebagai base64 — satu
barisnya saja 25 MB, dan GitHub menolaknya saat diunggah. Setelah gambarnya dikeluarkan
jadi berkas terpisah lalu dikompres, tinggal 2,7 MB.

**[PesanAja](https://github.com/raymclung/Pesan-Aja)** ·
[demo](https://raymclung.github.io/Pesan-Aja/) — Prototipe aplikasi pemesanan layanan
seperti salon dan laundry. Dua puluh halaman, mobile-first, bisa dipasang sebagai PWA.
Ini tugas kuliah, dan masih ada CSS yang tercecer di sana-sini yang belum sempat saya
rapikan.

**[PGN to Puzzle](https://github.com/raymclung/PGN-to-puzzles-Chess)** — Alat baris
perintah yang membaca partai catur, mencari langkah yang mengubah posisi seimbang menjadi
kalah, lalu menjadikannya puzzle.

Bagian yang paling lama saya pikirkan adalah cara menentukan tingkat kesulitan. Awalnya
saya pakai panjang solusi, tapi itu keliru — rangkaian panjang berisi langkah-langkah
gamblang tetap mudah, sementara satu langkah tenang yang brilian tetap sulit. Akhirnya
levelnya ditentukan oleh ayunan evaluasi dan penanda seperti pengorbanan.

### Perkakas

JavaScript · HTML · CSS · Python · C# · C · Git

### Kontak

[LinkedIn](https://www.linkedin.com/in/raymclunggunawan/) ·
[raymclung@gmail.com](mailto:raymclung@gmail.com)

Terbuka untuk magang dan proyek lepas.
