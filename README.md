# Splitter - Aplikasi Pembagian Kelompok

## 🌐 Bahasa / Language

- 🇮🇩 [Bahasa Indonesia](#deskripsi) (Current / Saat ini)
- 🇬🇧 [English](#description)

---

Aplikasi web untuk membagi peserta ke dalam kelompok secara otomatis dan acak dengan berbagai opsi pengaturan gender dan distribusi yang seimbang.

<a id="deskripsi"></a>
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

# Splitter - Group Division Application

## 🌐 Language / Bahasa

- 🇬🇧 [English](#description) (Current / Saat ini)
- 🇮🇩 [Bahasa Indonesia](#deskripsi)

---

Web application for automatically and randomly dividing participants into groups with various gender settings and balanced distribution options.

<a id="description"></a>
## 📋 Description

Splitter is a web application based on HTML, CSS, and JavaScript that allows you to:
- Automatically divide participants into multiple groups
- Configure distribution based on gender (Male/Female)
- Provide custom names for each group
- Save results in various formats (PNG Image, TXT File)
- Import previously saved data

## ✨ Main Features

### 1. **Data Title (Optional)**
- Add a title for your group data
- If not filled, will automatically use "Untitled"
- Title will appear in all outputs (results, images, TXT files)

### 2. **Participant Management**
- Easily add participants
- Select gender for each participant (Male/Female) - optional
- Remove unnecessary participants
- Participant name validation

### 3. **Gender Settings**
- **Separate by gender**: Separates Male and Female into separate groups
- **Minimum gender per group**: Set minimum number of Male/Female per group for balanced distribution

### 4. **Group Naming**
- Each group can be given a custom name
- Edit group name directly in the division results
- Group names are saved and appear in all outputs

### 5. **Update Groups**
- "Create Groups" button automatically changes to "Update Groups" after results are displayed
- Update existing groups with new participant additions/deletions
- Maintains existing group structure

### 6. **Export & Import Data**
- **Save as Image**: Export results as PNG file for display/printing
- **Save as TXT**: Export results as text file that can be imported back
- **Import Data**: Load data from previously saved TXT file
  - Loads data title
  - Loads custom group names
  - Loads all participants with gender

### 7. **Additional Features**
- Copy results to clipboard
- Randomize group division again
- Reset all data
- Real-time statistics (Total Participants, Number of Groups, Average per Group)

## 🚀 How to Use

### Data Preparation

1. **Data Title (Optional)**
   - Enter a title for your group data
   - If not filled, will automatically use "Untitled"

2. **Enter Number of Groups**
   - Determine how many groups you want

3. **Add Participants**
   - Click "Add Participant" button or press **Enter** after typing name
   - Select gender for each participant (Male/Female) - optional

4. **Gender Settings (Optional)**
   - **Separate by gender**: Activate if you want Male and Female separated
   - **Minimum gender per group**: Set minimum number of Male/Female per group

### Creating Groups

5. Click **"Create Groups"** to automatically and randomly divide participants

### After Results Appear

6. **Edit Group Name**
   - Click on the group name input field in each group card
   - Change name as desired
   - Press Enter or click outside to save

7. **Update Groups**
   - Button will automatically change to **"Update Groups"**
   - Click to update groups with participant changes (add/remove)

8. **Other Actions**
   - **Copy Results**: Copy results to clipboard
   - **Randomize Again**: Create new random division
   - **Save as Image**: Export as PNG
   - **Save as TXT**: Export as text file that can be imported

### Import Data

9. **Import Group Data**
   - Click **"Import Group Data (TXT)"** button
   - Select previously saved TXT file
   - Data will be loaded: title, group names, and all participants

### Reset

10. Click **"Reset All"** to delete all data and start from scratch

## 📁 File Structure

```
Splitter/
├── index.html           # Main application file
└── README.md           # Project documentation
```

## 🛠️ Technology

- **HTML5**: Application structure
- **CSS3**: Responsive styling and layout
- **JavaScript (Vanilla)**: Application logic and DOM manipulation
- **Canvas API**: For PNG image export

## 📱 Responsive Design

Application is designed responsively and can be used on:
- Desktop
- Tablet
- Mobile device

## 💾 File Format

### Export TXT
Saved TXT file has the format:
```
DATA TITLE
==========

Group 1
==========
1. Participant Name (male)
2. Participant Name (female)
...

Summary:
- Total: X people
- Male: X people
- Female: X people

...

OVERALL SUMMARY
=====================
Total Participants: X people
Total Groups: X groups
...
```

### Import TXT
Application can read TXT format it generates itself, including:
- Data title
- Custom group names
- Participant list with gender
- Per-group summary

## ⚙️ Division Algorithm

Application uses several division algorithms:

1. **Simple Random Distribution**: Round-robin distribution for even distribution
2. **Separate by Gender**: Separates Male and Female into separate groups
3. **Minimum Gender**: Ensures each group has minimum Male/Female according to settings
4. **Smart Update**: Adds new participants and removes deleted participants without changing existing group structure

## 🎯 Use Cases

This application is suitable for:
- Study group division
- Sports team division
- Work group division
- Class division
- Events that require group division

## 📝 Important Notes

- **Import only from TXT file**: PNG image files cannot be imported as they require OCR
- **TXT Format**: Use TXT files generated by the application for perfect import
- **Group Names**: Group names can be changed anytime after results are displayed
- **Update Groups**: Update feature maintains existing group structure and only adds/removes participants

## 🔄 Version

**Version 1.0** - Full features with:
- Optional data title
- Custom group naming
- Group update
- Export/Import data
- Gender settings

## 📄 License

This project is free to use for personal and commercial purposes.

## 👨‍💻 Development

This application is developed using vanilla JavaScript without external frameworks, so:
- Lightweight and fast
- No build process required
- Easy to deploy
- Can run directly in browser

## 🤝 Contribution

If you want to contribute or report bugs, please create an issue or pull request.

---

**Created and developed by Erlan Nauval Aqilah**
