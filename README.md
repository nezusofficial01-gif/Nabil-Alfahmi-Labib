[README.md](https://github.com/user-attachments/files/34062877/README.md)
# Portfolio — Nabil Alfahmi Labib

Website portfolio Industrial Engineering / Manufacturing / Continuous Improvement.
Dibuat dengan HTML, CSS, dan JavaScript murni (tanpa framework, tanpa build tool), sehingga bisa langsung dipublikasikan di GitHub Pages.

## Struktur File

```
.
├── index.html      # Seluruh website (HTML + CSS + JS)
├── README.md       # Dokumen ini
└── assets/         # Gambar proyek (buat folder ini sendiri)
    ├── 01-layout.jpg
    ├── 02-dashboard.jpg
    ├── 03-vsm.jpg
    ├── 04-equipment.jpg
    └── 05-warehouse.jpg
```

## Menjalankan Secara Lokal

Buka `index.html` langsung di browser. Tidak perlu instalasi apa pun.
Font dimuat dari Google Fonts, jadi diperlukan koneksi internet untuk tampilan font yang sesuai.

## Deploy ke GitHub Pages

1. Buat repository baru di GitHub (misalnya `portfolio`).
2. Upload `index.html`, `README.md`, dan folder `assets/`.
3. Buka **Settings → Pages**.
4. Pada **Build and deployment**, pilih **Deploy from a branch**, Branch `main`, folder `/ (root)`, lalu **Save**.
5. Tunggu 1–2 menit. Website tayang di `https://USERNAME.github.io/NAMA-REPO/`.

Untuk memperbarui website, edit file lalu commit. GitHub Pages akan memperbarui otomatis.

## Mengganti Konten

### Teks proyek

Buka `index.html`, cari `const P=[` di dalam tag `<script>`. Setiap proyek berisi:

| Field | Fungsi |
|---|---|
| `no` | Nomor proyek |
| `t` | Judul proyek |
| `cat` | Kategori |
| `st` | Label status yang tampil |
| `k` | Jenis untuk filter: `work`, `team`, atau `academic` |
| `d` | Deskripsi singkat di kartu |
| `r` | Peran singkat di kartu |
| `img` | Path gambar |
| `s` | Isi case study (per bagian) |

Pada `s`, bagian yang bernilai `null` akan menampilkan placeholder. Isi dengan teks (string) atau daftar (array) bila datanya sudah ada. Bagian yang tidak ada di `s` tidak akan ditampilkan.

### Teks lain

Hero, About, Experience, Skills, dan Contact ditulis langsung sebagai HTML biasa di bagian `<main>`. Cari teksnya dan edit.

### Warna

Semua warna ada di `:root` pada bagian `<style>`: `--blue` (#155687), `--ink`, `--mute`, `--tint`, `--line`.

## Menambahkan Gambar Proyek

1. Buat folder `assets/` di samping `index.html`.
2. Simpan gambar dengan nama sesuai nilai `img` pada data proyek (misalnya `assets/01-layout.jpg`).
3. Selama file belum ada, website otomatis menampilkan placeholder.

Saran: gunakan JPG atau WebP, rasio 16:9, lebar sekitar 1200 px, dan ukuran di bawah 300 KB per gambar.

## Kerahasiaan Dokumen

Dokumen manufaktur dapat memuat informasi rahasia. Sebelum mengunggah gambar:

- Hapus atau blur nama pelanggan, nama perusahaan, kode part, dan data produksi internal.
- Sensor detail fasilitas dan drawing yang bersifat proprietary.
- Pastikan Anda berwenang mempublikasikan setiap gambar.

Nama perusahaan di halaman Experience saat ini sengaja ditulis netral. Ganti hanya jika sudah diizinkan.

## Checklist Sebelum Publikasi

- [ ] Link CV Google Drive terbuka dan aksesnya "Anyone with the link"
- [ ] Gambar proyek sudah disensor dan ditambahkan
- [ ] Semua teks "Belum ada data" sudah diisi atau dihapus
- [ ] Tidak ada angka hasil (penghematan, lead time, dll.) tanpa dokumen pendukung
- [ ] Link Email, WhatsApp, dan LinkedIn sudah dicoba
- [ ] Tampilan dicek di desktop dan HP

## Prinsip Konten

- Pekerjaan di tempat kerja, proyek tim, proyek akademik, dan solusi yang masih berupa rancangan dibedakan dengan jelas.
- Pada proyek tim, kontribusi pribadi dipisahkan dari hasil tim.
- Tidak ada klaim hasil terukur tanpa dokumentasi.

## Kontak

- Email: alfahmilabibnabil@gmail.com
- WhatsApp: https://wa.me/6285777324671
- LinkedIn: https://www.linkedin.com/in/nabil-alfahmi-labib-291751264/
