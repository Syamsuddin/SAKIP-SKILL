# Panduan Penggunaan SAKIP Skill Suite

Dokumen ini akan memandu Anda langkah demi langkah dalam menggunakan paket skill SAKIP untuk mengoptimalkan dokumen perencanaan, pelaksanaan, dan pelaporan kinerja instansi pemerintah hingga mencapai predikat AA dalam evaluasi SAKIP oleh KemenPAN-RB.

## Prasyarat

- Aplikasi chatbot Claude dengan SAKIP Skill Suite terpasang (file `.skill`).
- Memahami dasar-dasar siklus SAKIP dan dokumen terkait (RPJMD, Renstra, RKT, PK, IKU, LKIP).
- Memiliki akses ke dokumen perencanaan dan data kinerja instansi.

## Tahap 1: Memulai Percakapan dan Orkestrator

1. Buka aplikasi chatbot Claude dan mulai percakapan baru.
2. Jelaskan bahwa Anda ingin mengoptimalkan dokumen SAKIP instansi untuk mengejar predikat tertentu (misal: "Saya ingin meningkatkan nilai SAKIP Dinas X dari BB ke A").
3. `sakip-orkestrator` akan merespons dan mengumpulkan informasi dasar seperti nama instansi, periode Renstra, dan predikat saat ini.
4. Jawab pertanyaan orkestrator dengan data aktual agar konteks jelas.
5. Orkestrator akan menyimpan data ini dalam Dosir Kinerja dan merutekan ke langkah berikutnya.

## Tahap 2: Perencanaan Kinerja dengan `sakip-perencana`

1. Jika dokumen perencanaan belum optimal, orkestrator akan menyarankan untuk menggunakan `sakip-perencana`.
2. Siapkan draft atau garis besar dokumen Renstra, RKT, dan PK instansi.
3. Jabarkan struktur organisasi, tugas pokok dan fungsi, dan isu-isu strategis yang ingin ditangani dalam periode perencanaan.
4. `sakip-perencana` akan memandu dalam menyusun sasaran strategis, indikator kinerja (IKU/IKK), dan target yang SMART (Specific, Measurable, Achievable, Relevant, Time-bound).
5. Paparkan rancangan pohon kinerja (cascading) dari level nasional ke level instansi.
6. Perencana akan memberikan umpan balik dan saran perbaikan untuk memastikan keselarasan vertikal dan horizontal.
7. Lakukan iterasi perbaikan dokumen perencanaan hingga perencana menyatakan kualitasnya baik.

## Tahap 3: Pengukuran & Pelaporan Kinerja dengan `sakip-pelaporan` 

1. Siapkan data realisasi kinerja dan anggaran instansi, idealnya sampai level eselon IV secara periodik (bulanan, triwulanan, tahunan).
2. Gunakan `sakip-pelaporan` untuk menyusun kerangka pengukuran kinerja sesuai IKU/IKK dan target dalam dokumen perencanaan.
3. Masukkan data realisasi dan lakukan perhitungan capaian, analisis efisiensi (kinerja dibandingkan penyerapan anggaran), dan identifikasi faktor pendorong/penghambat.
4. Buat draft LKIP dengan bantuan `sakip-pelaporan` - pastikan ada narasi analitis, tidak sekadar tabel angka.
5. Pelaporan akan menilai kualitas LKIP dan memberikan saran perbaikan dari lensa evaluator - lakukan iterasi hingga kualitas memuaskan.

## Tahap 4: Evaluasi Mandiri dengan `sakip-evaluator`

1. Dengan dokumen perencanaan, hasil pengukuran, dan LKIP yang sudah disusun, jalankan `sakip-evaluator` untuk mensimulasikan penilaian AKIP.
2. Evaluator akan menilai setiap komponen sesuai PermenPAN-RB 88/2021 dan memberikan skor per komponen serta total nilai AKIP.
3. Evaluator juga akan memprediksi predikat (AA, A, BB, B, CC, C) dan mengidentifikasi aspek-aspek yang menghambat pencapaian predikat lebih tinggi.
4. Hasil penilaian mandiri ini akan disimpan dalam Dosir Kinerja sebagai baseline.

## Tahap 5: Penyusunan Rencana Aksi dengan `sakip-improver`

1. Berbekal hasil evaluasi mandiri, gunakan `sakip-improver` untuk mengonversi temuan dan rekomendasi menjadi rencana aksi yang konkret dan terukur.
2. Improver akan membantu menentukan prioritas perbaikan berdasarkan potensi penambahan nilai terbesar dengan sumber daya minimal.
3. Susun daftar aksi yang tersekuens dengan penanggung jawab, tenggat waktu, dan metrik keberhasilan yang jelas.
4. Integrasikan rencana aksi ini dengan sistem manajemen kinerja instansi untuk memastikan implementasi dan pemantauan.

## Tahap 6: Eksekusi Rencana & Iterasi

1. Dengan panduan orkestrator, eksekusi rencana aksi secara bertahap sesuai tenggat waktu.
2. Secara berkala (misal: tiap semester), ulangi Tahap 3-5 untuk melihat progres:
   - Perbarui data kinerja dan susun LKIP terbaru dengan `sakip-pelaporan`.
   - Evaluasi ulang dengan `sakip-evaluator` untuk mengetahui perubahan nilai AKIP.
   - Identifikasi area perbaikan dan susun rencana tindak lanjut dengan `sakip-improver`.
3. Lakukan siklus ini hingga target predikat AKIP tercapai.

## Tips Menggunakan Suite

- Sertakan data aktual sebanyak mungkin agar umpan balik skill relevan.
- Jangan ragu untuk meminta klarifikasi atau rekomendasi yang lebih spesifik.
- Validasi hasil kerja skill dengan pihak-pihak terkait dalam instansi untuk memastikan kelayakan implementasi.
- Manfaatkan fitur "Dosir Kinerja" sebagai hasil antara yang dapat dibagikan dan direviu bersama.

Dengan mengikuti panduan bertahap ini dan memanfaatkan paket lengkap skill SAKIP, Anda dapat secara sistematis dan efisien meningkatkan kualitas perencanaan, pengukuran, pelaporan, dan evaluasi kinerja instansi hingga mencapai predikat tertinggi dalam evaluasi SAKIP. Selamat mencoba!

