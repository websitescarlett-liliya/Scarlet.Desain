# Website Builder - Tempel Desain

Website builder sederhana dengan sistem tempel komponen. Panel kiri menampilkan source code, panel kanan menampilkan hasil desain secara langsung.

## Fitur

- Tambah komponen dengan satu klik: Tombol, Menu, Fitur
- Preview desain real-time di panel kanan
- Panel pengaturan untuk setiap elemen terpilih
- Ubah warna background dan warna teks
- Salin code HTML hasil desain dengan satu klik
- Hapus elemen yang tidak dibutuhkan (klik dua kali)
- Tampilan hitam putih, teks hitam background putih

## Struktur Proyek

```
project/
├── builder.html      # File utama aplikasi builder
├── README.md         # Dokumentasi proyek
└── assets/           # Folder opsional untuk gambar dan file tambahan
```

## Cara Instalasi

1. Download atau clone repositori ini
2. Tidak membutuhkan instalasi tambahan
3. Tidak membutuhkan server atau database

## Cara Penggunaan

1. Buka file `builder.html` di browser
2. Klik tombol di header untuk menambah komponen:
   - Tambah Tombol: membuat button baru
   - Tambah Menu: membuat navigasi baru
   - Tambah Fitur: membuat card fitur baru
   - Tambah Teks: membuat teks yang bisa diedit langsung
3. Klik dua kali pada elemen di canvas untuk menghapusnya
4. Atur melalui panel pengaturan di bawah canvas:
   - Warna Background
   - Warna Teks
5. Klik tombol Salin Code untuk menyalin HTML hasil desain
6. Tempel code tersebut ke website yang dibutuhkan

## Teknologi

- HTML5 untuk struktur
- CSS3 untuk styling, tanpa framework
- JavaScript murni, tanpa library tambahan

## Kustomisasi

Untuk menambah jenis komponen baru, edit fungsi `addEl()` di dalam file `builder.html`:

```javascript
if (type === 'nama-baru') {
  el = document.createElement('div');
  el.innerHTML = '<p>Komponen baru</p>';
}
```

Kemudian tambahkan tombol baru di bagian toolbar:

```html
<button class="tool" onclick="addEl('nama-baru')">+ Nama Baru</button>
```

## Catatan

- Code yang disalin hanya berisi HTML hasil desain di dalam canvas
- CSS dasar perlu disesuaikan dengan website tujuan
- Klik dua kali pada elemen untuk menghapusnya langsung dari canvas
- Semua perubahan tersimpan hanya selama browser terbuka

## Lisensi

Bebas digunakan untuk keperluan pribadi dan komersial.
