# YouTube Deposit Box

**Organize Channels in One Place**

Local-first dashboard untuk menyimpan profil channel YouTube, melakukan sinkronisasi statistik publik melalui YouTube Data API v3, melakukan backup/restore JSON, dan memantau status channel.

## Fitur

- IndexedDB sebagai penyimpanan utama lokal
- YouTube Data API v3 sync per channel dan Sync All
- Subscribers, Total Views, Views Change, Total Videos
- Nama channel dan logo channel dari API setelah sync
- Channel tags/keywords dari API jika tersedia
- Filter status dan monetisasi
- Overview total Channels, Aktif, Hiatus, Monetized Channels
- Backup dan Restore JSON
- API key disimpan lokal di browser
- Responsive layout
- PWA installable + offline app shell

## Deploy ke Vercel

1. Upload seluruh isi repository ini ke GitHub.
2. Import repository di Vercel.
3. Framework Preset: **Other** / static site.
4. Build command: kosong.
5. Output directory: kosong / root project.
6. Deploy.

## Menjalankan lokal

Karena service worker memerlukan HTTP/HTTPS, jangan membuka `index.html` langsung dengan `file://` jika ingin menguji PWA.

Contoh:

```bash
python -m http.server 8080
```

Lalu buka `http://localhost:8080`.

## YouTube API

Masukkan API key dari Google Cloud Console melalui **API Settings**. Aktifkan **YouTube Data API v3** pada project Google Cloud Anda.

## Data dan privasi

Data channel dan API key disimpan di browser pengguna. Backup JSON perlu dilakukan secara berkala jika data penting.
