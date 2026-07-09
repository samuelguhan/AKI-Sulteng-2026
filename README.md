# Dashboard Penyerapan AKI UPP Sulawesi Tengah 2026

Executive dashboard PT PLN (Persero) untuk memonitor penyerapan AKI Proyek
(Jaringan, Pembangkit, Pertanahan) Tahun 2026. Bergaya konsultan (McKinsey/BCG),
latar cerah, interaktif, dan **realtime** — data ditarik otomatis dari Google Sheets.

## Fitur
- **Filter Kategori:** Overall, Pertanahan, Pembangkit, Jaringan
- **Filter Waktu:** Per Bulan (dengan pemilih bulan), Semester 1, Semester 2, Overall (1 Tahun)
- KPI ringkas, progress penyerapan (1 donut), perbandingan kategori
- **Bar chart stacked per bulan** (realisasi vs sisa plan) dengan nilai %
- **Top Disbursement** — proyek dengan realisasi terbesar, mengikuti filter
- Tabel ringkasan + indikator eksekutif (status On Track / Warning / Critical)
- Mobile friendly, auto-refresh tiap 5 menit

## Cara upload ke GitHub Pages
1. Buat repository baru di GitHub.
2. Upload file **`index.html`** (cukup satu file ini — logo sudah tertanam).
3. **Settings → Pages → Source: `main` / root → Save.**
4. Tunggu ±1 menit → situs aktif di `https://<username>.github.io/<repo>/`.

## Mengganti / mengedit
- **Update angka:** cukup ubah isi Google Sheets — dashboard ikut berubah otomatis.
- **Ubah tampilan/fitur:** edit `index.html`, lalu upload ulang (timpa file lama) → Commit.
- Semua pengaturan ada di objek **`CONFIG`** di dalam `<script>` (URL sheet, nama kolom,
  kategori, warna, interval refresh).

---
Created by : **Samuel Guhan**
