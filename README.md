[language]
# Splitter - Aplikasi Pembagian Kelompok

Aplikasi web untuk membagi peserta ke dalam kelompok secara otomatis dan acak dengan berbagai opsi pengaturan gender dan distribusi yang seimbang.

## 📋 Deskripsi

Splitter adalah aplikasi web berbasis HTML, CSS, dan JavaScript yang memungkinkan Anda untuk:
- Membagi peserta ke dalam beberapa kelompok secara otomatis
- Mengatur distribusi berdasarkan gender (Putra/Putri)
- Memberikan nama custom untuk setiap kelompok
- Menyimpan hasil dalam berbagai format (Gambar PNG, File TXT)
- Mengimpor data yang sudah disimpan sebelumnya

## ✨ Fitur Utama

### 1. **Judul Data (Opsional)**
- Tambahkan judul untuk data kelompok Anda
- Jika tidak diisi, akan menggunakan "Untitled" secara otomatis
- Judul akan muncul di semua output (hasil, gambar, file TXT)

### 2. **Manajemen Peserta**
- Tambah peserta dengan mudah
- Pilih jenis kelamin untuk setiap peserta (Putra/Putri) - opsional
- Hapus peserta yang tidak diperlukan
- Validasi nama peserta

### 3. **Pengaturan Gender**
- **Pisahkan berdasarkan gender**: Memisahkan Putra dan Putri ke kelompok terpisah
- **Minimal gender per kelompok**: Atur jumlah minimal Putra/Putri per kelompok untuk distribusi seimbang

### 4. **Penamaan Kelompok**
- Setiap kelompok dapat diberi nama custom
- Edit nama kelompok langsung di hasil pembagian
- Nama kelompok tersimpan dan muncul di semua output

### 5. **Update Kelompok**
- Tombol "Buat Kelompok" otomatis berubah menjadi "Update Kelompok" setelah hasil ditampilkan
- Update kelompok yang sudah ada dengan perubahan peserta baru/hapus
- Mempertahankan struktur kelompok yang sudah ada

### 6. **Export & Import Data**
- **Simpan sebagai Gambar**: Export hasil sebagai file PNG untuk tampilan/print
- **Simpan sebagai TXT**: Export hasil sebagai file teks yang bisa diimport kembali
- **Import Data**: Muat data dari file TXT yang sebelumnya disimpan
  - Memuat judul data
  - Memuat nama kelompok custom
  - Memuat semua peserta dengan gender

### 7. **Fitur Tambahan**
- Salin hasil ke clipboard
- Acak ulang pembagian kelompok
- Reset semua data
- Statistik real-time (Total Peserta, Jumlah Kelompok, Rata-rata per Kelompok)

## 🚀 Cara Penggunaan

### Persiapan Data

1. **Judul Data (Opsional)**
   - Masukkan judul untuk data kelompok Anda
   - Jika tidak diisi, akan menggunakan "Untitled" secara otomatis

2. **Masukkan Jumlah Kelompok**
   - Tentukan berapa banyak kelompok yang diinginkan

3. **Tambahkan Peserta**
   - Klik tombol "Tambah Peserta" atau tekan **Enter** setelah mengetik nama
   - Pilih jenis kelamin untuk setiap peserta (Putra/Putri) - opsional

4. **Pengaturan Gender (Opsional)**
   - **Pisahkan berdasarkan gender**: Aktifkan jika ingin Putra dan Putri terpisah
   - **Minimal gender per kelompok**: Atur jumlah minimal Putra/Putri per kelompok

### Membuat Kelompok

5. Klik **"Buat Kelompok"** untuk membagi peserta secara otomatis dan acak

### Setelah Hasil Muncul

6. **Edit Nama Kelompok**
   - Klik pada input field nama kelompok di setiap kartu kelompok
   - Ubah nama sesuai keinginan
   - Tekan Enter atau klik di luar untuk menyimpan

7. **Update Kelompok**
   - Tombol akan otomatis berubah menjadi **"Update Kelompok"**
   - Klik untuk memperbarui kelompok dengan perubahan peserta (tambah/hapus)

8. **Aksi Lainnya**
   - **Salin Hasil**: Salin hasil ke clipboard
   - **Acak Ulang**: Buat pembagian baru secara acak
   - **Simpan sebagai Gambar**: Export sebagai PNG
   - **Simpan sebagai TXT**: Export sebagai file teks yang bisa diimport

### Import Data

9. **Import Data Kelompok**
   - Klik tombol **"Import Data Kelompok (TXT)"**
   - Pilih file TXT yang sebelumnya disimpan
   - Data akan dimuat: judul, nama kelompok, dan semua peserta

### Reset

10. Klik **"Reset Semua"** untuk menghapus semua data dan memulai dari awal

## 📁 Struktur File

```
Splitter/
├── index.html           # File utama aplikasi
└── README.md           # Dokumentasi proyek
```

## 🛠️ Teknologi

- **HTML5**: Struktur aplikasi
- **CSS3**: Styling dan layout responsif
- **JavaScript (Vanilla)**: Logika aplikasi dan manipulasi DOM
- **Canvas API**: Untuk export gambar PNG

## 📱 Responsive Design

Aplikasi dirancang responsif dan dapat digunakan di:
- Desktop
- Tablet
- Mobile device

## 💾 Format File

### Export TXT
File TXT yang disimpan memiliki format:
```
JUDUL DATA
==========

Kelompok 1
==========
1. Nama Peserta (putra)
2. Nama Peserta (putri)
...

Ringkasan:
- Total: X orang
- Putra: X orang
- Putri: X orang

...

RINGKASAN KESELURUHAN
=====================
Total Peserta: X orang
Total Kelompok: X kelompok
...
```

### Import TXT
Aplikasi dapat membaca format TXT yang dihasilkan sendiri, termasuk:
- Judul data
- Nama kelompok custom
- Daftar peserta dengan gender
- Ringkasan per kelompok

## ⚙️ Algoritma Pembagian

Aplikasi menggunakan beberapa algoritma pembagian:

1. **Distribusi Acak Sederhana**: Round-robin distribution untuk distribusi merata
2. **Pisah Berdasarkan Gender**: Memisahkan Putra dan Putri ke kelompok terpisah
3. **Minimal Gender**: Memastikan setiap kelompok memiliki minimal Putra/Putri sesuai pengaturan
4. **Update Cerdas**: Menambah peserta baru dan menghapus peserta yang dihapus tanpa mengubah struktur kelompok yang ada

## 🎯 Use Cases

Aplikasi ini cocok untuk:
- Pembagian kelompok belajar
- Pembagian tim olahraga
- Pembagian kelompok kerja
- Pembagian kelas
- Acara-acara yang memerlukan pembagian kelompok

## 📝 Catatan Penting

- **Import hanya dari file TXT**: File gambar PNG tidak bisa diimport karena memerlukan OCR
- **Format TXT**: Gunakan file TXT yang dihasilkan oleh aplikasi untuk import yang sempurna
- **Nama Kelompok**: Nama kelompok dapat diubah kapan saja setelah hasil ditampilkan
- **Update Kelompok**: Fitur update mempertahankan struktur kelompok yang ada dan hanya menambah/menghapus peserta

## 🔄 Versi

**Versi 1.0** - Fitur lengkap dengan:
- Judul data opsional
- Penamaan kelompok custom
- Update kelompok
- Export/Import data
- Pengaturan gender

## 📄 Lisensi

Proyek ini bebas digunakan untuk keperluan pribadi maupun komersial.

## 👨‍💻 Pengembangan

Aplikasi ini dikembangkan menggunakan vanilla JavaScript tanpa framework eksternal, sehingga:
- Ringan dan cepat
- Tidak memerlukan build process
- Mudah di-deploy
- Dapat dijalankan langsung di browser

## 🤝 Kontribusi

Jika Anda ingin berkontribusi atau melaporkan bug, silakan buat issue atau pull request.

---

**Dibuat dan dikembangkan oleh Erlan Nauval Aqilah**

