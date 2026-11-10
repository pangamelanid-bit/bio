# Halaman Link-in-Bio PAN Gamelan

Halaman Link-in-Bio mandiri berbasis HTML5 dan CSS modern untuk **PAN Gamelan**, dirancang sebagai pengganti layanan berbayar seperti Linktree. Sangat ringan (total unduhan halaman di browser modern sekitar **24 KB**), responsif untuk layar ponsel, dan dapat di-host gratis selamanya di **GitHub Pages**.

---

## Struktur File

- `index.html` — Halaman utama berisi profil, tombol WhatsApp (`0812-2596-6778`), katalog produk Mayar.id, kanal media sosial, dan tombol **Buat Beli Kopi**.
- `style.css` — Stylesheet murni menggunakan CSS Cascade Layers (`@layer`), variabel palet warna resmi PAN Gamelan (Navy Gamelan & Gold Gong), serta dukungan kontras tinggi WCAG AA.
- `logo.webp` & `logo.png` — Logo resmi PAN Gamelan teroptimasi (WebP 5 KB dengan fallback PNG).
- `images/` — Folder berisi 4 gambar thumbnail produk yang sudah dikompresi ke format WebP dan JPG (total hanya ~9 KB untuk keempat gambar WebP).

---

## Cara Memasang Gratis di GitHub Pages

1. Buat repositori publik baru di akun GitHub Anda (misalnya bernama `bio` atau `pan-gamelan-links`).
2. Unggah seluruh isi folder ini (`index.html`, `style.css`, `logo.webp`, `logo.png`, serta folder `images/`) ke direktori utama (*root*) repositori tersebut.
3. Buka menu **Settings** pada repositori GitHub Anda, lalu pilih menu **Pages** di bilah kiri.
4. Pada bagian **Build and deployment** > **Source**, pilih **Deploy from a branch**.
5. Pilih branch `main` (atau `master`), pilih folder `/ (root)`, lalu klik **Save**.
6. Tunggu sekitar 1 menit. Halaman Link-in-Bio Anda akan aktif di alamat:
   `https://<username-github-anda>.github.io/<nama-repositori>/`

---

## Catatan Pembayaran Wallet & Tombol "Buat Beli Kopi"

Karena GitHub Pages bersifat **statis** (tidak memiliki server backend untuk menyimpan kunci rahasia API *payment gateway* secara aman), penggunaan tautan produk **Mayar.id** (`https://pan-gamelan.myr.id/`) adalah solusi paling aman dan langsung:
- Pembeli dapat membayar melalui **QRIS, GoPay, OVO, Dana, ShopeePay, atau Virtual Account**, dan dana otomatis masuk ke saldo/rekening yang terhubung di akun Mayar Anda.
- Untuk tombol **Buat Beli Kopi**, saat ini diarahkan ke `https://pan-gamelan.myr.id/`. Jika Anda membuat halaman khusus *Tip / Traktir* di dashboard Mayar.id (menu **Payment Link / Donasi**), Anda cukup mengganti atribut `href` pada bagian `link-card-coffee` di `index.html` dengan URL Payment Link tersebut.
