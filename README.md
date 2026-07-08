# Dashboard Penyerapan AKI UPP Sulawesi Tengah 2026

Executive dashboard PT PLN (Persero) untuk memonitor penyerapan AKI Proyek
(Jaringan, Pembangkit, Pertanahan) Tahun 2026. Data ditarik **otomatis (realtime)**
dari Google Sheets — begitu isi sheet berubah, dashboard ikut ter-update.

## Cara upload ke GitHub Pages
1. Buat repository baru di GitHub (mis. `dashboard-aki-sulteng`).
2. Upload file **`index.html`** ke repo (cukup satu file ini — logo sudah tertanam).
3. Buka **Settings → Pages → Source: `main` / root → Save**.
4. Tunggu ±1 menit, dashboard tampil di `https://<username>.github.io/<repo>/`.

Bisa juga langsung dibuka di HP dengan cara double-click `index.html` (tampilan sudah mobile friendly).

## Mengubah sumber data / kategori
Semua pengaturan ada di objek **`CONFIG`** di dalam `index.html` (bagian `<script>`):

| Pengaturan            | Keterangan                                            |
|-----------------------|-------------------------------------------------------|
| `csvUrl`              | Link CSV Google Sheets (File → Share → Publish to web → CSV) |
| `refreshMs`           | Interval auto-refresh (default 5 menit)               |
| `col.planAki`         | Nama kolom Plan AKI  (default `Kebutuhan AKI 2026`)   |
| `col.realAki`         | Nama kolom Realisasi (default `Total Realisasi`)      |
| `kategoriMap`         | Pemetaan kode → kategori (`JAR→Jaringan`, `KIT→Pembangkit`, `TANAH→Pertanahan`) |
| `planKeys`/`realKeys` | Nama kolom Plan/Real per bulan                        |

## Menambah informasi baru nanti
Struktur kode dibagi per Section (1–7) dengan komentar berbahasa Indonesia,
sehingga mudah menambah kartu/grafik baru. Cukup tambahkan blok HTML pada
`<div class="section">` dan panggil datanya di fungsi `render()`.

---
Created by : **Samuel Guhan**
