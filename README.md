# Angka, Pola & Bentuk Pertamaku — Calistung Ceria Modul 2 TK

Permainan matematika fondasi untuk anak TK: kesadaran bilangan, pola, bentuk,
klasifikasi, dan ruang. Produk **Toko Aplikasi Edukasi AwwanMahda**, dibangun
dengan mesin yang sama dengan Modul 1 (Calistung Ceria) — satu berkas
`index.html` vanilla tanpa CDN, PWA offline, TTS Bahasa Indonesia.

- **Status:** v1.0 — dibangun & diuji lokal 15 November 2026 (belum deploy).
- **Acuan materi:** Peta Materi TK (CP Fase Fondasi, Keputusan Kepala BSKAP
  046/H/KR/2025) — Modul 2: Matematika.

## Isi (14 aktivitas, ronde 10 soal)

- **Bilangan & Berhitung (5):** Hitung & Pilih Angka, Angka & Jumlahnya,
  Banyak atau Sedikit, Sama Banyak, Hitung Mundur.
- **Pola (4):** Pola AB, Pola ABC, Pola ABCD, Pola Bentuk.
- **Bentuk & Ruang (5):** Kenal Bentuk, Bentuk di Sekitarku, Satu Kelompok
  (klasifikasi), Paling Besar / Kecil, Di Mana Posisinya? (posisi & ruang).

## Model B (demo + kode akses)

- **Gratis (demo):** Hitung & Pilih Angka, Banyak atau Sedikit, Pola AB,
  Kenal Bentuk, Di Mana Posisinya? (5 aktivitas).
- **Terkunci:** 9 aktivitas lain, dibuka dengan kode akses format
  `CERIA2-XXXXXX`. Aplikasi hanya menyimpan **hash SHA-256** kode.
- Satu **kode uji internal** dibuat untuk QA (plaintext TIDAK dicatat di sini;
  disimpan admin di berkas kode akses Modul 2). Batch produksi dibuat terpisah
  saat rilis.
- `LINK_BELI` di `index.html` sementara menunjuk Linktree toko; ganti ke
  tautan produk Lynk Modul 2 bila produknya sudah terbit.

## Prinsip desain (dari Peta Materi TK)

- Belajar lewat bermain bermakna; aplikasi **menstimulasi kesiapan belajar**,
  bukan janji instan. Tanpa skor hukuman/label gagal — penguatan berupa
  dorongan & bintang proses.
- Sesi pendek 5–10 menit (10 soal), titik berhenti alami di layar selesai,
  saran kegiatan di luar layar (bergerak & benda sungguhan) di akhir permainan.
- Kunci localStorage memakai awalan `cm2_` agar tidak bertabrakan dengan
  Modul 1 bila di-host pada domain yang sama.

## Teknis

- `index.html` + `manifest.webmanifest` + `sw.js` (cache `calistung-modul2-v1`,
  cache-first) + `icon.svg`. Tanpa dependensi/CDN.
- Deploy (saat rilis): impor repo ke Vercel (preset Other/static, tanpa build
  command) — sama seperti Modul 1.

## Struktur penamaan produk (baku proyek)

`Jenjang + Kelas + Semester + Mata Pelajaran` — modul ini: **TK · Modul 2 · Matematika Fondasi**.
