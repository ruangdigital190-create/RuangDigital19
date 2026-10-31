# RUANGDIGITAL190 — Website Satu File

Website katalog digital RUANGDIGITAL190 dibuat dengan HTML, CSS, dan JavaScript vanilla.

## File website

- `index.html` — seluruh website beserta semua logo/gambar sudah tertanam di dalam satu file.
- Tidak membutuhkan folder `assets`, gambar terpisah, framework, atau database.

## Isi katalog

- 10 aplikasi: Netflix, Spotify, YouTube Premium, CapCut, Alight Motion, Canva, ChatGPT, Gemini, Grammarly, dan QuillBot.
- Mobile Legends: 25 pilihan nominal Diamond.
- Free Fire: 20 pilihan nominal Diamond serta Membership Mingguan, BP Card, dan Membership Bulanan.

## Fitur

- Logo toko dan logo produk tertanam langsung di `index.html`.
- Pencarian produk dan filter kategori.
- Logo berjalan yang dapat diklik.
- Modal detail paket dan harga.
- Tombol WhatsApp dengan pesan pesanan otomatis.
- Tombol WhatsApp mengambang yang dapat digeser.
- Tidak ada keranjang atau checkout.
- Tampilan responsif untuk ponsel, tablet, dan desktop.

## Pengaturan toko

Buka `index.html`, lalu cari bagian `STORE_CONFIG` di dalam JavaScript.

```js
const STORE_CONFIG = {
  storeName: "RUANGDIGITAL190",
  whatsappNumber: "6285725423328",
  // ...
};
```

Nomor WhatsApp ditulis dengan format internasional tanpa tanda `+`, spasi, atau tanda hubung.

## Mengubah harga dan stok

Cari bagian `PRODUCTS` di dalam `index.html`.

- `title`, `description`, `short`, dan `info`: informasi produk.
- `variants`: pilihan paket.
- `price`: angka rupiah tanpa titik, misalnya `45000`.
- `price: null`: harga belum tersedia dan akan ditampilkan sebagai “Hubungi Admin”.
- `stock`: `available`, `limited`, `out_of_stock`, atau `confirm`.
- Diskon hanya tampil jika `discountEnabled: true`, `originalPrice` terisi, dan `price` lebih rendah daripada `originalPrice`.

Website bersifat statis. Perubahan harga atau stok harus disimpan lalu diunggah kembali ke GitHub agar tampil bagi semua pengunjung.

## Deploy ke GitHub Pages

1. Buat repository baru di GitHub.
2. Unggah `index.html` ke folder utama repository.
3. Buka **Settings → Pages**.
4. Pada bagian **Build and deployment**, pilih **Deploy from a branch**.
5. Pilih branch `main` dan folder `/ (root)`, lalu klik **Save**.
6. Tunggu proses deployment selesai dan buka alamat GitHub Pages yang diberikan.

**Penting:** Untuk versi satu file ini, cukup unggah `index.html`. Semua logo sudah disematkan di dalamnya.

## Catatan

Logo produk merupakan milik masing-masing pemegang merek dan ditampilkan untuk mengidentifikasi produk. Penayangan logo tidak menyatakan afiliasi atau dukungan resmi. Harga dan stok dapat berubah; konfirmasikan kepada admin sebelum pembayaran.
