# 👨‍🏫 Panduan Guru - Mengelola Soal Game Edukasi

Selamat datang di Panel Guru! Panduan ini menjelaskan cara mengelola soal-soal untuk setiap game edukasi.

---

## 🚀 Akses Panel Guru

1. Buka aplikasi di halaman home
2. Scroll ke bawah atau cari tombol **"Buka Panel Guru"**
3. Klik tombol tersebut untuk masuk ke dashboard guru

---

## 📚 Dashboard Guru

Anda akan melihat 4 card game dengan informasi:
- Nama game
- Deskripsi singkat
- Jumlah soal yang tersedia
- Tombol "Edit Soal"

Setiap game dapat diedit secara terpisah. Soal-soal tidak akan tercampur antar game.

---

## ✏️ Mengelola Soal

### 1. MEMBACA SOAL YANG ADA

Ketika Anda klik "Edit Soal" untuk suatu game, Anda akan melihat:
- Daftar semua soal untuk game tersebut
- Setiap soal menampilkan:
  - Pertanyaan
  - 4 pilihan jawaban dengan warna:
    - **Hijau** = Jawaban yang benar
    - **Abu-abu** = Jawaban yang salah
  - Tombol Edit dan Hapus

---

### 2. MENAMBAH SOAL BARU

**Langkah-langkah:**

1. Klik tombol **"+ Tambah Soal"** di bagian atas daftar soal
2. Form akan muncul untuk soal baru:

   **Bagian 1: Pertanyaan**
   - Ketik pertanyaan di text area
   - Contoh: "Dari pukul 08:00 sampai pukul 09:30, berapa lama?"

   **Bagian 2: Pilihan Jawaban**
   - Anda akan melihat 4 input field untuk jawaban
   - Di samping setiap jawaban ada radio button
   - **Penting**: Pilih radio button untuk jawaban yang BENAR

   **Contoh:**
   ```
   ○ 30 menit
   ⦿ 1 jam 30 menit  ← TANDAI INI (jawaban benar)
   ○ 1 jam
   ○ 2 jam
   ```

3. Klik tombol **"✓ Simpan"** untuk menyimpan soal baru
4. Soal akan ditambahkan ke daftar

---

### 3. MENGEDIT SOAL YANG ADA

**Langkah-langkah:**

1. Cari soal yang ingin diedit di daftar
2. Klik tombol **"✏️ Edit"** pada soal tersebut
3. Form edit akan terbuka dengan:
   - Pertanyaan yang bisa diubah
   - 4 jawaban yang bisa dimodifikasi
   - Radio button untuk menandai jawaban benar

4. Lakukan perubahan yang diinginkan
5. Pastikan jawaban benar sudah ditandai dengan radio button
6. Klik **"✓ Simpan"** untuk menyimpan perubahan
7. Atau klik **"✗ Batal"** untuk membatalkan

---

### 4. MENGHAPUS SOAL

**Langkah-langkah:**

1. Cari soal yang ingin dihapus
2. Klik tombol **"🗑️"** (tempat sampah) di sebelah tombol Edit
3. Soal akan langsung dihapus dari daftar
4. **Catatan**: Penghapusan bersifat permanen untuk session ini

---

### 5. RESET KE SOAL STANDAR

Jika Anda ingin mengembalikan semua soal ke pengaturan awal:

1. Di halaman edit soal, lihat bagian atas
2. Ada card putih dengan tombol **"↻ Kembalikan ke Standar"**
3. Klik tombol tersebut
4. Sistem akan menanyakan konfirmasi: "Yakin ingin mengembalikan soal ke pengaturan standar?"
5. Klik "OK" untuk mengkonfirmasi
6. Semua soal custom akan dihapus dan soal standar akan dipulihkan

---

## 📋 Soal-Soal Standar

Setiap game sudah dilengkapi dengan soal-soal standar:

### Game 1: Baca Jam Analog (5 soal)
- Pertanyaan tentang membaca jam dengan jarum
- Fokus pada pemahaman posisi jarum pendek (jam) dan jarum panjang (menit)

### Game 2: Baca Jam Digital (5 soal)
- Pertanyaan tentang membaca angka di jam digital
- Fokus pada format jam:menit dan periode waktu (pagi/siang/sore/malam)

### Game 3: Hitung Durasi (5 soal)
- Pertanyaan tentang menghitung lama waktu
- Fokus pada perhitungan durasi antara dua waktu

### Game 4: Padukan Aktivitas (5 soal)
- Pertanyaan tentang mencocokkan aktivitas dengan waktu sehari-hari
- Fokus pada pemahaman jadwal aktivitas normal

---

## 💡 Tips Membuat Soal yang Baik

### 1. PERTANYAAN YANG JELAS
- ✅ Gunakan bahasa yang sederhana dan mudah dipahami anak kelas 2 SD
- ✅ Pertanyaan harus spesifik dan tidak ambigu
- ❌ Hindari pertanyaan yang terlalu kompleks atau bertele-tele

### 2. JAWABAN YANG BERMAKNA
- ✅ Buat pilihan jawaban yang masuk akal sebagai distraksi
- ✅ Hindari pilihan yang terlalu jelas salah
- ❌ Jangan buat semua jawaban terlihat sama

### 3. TINGKAT KESULITAN
- ✅ Mulai dari soal mudah untuk game pertama
- ✅ Gradually increase difficulty
- ✅ Seimbangkan antara soal mudah dan sulit

### 4. KONSISTENSI FORMAT
- ✅ Untuk Baca Jam Analog: format "Pukul HH:MM" (Pukul 03:00)
- ✅ Untuk Baca Jam Digital: format "HH:MM" atau deskripsi waktu
- ✅ Untuk Durasi: format "X jam Y menit" atau "X menit"
- ✅ Untuk Aktivitas: deskripsi aktivitas atau waktu

---

## 🔊 Audio Feedback untuk Siswa

Ketika siswa bermain:
- **Jawaban Benar**: 
  - Suara musik yang ceria (3 nada naik)
  - Ucapan: "Jawaban kalian benar! Hebat sekali!"
  
- **Jawaban Salah**:
  - Suara musik yang lembut (3 nada turun)
  - Ucapan: "Jawaban kalian salah. Coba lagi!"

Audio ini membantu memberikan umpan balik langsung kepada siswa.

---

## 📊 Monitoring Soal

### Melihat Daftar Soal
- Dari dashboard guru, jumlah soal ditampilkan di setiap card game
- Klik "Edit Soal" untuk melihat detail semua soal

### Backup Soal
- Soal disimpan di localStorage browser
- Jika ingin backup, catat nomor dan konten soal di notepad

### Sharing Soal
- Soal tidak bisa di-export/import secara otomatis
- Jika perlu sharing, ketik ulang soal di device lain

---

## ⚙️ Troubleshooting

### Soal Tidak Tersimpan
- **Penyebab**: Browser tidak mendukung localStorage atau dalam private mode
- **Solusi**: Gunakan browser normal (bukan private mode) dan pastikan storage diizinkan

### Soal Hilang setelah Refresh
- **Penyebab**: Mungkin clear browser cache atau cookies
- **Solusi**: Catat soal Anda, atau gunakan "Kembalikan ke Standar" lalu edit ulang

### Tidak Ada Audio Saat Test
- **Penyebab**: Volume device mati atau speaker tidak terhubung
- **Solusi**: Periksa volume device, atau aktifkan speaker/earphone

### Jawaban Tidak Ditandai Benar
- **Penyebab**: Lupa klik radio button untuk jawaban yang benar
- **Solusi**: Pastikan SELALU tandai salah satu jawaban sebagai benar sebelum simpan

---

## 🎯 Workflow Rekomendasi

### Awal Tahun Ajaran
1. Review soal-soal standar
2. Sesuaikan dengan kurikulum lokal Anda
3. Tambah atau kurangi soal sesuai kebutuhan

### Selama Pembelajaran
1. Monitor progress siswa
2. Adjust kesulitan soal jika diperlukan
3. Tambah soal baru untuk reinforcement

### Persiapan Ulangan
1. Buat soal lebih sulit/mudah sesuai level siswa
2. Fokus pada topik yang belum dikuasai
3. Gunakan audio feedback untuk motivasi

---

## 📞 Dukungan & Feedback

Jika ada pertanyaan atau saran tentang panel guru:
- Hubungi developer
- Laporkan bug atau error
- Sarankan fitur baru yang membantu

---

**Semoga berhasil menggunakan Panel Guru!** 🎓✨

Ingat: Soal yang baik akan meningkatkan pembelajaran siswa! 📚
