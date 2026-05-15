# 🚀 Ilham OS — Panduan Deploy

## File yang kamu butuhkan (semua ada di folder ini):
```
index.html        ← app utama
manifest.json     ← konfigurasi PWA
sw.js             ← service worker (offline support)
icon-192.png      ← generate dulu pakai generate-icons.html
icon-512.png      ← generate dulu pakai generate-icons.html
```

---

## LANGKAH 1 — Generate Icon (2 menit)

1. Buka file `generate-icons.html` di browser
2. Klik "Download icon-192.png" → simpan di folder ini
3. Klik "Download icon-512.png" → simpan di folder ini

---

## LANGKAH 2 — Deploy ke Vercel (3 menit)

1. Buka **vercel.com** → Sign Up gratis (pakai Google/GitHub)
2. Di dashboard, klik **"Add New → Project"**
3. Pilih **"Deploy without Git"** → drag & drop **seluruh folder** ini
4. Tunggu ~30 detik → dapat URL seperti `ilham-os.vercel.app`
5. ✅ Bisa dibuka di laptop kapanpun!

**Custom domain gratis** (opsional):
- Di Vercel dashboard → Settings → Domains
- Ketik nama yang kamu mau, misal `ilham.vercel.app`

---

## LANGKAH 3 — Install di iPhone (2 menit)

1. Buka URL Vercel kamu di **Safari** iPhone (harus Safari, bukan Chrome)
2. Tap tombol **Share** (kotak dengan panah atas) di bawah layar
3. Scroll ke bawah → tap **"Add to Home Screen"**
4. Ketik nama: **Ilham OS** → tap **Add**
5. ✅ Icon muncul di home screen, buka seperti app biasa!

> **Catatan iPhone:**
> - Berjalan fullscreen tanpa browser bar
> - Data tersimpan di iPhone (localStorage)
> - Bisa pakai offline setelah pertama kali dibuka
> - Notifikasi perlu izin saat pertama buka

---

## LANGKAH 4 — Setup AI (Asri)

AI sudah terhubung ke Claude API. Untuk mengaktifkan:
- Pastikan kamu punya Anthropic API key
- Atau biarkan saja — chat bar tetap muncul, kalau API belum diset akan error tapi app tetap berjalan normal

---

## FAQ

**Q: Data di iPhone vs laptop sama?**
A: Belum — data tersimpan lokal di masing-masing device. Kalau mau sync, perlu tambah Supabase (bisa dikerjakan nanti).

**Q: Apakah gratis selamanya?**
A: Vercel gratis untuk personal project. Tidak ada batas waktu.

**Q: Bisa update app?**
A: Upload ulang file ke Vercel → otomatis update. iPhone refresh otomatis saat ada koneksi.

**Q: Kalau mau ganti nama domain?**
A: Di Vercel Settings → Domains, bisa set custom domain sendiri atau pakai subdomain Vercel gratis.
