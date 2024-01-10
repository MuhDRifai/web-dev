# Element Semantik

## PENDAHULUAN
`Element Semantik` merujuk pada elemen-elemen yang menyampaikan makna atau tujuan dalam sebuah dokumen. Elemen-elemen ini memiliki peran penting dalam struktur dan organisasi konten di web. Sebagai contoh, tag `<footer>` digunakan untuk membuat bagian kaki pada sebuah halaman web. Berikut adalah daftar elemen-elemen semantik yang telah dipilih:

---

| Elemen         | Penjelasan                                               |
| -------------- | -------------------------------------------------------- |
| `<article>`    | Digunakan untuk mendefinisikan elemen artikel.           |
| `<aside>`      | Menunjukkan bagian konten samping atau sidebar.          |
| `<details>`    | Membuat widget pengungkapan untuk detail tambahan.       |
| `<figcaption>` | Menyediakan keterangan untuk konten dalam `<figure>`.    |
| `<figure>`     | Mewakili konten yang dirujuk sebagai sebuah gambar.      |
| `<footer>`     | Mendefinisikan bagian kaki dari sebuah halaman web.      |
| `<header>`     | Menetapkan bagian kepala atau bagian atas halaman web.   |
| `<main>`       | Menunjukkan area konten utama dari dokumen.              |
| `<mark>`       | Mencetak atau menandai teks tertentu dalam dokumen.      |
| `<nav>`        | Menandai sebuah bagian navigasi dalam dokumen.           |
| `<section>`    | Mendefinisikan sebuah bagian dalam dokumen, seperti bab. |
| `<summary>`    | Memberikan ringkasan atau judul untuk elemen `<details>`.|
| `<time>`       | Mewakili periode waktu atau rentang waktu tertentu.      |

---
**Pastikan untuk menggunakan elemen-elemen semantik ini dengan tepat guna meningkatkan struktur dan makna dari dokumen HTML Anda.**

# Alasan Menggunakan Elemen Semantik

Salah satu alasan utama penggunaan elemen semantik adalah untuk membuat kode lebih mudah dipahami oleh manusia dan mesin. Sebagai contoh, penggunaan elemen semantik:
```html
 <div class="header"></div>
    <div class="section">
        <div class="article">
            <div class="figure">
                <img src="" alt="">
                <div class="figcaption"></div>
            </div>
        </div>
    </div>
    <div class="footer"></div>
```
# Membuat Layout dengan Elemen Semantik

Berikut adalah contoh implementasi layout dengan menggunakan elemen semantik. Untuk melihat contohnya, silakan kunjungi tautan berikut: [Contoh layout elemen semantik](semantik.html).

## Penjelasan Singkat tentang Contoh

Pada tautan di atas, kami menunjukkan penerapan elemen semantik dalam pembuatan tata letak web. Selain itu, kami menggunakan `CSS`, khususnya `CSS inline`. Penjelasan lebih lanjut dapat ditemukan di folder [belajar css](../belajar-css/).

Kembali ke topik, contoh penggunaan `CSS Inline` dapat ditemukan pada bagian berikut:

```html
<body style="background-color: aqua;">
```

Di sini, elemen `body` pada halaman web akan memiliki warna latar belakang `aqua`, karena kita menggunakan gaya (`style`) dengan properti `background-color`.