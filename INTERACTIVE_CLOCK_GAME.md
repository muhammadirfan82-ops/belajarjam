# Game Jam Interaktif dengan Soal dan Scoring

## Fitur Baru

Jam Interaktif sekarang dilengkapi dengan sistem soal lengkap, scoring, dan panel edit guru yang canggih!

### 1. Sistem Soal untuk Game Interaktif

#### Struktur Soal
Setiap soal jam interaktif memiliki:
- **question**: Pertanyaan/instruksi untuk siswa (e.g., "Atur jam ke pukul 08:00")
- **targetTime**: Waktu target dalam format HH:MM (e.g., "08:00")
- **tolerance**: Toleransi menit untuk jawaban yang diterima (default: 1 menit)
- **score**: Poin yang didapat jika jawaban benar (default: 15 poin)

#### Contoh Soal Default
```javascript
{
  id: '1',
  gameType: 'interactive',
  question: 'Atur jam ke pukul 08:00 (pagi hari, saatnya sekolah)',
  targetTime: '08:00',
  tolerance: 1,
  score: 15,
  answers: [],
  correctAnswerIndex: 0,
}
```

### 2. Gameplay

Siswa melakukan:
1. Melihat pertanyaan yang menginstruksikan waktu tertentu
2. Menyeret jarum jam untuk mengatur waktu
3. Menekan tombol "Periksa Jawaban"
4. Mendapat feedback audio dan visual
5. Menerima skor jika jawaban benar

**Sistem Validasi:**
- Waktu yang diatur harus berada dalam toleransi (±X menit) dari target
- Hanya jam dan menit yang dihitung (detik diabaikan)
- Contoh: Target 08:00 dengan tolerance 1 = 07:59 hingga 08:01 diterima

### 3. Panel Guru - Edit Soal Jam Interaktif

Guru dapat mengakses panel edit soal jam interaktif di `/teacher`:

#### Fitur Edit:
- **Tambah Soal**: Buat soal baru dengan pertanyaan, waktu target, toleransi, dan skor
- **Edit Soal**: Ubah pertanyaan, waktu target, toleransi, atau skor
- **Hapus Soal**: Menghapus soal yang tidak diperlukan
- **Reset Default**: Kembalikan ke soal standar

#### Input Fields:
1. **Pertanyaan**: Text area untuk instruksi kepada siswa
2. **Waktu Target**: Time input (format HH:MM)
3. **Toleransi Menit**: Number input (0-5 menit)
4. **Skor (poin)**: Number input (1-100 poin)

#### Tampilan Soal:
- Menampilkan emoji aktivitas berdasarkan waktu (🌅 pagi, ☀️ siang, 🌆 sore, 🌙 malam)
- Menampilkan detail waktu target, toleransi, dan skor
- Tombol Edit dan Hapus untuk setiap soal

### 4. Scoring System

**Perhitungan Skor:**
- Siswa mendapat poin hanya jika jawaban benar (dalam toleransi)
- Total skor = sum dari semua poin soal yang dijawab benar
- Persentase = (skor didapat / total skor maksimal) × 100%

**Hasil Akhir:**
- Menampilkan skor: "XX/YY poin"
- Menampilkan persentase keberhasilan
- Pesan motivasi berdasarkan persentase

### 5. Komponen Baru

#### InteractiveClockEditor
- Path: `/components/InteractiveClockEditor.tsx`
- Props:
  - `gameType`: 'interactive'
  - `questions`: Array of Question
  - `onQuestionsChange`: Callback untuk update soal
- Fitur:
  - Form untuk tambah soal
  - List soal dengan edit/delete
  - Validation sebelum save
  - Display emoji aktivitas

#### Update InteractiveAnimatedClock
- Props baru:
  - `initialHours`: Jam awal (default: 10)
  - `initialMinutes`: Menit awal (default: 30)
  - `onTimeChange`: Callback saat waktu berubah
- Trigger callback setiap kali jarum di-drag

### 6. Default Questions

4 soal sudah disediakan:
1. Pukul 08:00 - Pagi hari (saatnya sekolah) - 15 poin
2. Pukul 12:00 - Siang hari (waktu makan siang) - 15 poin
3. Pukul 15:30 - Sore hari (waktu bermain) - 15 poin
4. Pukul 19:00 - Malam hari (waktu makan malam) - 15 poin

Total skor maksimal dengan default soal: 60 poin

### 7. File yang Dimodifikasi

1. `/lib/questions-storage.ts`
   - Tambah 'interactive' ke gameType
   - Tambah targetTime dan tolerance ke Question interface
   - Tambah default soal untuk interactive

2. `/components/InteractiveClockEditor.tsx` (NEW)
   - Editor khusus untuk soal jam interaktif

3. `/components/InteractiveAnimatedClock.tsx`
   - Tambah props: initialHours, initialMinutes, onTimeChange
   - Tambah callback di handleMouseMove dan handleTouchMove

4. `/app/games/interactive-clock/page.tsx`
   - Complete game logic dengan soal dan scoring
   - Validasi jawaban dengan tolerance
   - Audio feedback
   - Score calculation

5. `/app/teacher/page.tsx`
   - Tambah 'interactive' game type
   - Import InteractiveClockEditor
   - Conditional render untuk editor yang sesuai

### 8. Workflow Penggunaan

**Untuk Guru:**
1. Buka `/teacher`
2. Klik "Jam Interaktif"
3. Lihat soal default atau tambah soal baru
4. Edit waktu target, toleransi, atau skor sesuai kebutuhan
5. Soal otomatis tersimpan

**Untuk Siswa:**
1. Ke menu home
2. Klik "Jam Interaktif"
3. Baca pertanyaan
4. Drag jarum jam ke waktu yang benar
5. Klik "Periksa Jawaban"
6. Lihat hasil dan skor

---

**Contoh Alur Validasi:**
- Target: 15:30 (sore)
- Tolerance: 2 menit
- Jawaban Benar: 15:28, 15:29, 15:30, 15:31, 15:32
- Jawaban Salah: 15:27, 15:33, atau waktu lain

Fitur ini sempurna untuk pembelajaran interaktif di Interactive Flat Panel!
