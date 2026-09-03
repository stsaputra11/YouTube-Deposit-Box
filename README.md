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


## UI settings update
API Settings is accessed from the gear icon in the sticky header. Backup JSON and Restore JSON are available inside API Settings under Data Management.
