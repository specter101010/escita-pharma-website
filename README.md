# Escita Pharma — Corporate Website

Website profil perusahaan farmasi dengan katalog produk, informasi perusahaan, berita, peluang karier, dan halaman kontak. Dibangun sebagai aplikasi React dengan tampilan responsif, transisi halaman, serta navigasi yang mudah dijelajahi.

**Live website:** [escita-pharma.netlify.app](https://escita-pharma.netlify.app/)

![Escita Pharma](public/images/logo-full.png)

## Fitur

- Beranda dengan profil singkat, informasi perusahaan, dan lokasi.
- Halaman tentang perusahaan: sejarah, struktur operasional, tim, dan legalitas.
- Katalog produk dalam kategori obat bebas, obat resep etikal, dan obat generik berlogo, lengkap dengan pencarian berdasarkan nama, deskripsi, atau bentuk produk.
- Halaman berita, peluang karier, komunitas talenta, dan kontak.
- Animasi antarseksi serta perpindahan halaman dengan Framer Motion.
- Navigasi responsif untuk desktop dan perangkat seluler.

## Teknologi

| Kebutuhan | Teknologi |
| --- | --- |
| Antarmuka | React 18 |
| Build tool | Vite 5 |
| Styling | Tailwind CSS 3 |
| Navigasi | React Router DOM 6 |
| Animasi | Framer Motion 11 |
| Hosting demo | Netlify |

## Menjalankan secara lokal

Pastikan Node.js dan npm telah terpasang, kemudian jalankan:

```bash
git clone https://github.com/specter101010/kesehatan.git
cd kesehatan
npm install
npm run dev
```

Buka alamat lokal yang ditampilkan Vite di terminal, biasanya `http://localhost:5173`.

Perintah lain:

```bash
npm run build    # membuat hasil build di dist/
npm run preview  # meninjau hasil build secara lokal
```

## Struktur proyek

```text
public/               # gambar, video, ikon, dan aturan redirect Netlify
src/
  components/          # komponen layout dan UI yang digunakan ulang
  pages/               # beranda, tentang, produk, berita, karier, kontak
  App.jsx              # konfigurasi rute dan transisi halaman
  data.js              # data produk, tim, berita, dan informasi situs
  index.css            # gaya global dan konfigurasi tampilan
```

## Konten dan konfigurasi

- Perbarui data produk, tim, berita, kontak, dan tautan di `src/data.js`.
- Simpan aset visual di `public/images/` dan video beranda di `public/videos/`.
- Untuk deploy sebagai single-page application di Netlify, aturan fallback rute sudah tersedia di `public/_redirects`.

> **Status formulir:** Form kontak dan komunitas talenta saat ini hanya menampilkan pesan berhasil di sisi antarmuka. Data belum dikirim atau disimpan. Hubungkan handler `submit` di `src/pages/Contact.jsx` dan `src/pages/Careers.jsx` ke layanan formulir atau backend sebelum digunakan untuk menerima pesan dan data pelamar.

## Demo

Lihat hasilnya di **[Escita Pharma](https://escita-pharma.netlify.app/)**.
