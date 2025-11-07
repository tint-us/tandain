PDF & Image Utility (Client-Side)

Aplikasi web sederhana untuk konversi file PDF ke format gambar (PNG/JPG) dan penambahan watermark pada file PDF maupun Gambar (PNG/JPG). Aplikasi ini dirancang untuk berjalan sepenuhnya di sisi klien (client-side) menggunakan JavaScript, sehingga tidak memerlukan server backend untuk pemrosesan file.

Fitur Utama

Konversi PDF: Konversi setiap halaman PDF menjadi file gambar (PNG) berkualitas tinggi.

Watermark PDF: Tambahkan teks watermark yang transparan dan berulang (diagonal) atau di tengah pada semua halaman PDF.

Watermark Gambar: Tambahkan teks watermark pada file gambar PNG atau JPG.

Input Fleksibel: Mendukung unggah, drag & drop, dan paste file langsung ke area kerja.

Teknologi yang Digunakan

Aplikasi ini menggunakan pustaka JavaScript pihak ketiga yang dimuat via CDN, menjadikannya sangat ringan dan mudah di-deploy:

Tailwind CSS: Untuk gaya dan desain yang responsif.

PDF.js: Untuk merender file PDF ke elemen Canvas (digunakan untuk konversi ke gambar).

PDF-lib: Untuk memodifikasi dan menambahkan watermark ke file PDF.

Struktur Proyek

Proyek ini hanya terdiri dari file-file berikut di direktori root:

/
|-- tool_konversi_watermark.html  <-- File utama aplikasi
|-- README.md                     <-- File panduan ini
|-- serve.json                    <-- File konfigurasi server lokal (BARU)


Menjalankan Secara Lokal

Anda dapat menjalankan aplikasi ini menggunakan server web lokal sederhana (seperti serve dari NPM) untuk memastikan semua fitur (terutama operasi file) berfungsi dengan benar.

1. Prasyarat

Pastikan Anda telah menginstal Node.js dan NPM.

2. Instalasi serve

serve adalah server statis ringan yang mudah digunakan:

npm install -g serve


3. Menjalankan Server

Dengan adanya file serve.json, serve akan secara otomatis menggunakan port yang telah Anda atur di sana (saat ini Port 8080).

Buka terminal di dalam direktori yang berisi tool_konversi_watermark.html dan serve.json.

Jalankan perintah berikut (tanpa argumen port):

serve .


Aplikasi akan tersedia di: http://localhost:8080.

Mengubah Port Default: Untuk mengubah port, cukup edit nilai "port" di dalam file serve.json.

Deployment ke GitHub Pages

Karena aplikasi ini client-side murni, deployment sangat mudah:

Buat Repositori: Buat repositori baru di GitHub (misalnya, pdf-image-utility).

Unggah File: Unggah ketiga file (tool_konversi_watermark.html, README.md, dan serve.json) ke repositori tersebut.

Atur GitHub Pages:

Buka Settings repositori Anda.

Pilih Pages di menu samping.

Pada bagian Source, pilih Deploy from a branch dan pastikan Branch diatur ke main (atau master) dan folder diatur ke /(root).

Klik Save.

GitHub Pages akan membutuhkan waktu beberapa menit untuk membangun dan menayangkan situs Anda. Aplikasi Anda akan tersedia di URL seperti: https://<username>.github.io/pdf-image-utility/tool_konversi_watermark.html
