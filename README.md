# 🎓 Game Edukasi - Belajar Jam

Aplikasi game edukasi interaktif untuk siswa kelas 2 SD yang membantu belajar membaca jam analog dan digital, memahami durasi, serta mengenal konsep waktu.

## ✨ Fitur Utama

### 🎮 4 Game Interaktif
1. **Baca Jam Analog** - Belajar membaca jam dengan jarum jam (jarum pendek = jam, jarum panjang = menit)
2. **Baca Jam Digital** - Latihan membaca angka di layar jam digital
3. **Hitung Durasi** - Menghitung berapa lama waktu berlalu antara dua waktu
4. **Padukan Aktivitas** - Mencocokkan aktivitas sehari-hari dengan waktu yang tepat

### 👨‍🏫 Panel Guru
- **Edit Soal**: Guru dapat menambah, mengubah, dan menghapus soal untuk setiap game
- **Kelola Pertanyaan**: Customize pertanyaan dan jawaban sesuai kurikulum
- **Reset ke Standar**: Kembalikan soal ke pengaturan default jika diperlukan
- **Akses**: Buka dari halaman home → "Buka Panel Guru"

### 🔊 Audio Feedback
- **Suara Benar**: Nada musik ceria ketika siswa menjawab benar, disertai ucapan "Jawaban kalian benar! Hebat sekali!"
- **Suara Salah**: Nada musik yang menenangkan ketika jawaban salah, disertai ucapan "Jawaban kalian salah. Coba lagi!"
- **Motivasi**: Feedback audio membantu memotivasi siswa untuk terus belajar

### 🎯 Fitur Pembelajaran
- Progress bar untuk tracking kemajuan
- Sistem poin dan bintang
- Pesan motivasi berdasarkan skor akhir
- Opsi untuk bermain ulang
- 10 soal per sesi game

## 🚀 Cara Menggunakan

### Untuk Siswa
1. Buka aplikasi dan pilih salah satu dari 4 game
2. Baca pertanyaan dengan seksama
3. Lihat jam (analog/digital) atau informasi yang diberikan
4. Pilih jawaban yang benar dengan mengklik tombol
5. Dengarkan feedback audio dan lihat hasilnya
6. Lanjutkan ke soal berikutnya
7. Lihat skor akhir di akhir permainan

### Untuk Guru
1. Dari halaman home, klik "Buka Panel Guru"
2. Pilih salah satu dari 4 game yang ingin diedit
3. **Tambah Soal Baru**:
   - Klik tombol "Tambah Soal"
   - Isi pertanyaan
   - Isi 4 pilihan jawaban
   - Tandai jawaban yang benar dengan radio button
   - Klik "Simpan"
4. **Edit Soal Existing**:
   - Klik tombol "Edit" di soal yang ingin diubah
   - Modifikasi pertanyaan atau jawaban
   - Klik "Simpan"
5. **Hapus Soal**:
   - Klik tombol "Hapus" (tempat sampah) pada soal
6. **Reset ke Standar**:
   - Klik "Kembalikan ke Standar" untuk reset semua soal

## 🎨 Desain & Warna

Setiap game memiliki warna unik:
- **Baca Jam Analog**: Ungu & Biru
- **Baca Jam Digital**: Biru
- **Hitung Durasi**: Oranye
- **Padukan Aktivitas**: Pink

## 💾 Penyimpanan Data

- Soal-soal yang diedit disimpan di localStorage browser
- Data per game tersimpan terpisah
- Guru dapat reset soal ke standar kapan saja
- Tidak perlu login - akses langsung

## 🔧 Teknologi yang Digunakan

- **Frontend**: Next.js 16, React 19, TypeScript
- **UI Components**: shadcn/ui
- **Styling**: Tailwind CSS
- **Audio**: Web Audio API & Web Speech API (text-to-speech)
- **Storage**: Browser localStorage

## 📱 Responsive Design

- Desain mobile-first yang bekerja di semua ukuran layar
- Optimal untuk tablet dan smartphone siswa
- Interface yang user-friendly untuk anak-anak

## 🎓 Tujuan Pembelajaran

Aplikasi ini dirancang untuk membantu siswa kelas 2 SD:
- ✓ Membaca jam analog dengan memahami posisi jarum jam
- ✓ Membaca jam digital dengan memahami format jam:menit
- ✓ Menghitung durasi/lama waktu berlalu
- ✓ Mengenal konsep waktu dalam kehidupan sehari-hari
- ✓ Meningkatkan pemahaman tentang manajemen waktu

## 📝 Catatan

- Aplikasi ini menggunakan Text-to-Speech API browser untuk feedback audio
- Pastikan browser mendukung Web Audio API
- Untuk hasil terbaik, gunakan browser modern (Chrome, Firefox, Safari, Edge)
- Volume device harus dinyalakan untuk mendengar audio feedback

---

Dibuat dengan ❤️ untuk memudahkan pembelajaran anak-anak tentang waktu.
