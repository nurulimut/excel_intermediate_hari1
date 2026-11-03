# Modul Peserta OfficeMart Hari 1

Modul baca untuk peserta **Microsoft Excel for Professional — Intermediate Class**, Hari 1:
*Data Preparation, Navigasi & Logical Formulas*.

Isi per sesi: learning outcome, konsep inti, rumus kunci, studi kasus OfficeMart, langkah kerja di file latihan, dan jebakan umum. Dilengkapi cheat sheet shortcut dengan gambar keyboard interaktif, dua demo interaktif (simulasi IF/AND/OR/IFS dan pemisah kode `LEFT/MID/FIND`) serta post-test 8 soal.

| Sesi | Topik |
|---|---|
| Mulai di sini | Cara pakai file, agenda, aturan bisnis |
| Session 1 | Excel Table & Data Validation |
| Session 2 | Hyperlink & Navigasi Workbook |
| Session 3 | IF, AND/OR, IFS, IFERROR, IFNA |
| Session 4 | TODAY, EOMONTH, NETWORKDAYS, WEEKDAY, TEXT |
| Session 5 | Text Cleaning & Conditional Formatting |
| Session 6 | Lab Error: #VALUE!, #NAME?, #REF!, hyperlink rusak |
| Cheat Sheet | 43 shortcut dengan keyboard interaktif, fungsi favorit, referensi $ (F4), kode format angka, arti error |
| Closing | Hands-on integrasi & post-test |

> Seluruh data OfficeMart bersifat fiktif dan hanya untuk latihan.

## Struktur

```
index.html   # seluruh halaman (HTML + CSS + JS dalam satu file, tanpa build)
.nojekyll    # agar GitHub Pages menyajikan file apa adanya
README.md
```

Tidak ada dependensi atau proses build. Font dimuat dari Google Fonts; jika offline, halaman memakai font sistem.

## Deploy

### Opsi A — GitHub Pages

1. Buat repository baru di GitHub (Public), misalnya `excel-intermediate-hari1`.
2. Upload ketiga file ini ke branch `main` (tombol **Add file ▸ Upload files**), atau lewat terminal:
   ```bash
   git init
   git add .
   git commit -m "Modul peserta Excel Intermediate Hari 1"
   git branch -M main
   git remote add origin https://github.com/<username>/excel-intermediate-hari1.git
   git push -u origin main
   ```
3. Buka **Settings ▸ Pages**. Pada *Build and deployment*, pilih **Deploy from a branch**, branch `main`, folder `/ (root)`, lalu **Save**.
4. Tunggu 1–2 menit. Situs aktif di `https://<username>.github.io/excel-intermediate-hari1/`.

### Opsi B — Vercel

1. Push repository ke GitHub (langkah 1–2 di atas).
2. Masuk ke [vercel.com](https://vercel.com) ▸ **Add New ▸ Project** ▸ pilih repository ini.
3. Framework Preset: **Other**. Build Command dan Output Directory dibiarkan kosong.
4. Klik **Deploy**. Setiap push ke `main` akan memperbarui situs otomatis.

## Mengubah konten

Semua teks ada di `index.html`. Setiap sesi adalah satu blok `<section id="s1">` … `<section id="s6">`; menu samping ada di `<nav class="index">`. Soal post-test ada di bagian `<script>` pada array `Q`; daftar shortcut cheat sheet ada di array `SC`.

Rumus ditulis dengan pemisah titik koma (`;`) sesuai pengaturan regional Indonesia.
