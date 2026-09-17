# Builder Studio

Mockup UI untuk aplikasi website builder (drag & drop) bergaya split-view: panel kode di kiri, canvas preview di kanan.

## Isi File
- `index.html` — Halaman utama, sudah termasuk seluruh HTML, CSS, dan JavaScript dalam satu file (self-contained).

## Fitur yang Ditampilkan
- **Top Navbar**: logo brand, tools (Drag & Drop, Tombol, Menu, Fitur, Setting), pencarian, Undo/Redo, serta aksi Copy Code, Download .zip, dan Publish.
- **Editor Panel (kiri)**: tampilan kode HTML/CSS bergaya syntax-highlighted dengan tab file dan status bar.
- **Canvas Preview (kanan)**: pratinjau halaman hasil desain (hero section, kartu statistik, fitur) lengkap dengan pilihan device (Desktop/Tablet/Mobile).

## Cara Menggunakan
1. Ekstrak isi zip ini.
2. Buka `index.html` langsung di browser (double click, atau klik kanan → Open with browser).
3. Tidak perlu server atau instalasi tambahan — semua library dimuat dari CDN (Google Fonts, Font Awesome, JSZip, FileSaver.js).

## Tombol Interaktif
- **Copy Code**: menyalin kode editor ke clipboard.
- **Download .zip**: mengunduh `index.html` dalam bentuk file zip (`builder-studio-export.zip`) menggunakan JSZip & FileSaver.js.

## Dependensi (via CDN)
- [Google Fonts – Inter](https://fonts.google.com/specimen/Inter)
- [Font Awesome 6.4.0](https://fontawesome.com/)
- [JSZip 3.10.1](https://stuk.github.io/jszip/)
- [FileSaver.js 2.0.5](https://github.com/eligrey/FileSaver.js/)

## Catatan
Ini adalah tampilan statis (mockup) — tombol-tombol seperti Drag & Drop, Publish, dan navigasi editor belum terhubung ke fungsi backend apa pun. Bagian akhir file (canvas preview, features, dan script) dilengkapi agar dokumen HTML valid dan dapat dibuka langsung di browser.
