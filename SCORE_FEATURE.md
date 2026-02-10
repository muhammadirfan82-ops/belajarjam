# Fitur Sistem Skor (Scoring System)

## Ringkasan
Guru sekarang dapat mengatur skor individual untuk setiap soal di setiap game. Siswa akan mendapatkan poin sesuai dengan skor soal jika mereka menjawab dengan benar.

## Cara Menggunakan Fitur Skor

### 1. Mengatur Skor Saat Membuat Soal Baru
1. Buka **Panel Guru** → Pilih Game
2. Klik tombol **"Tambah Soal"**
3. Isi pertanyaan dan pilihan jawaban
4. Di bagian **"Skor (poin untuk jawaban benar)"**, masukkan nilai skor yang diinginkan
   - Default: 10 poin
   - Rentang: 1-100 poin
5. Klik **"Simpan"**

### 2. Mengubah Skor Soal yang Sudah Ada
1. Buka **Panel Guru** → Pilih Game
2. Cari soal yang ingin diubah skornya
3. Klik tombol **"Edit"** pada soal tersebut
4. Ubah nilai di bagian **"Skor (poin untuk jawaban benar)"**
5. Klik **"Simpan"** untuk menyimpan perubahan

### 3. Melihat Skor di Daftar Soal
- Setiap soal menampilkan badge biru yang berisi informasi skor
- Format: **"XX poin"** (contoh: "10 poin", "25 poin")
- Badge ditampilkan di samping kanan pertanyaan

## Cara Kerja di Game

### Perhitungan Skor Siswa
1. Siswa menjawab soal dengan benar → mendapatkan poin sesuai skor soal
2. Siswa menjawab soal dengan salah → mendapatkan 0 poin
3. Total skor adalah penjumlahan semua poin yang dikumpulkan

### Tampilan Hasil Akhir Game
Di akhir game, siswa akan melihat:
- **Skor Akhir**: Contoh "85/100 poin"
- **Persentase**: Contoh "85%"
- **Pesan Motivasi**: Berdasarkan persentase yang dicapai

### Pesan Motivasi Berdasarkan Persentase
- 100% → "Sempurna! Kamu hebat! 🌟"
- 80-99% → "Bagus sekali! 👏"
- 60-79% → "Bagus! Terus latihan 💪"
- <60% → "Ayo coba lagi! 📚"

## Contoh Skenario

### Skenario 1: Skor Standar
- Game memiliki 10 soal, masing-masing bernilai 10 poin
- Total skor maksimal = 100 poin
- Jika siswa benar 8 soal, skor = 80 poin

### Skenario 2: Skor Berbeda per Soal
- Soal 1: 5 poin (mudah)
- Soal 2: 10 poin (sedang)
- Soal 3: 15 poin (sulit)
- Total skor maksimal = 30 poin
- Jika siswa benar semua, skor = 30 poin

## Tips Menggunakan Fitur Skor

1. **Sesuaikan Tingkat Kesulitan**
   - Soal mudah: 5-10 poin
   - Soal sedang: 10-15 poin
   - Soal sulit: 15-25 poin

2. **Motivasi Siswa**
   - Berikan poin bonus pada soal tertentu untuk motivasi
   - Variasikan skor untuk membuat game lebih menarik

3. **Pengecekan Pemahaman**
   - Lihat persentase siswa untuk mengetahui pemahaman mereka
   - >80% = pemahaman baik
   - 60-80% = perlu latihan lebih
   - <60% = perlu bimbingan lebih

## Informasi Teknis

- **Field**: `score` di setiap Question
- **Tipe Data**: Number (angka)
- **Range**: 1-100
- **Default**: 10
- **Penyimpanan**: localStorage (per game)
- **Kompatibilitas**: Semua browser modern

## Dukungan Teknis

Jika ada masalah dengan fitur skor:
1. Pastikan skor soal sudah diatur di Panel Guru
2. Refresh halaman jika tidak melihat perubahan skor
3. Cek browser console untuk pesan error (F12 → Console)
