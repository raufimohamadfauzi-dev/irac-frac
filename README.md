# IRAC + FRAC Timun

Pencari bahan aktif berdasarkan hama/penyakit mentimun. UI sengaja sederhana: **cari sasaran → lihat bahan aktif → lihat kode IRAC/FRAC**.

## Status dataset awal
- Hama: thrips, kutu kebul, aphid, tungau, pengorok daun, ulat, oteng/kumbang daun, lalat buah.
- Penyakit: embun bulu, embun tepung, antraknosa, Alternaria, gummy stem blight, Pythium/Phytophthora, bercak bakteri, Fusarium, virus.
- Setiap relasi diberi scope bukti.
- `Indonesia ✓` hanya dipakai bila ada bukti publik produk/label Indonesia untuk mentimun + sasaran terkait.

## Menjalankan
Karena data dipisah sebagai JSON, jalankan lewat HTTP server atau GitHub Pages.

```bash
python -m http.server 8000
```

Lalu buka `http://localhost:8000`.

## Sumber dasar
Lihat `data/sources.json`. Klasifikasi utama menggunakan IRAC MoA v11.5 (Feb 2026) dan FRAC Code List 2026.

## Catatan
Database ini adalah alat pencarian/referensi, bukan label pestisida. Dosis, PHI, jumlah aplikasi dan legalitas penggunaan harus mengikuti label produk aktual di Indonesia.
