# YouTube Deposit Box

Local-first dashboard untuk mengelola dan memonitor channel YouTube.

## Fitur

- IndexedDB untuk data channel lokal
- YouTube Data API v3 untuk nama channel, handle, logo, subscribers, views, total video, dan channel keywords
- Subscriber Change dan View Change berdasarkan snapshot sync sebelumnya
- Filter status dan monetisasi
- Backup/Restore JSON
- PWA (manifest + service worker + icons)
- Responsive mobile/desktop

## Deploy ke Vercel

1. Upload seluruh isi repository ini ke GitHub.
2. Import repository di Vercel.
3. Framework Preset: **Other**.
4. Build Command: kosong.
5. Output Directory: kosong.
6. Deploy.

## YouTube API

Buka **API Settings** di aplikasi, masukkan YouTube Data API v3 key, lalu gunakan **Sync** atau **Sync All**.

> Data akun/password disimpan di browser pengguna. Jangan gunakan perangkat publik atau profil browser bersama.

## Historical statistics

Subscriber and view changes use dated local snapshots stored per channel in IndexedDB. Each calendar day keeps one snapshot; repeated Sync actions on the same day update that day's snapshot instead of changing the baseline. The dashboard supports **Daily**, **7 Days**, and **30 Days** comparison periods. Positive changes are green, negative changes are red, and zero/no-baseline changes are neutral.
