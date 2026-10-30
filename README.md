# Kanvas Eksperimen — Travel Umrah

Versi web dari "Kanvas Eksperimen" (Ash Maurya, lisensi CC BY-SA 4.0), diisi untuk studi Travel Umrah.

**Live:** https://coach-edtech.github.io/kanvas-eksperimen/

## Cara update

Repo ini adalah sumber kebenaran. Edit `index.html` di repo ini, lalu:

```bash
git add -A && git commit -m "deskripsi perubahan" && git push
```

GitHub Pages deploy otomatis ~30 detik setelah push.

Salinan kerja lokal: `~/workspace/kanvas-eksperimen/`

## Catatan teknis

- Kanvas fixed 1920×1358 px. Di layar, ukurannya otomatis diskalakan agar muat lebar viewport (`--fit` CSS var, tanpa library). `@media print` tetap memakai skala A4 landscape sendiri.
- Font Oswald + Barlow dimuat dari Google Fonts (CDN). Kalau file `fonts/*.woff2` lokal tersedia, ganti blok `@font-face` dan hapus `<link>` Google Fonts untuk hosting fully self-contained/offline.
- Preview lokal: buka `index.html` langsung di browser (double-click), atau `python3 -m http.server` di folder ini.
