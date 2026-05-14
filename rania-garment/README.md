# Rania Garment - Landing Page Static HTML

Landing page company profile **Rania Garment (CV. Rania Jaya Mulya)** dalam bentuk single-file HTML + Tailwind CSS (CDN).

## Isi Folder
- `index.html` — file utama landing page (sudah include semua section)
- `assets/logo.png` — logo CJM CV. Rania Jaya Mulya (lokal, tidak via CDN)
- `robots.txt` — untuk SEO
- `sitemap.xml` — untuk SEO

> **Catatan**: Foto produk, hero, dan about masih dari Unsplash (CDN eksternal) supaya ZIP tetap ringan. Bila ingin foto lokal, simpan ke `assets/` lalu ganti URL `https://images.unsplash.com/...` di `index.html` dengan `assets/nama-foto.jpg`.

## Cara Pakai

### 1. Test Lokal
Cukup buka `index.html` di browser (double-click). Tidak perlu install apapun.

### 2. Deploy ke Hosting Gratis

**Netlify (paling mudah):**
1. Buka https://app.netlify.com → Sign up gratis
2. Drag-and-drop folder `rania-garment-static` ke halaman Netlify
3. Selesai, langsung dapat URL `https://nama-acak.netlify.app`
4. (Opsional) Custom domain raniagarment.com via Settings → Domain

**Vercel:**
1. https://vercel.com → New Project → Upload folder
2. Deploy

**cPanel / shared hosting:**
1. Upload semua file ke folder `public_html` via File Manager / FTP
2. Selesai

## Aktivasi Form Kontak (PENTING!)
Form pakai **FormSubmit.co** (gratis, tanpa daftar).

**Langkah aktivasi (sekali saja):**
1. Setelah deploy, isi form di website lalu klik **Kirim Pesan**
2. Buka inbox email `info@raniagarment.com`
3. Akan ada email dari **FormSubmit** dengan link konfirmasi → KLIK link tsb
4. Setelah itu semua form submission selanjutnya otomatis masuk ke email Anda

> Bila ingin pakai EmailJS atau Formspree (alternatif), edit `<form action="...">` di `index.html` dengan endpoint masing-masing.

## Edit Konten
Semua teks ada di `index.html` — buka pakai text editor (Notepad++, VS Code, dll), Ctrl+F cari teks yang mau diubah, save.

**Nomor WhatsApp** ada di banyak tempat, gunakan Find & Replace:
- Cari: `6282125400565` → ganti nomor baru
- Cari: `082125400565` → ganti tampilan

**Email**: cari `info@raniagarment.com` → ganti semua

## Customisasi Cepat
- **Warna merah utama**: cari `#DC2626` (ganti ke warna brand baru)
- **Logo**: ganti URL logo di line ~80 dan ~footer
- **Foto produk**: ganti URL Unsplash di tiap product card

## Catatan
- Tailwind via CDN — ringan, langsung jalan, tapi untuk produksi disarankan compile via Tailwind CLI bila butuh ukuran file lebih kecil
- Semua icon pakai Font Awesome 6 (CDN)
- Font: Playfair Display (heading) + Inter (body) via Google Fonts
