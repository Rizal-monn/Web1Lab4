# Lab4Web - Praktikum 4: CSS Layout

Mata kuliah Pemrograman Web - Universitas Pelita Bangsa

## Struktur Folder
```
Lab4Web/
├── README.md
├── lab4_box/
│   └── lab4_box.html          (Box Element, Float, Clearfix)
└── lab4_layout/
    ├── home.html              (Layout Web Sederhana)
    ├── artikel.html
    ├── about.html             (Tugas 1)
    ├── kontak.html            (Tugas 2)
    └── style.css
```

## Bagian 1 - Box Element, Float & Clearfix (`lab4_box.html`)
1. Membuat dokumen HTML dengan `<header>` berisi `<h1>Box Element</h1>`.
2. Menambahkan tiga `div` (`div1`, `div2`, `div3`) di dalam `<section>`.
3. Menambahkan CSS `float:left` dan `padding:10px` sehingga ketiga kotak berjajar ke samping.
4. Menambahkan `div4` dengan `clear:left; float:none;` sehingga turun ke bawah element float.
5. Eksperimen `clear`: `left` / `right` / `both` / `none` (lihat jawaban di bawah).

> Screenshot: (tempel hasil browser di sini - Gambar 4.5 dan 4.6)

## Bagian 2 - Layout Web Sederhana (`lab4_layout`)
| Langkah | Penjelasan |
|---|---|
| Struktur dasar | `home.html` + `style.css`; isi dibungkus `<div id="container">` |
| Kerangka semantic | `<header>`, `<nav>`, `<section id="hero">`, `<section id="wrapper">` (berisi `#main` & `<aside id="sidebar">`), `<footer>` |
| CSS dasar | Import Google Font, reset `margin/padding`, `#container` lebar 980px & `margin:0 auto` (rata tengah) |
| Header | `padding:20px`, judul abu-abu |
| Navigasi | `<a>` dijadikan `inline-block` agar bisa diberi padding; `.active` & `:hover` mengubah warna |
| Hero panel | Background abu-abu, tombol "Learn more" |
| Main & sidebar | `float:left`; lebar 640px + 260px + padding 2x20px masing-masing = 980px |
| Sidebar widget | `.widget-box` berisi judul biru dan daftar link |
| Footer | `clear:both` agar berada di bawah kedua kolom float |
| Content box | 3 kolom `width:33.33%` + `float:left` + `box-sizing:border-box` |
| Artikel | `.entry` dengan gambar `float:left` / `.right-img` `float:right` |
| Clearfix | `.row:after, .entry:after { content:''; display:table; clear:both; }` |

> Screenshot: (tempel Gambar 4.9 - 4.16)

## Tugas
1. **About** (`about.html`): single layout (tanpa sidebar) berisi deskripsi, keahlian, dan portfolio.
2. **Kontak** (`kontak.html`): form nama, email, telepon, subjek, message, tombol kirim & reset.

> Screenshot: (tempel hasil about.html dan kontak.html)