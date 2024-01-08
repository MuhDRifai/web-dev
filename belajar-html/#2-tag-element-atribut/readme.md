# 02 - TAG, ELEMENT, ATRIBUT

## Pendahuluan
`Tag`, `Element`, dan `Atribut` merupakan tiga komponen kunci dalam pemrograman `HTML`. Memahami perbedaan dan penggunaan mereka secara tepat adalah langkah awal menuju pembuatan halaman web yang efisien dan terstruktur.

### Tag
`Tag` adalah penanda awal dan akhir dari sebuah `Element` dalam `HTML`, dibuat dengan kurung siku `<>`. Secara umum, tag selalu dituliskan secara berpasangan, seperti `<p></p>`, `<a></a>`, `<table></table>`. Namun, beberapa tag bersifat tidak berpasangan, misalnya `<img src="" alt="" />`.

### Element
`Element` adalah struktur dasar dalam `HTML` yang terdiri dari `tag pembuka`, `isi`, dan `tag penutup`. Sebagai contoh:
```html
<p align="center">Hello World!</p>
```
- `<p align="center">` merupakan `tag pembuka`.
- `Hello World!` merupakan `isi tag`.
- `</p>` adalah `tag penutup`.

### Atribut
`Atribut` adalah kata kunci khusus yang ditempatkan pada `tag pembuka` dan memengaruhi perilaku dari `element`. Contoh penggunaan atribut:
```html
<a href="https:/www.google.com">GOOGLE</a>
```

## Jenis-Jenis Atribut

### 1. Atribut Global
Atribut global dapat ditambahkan ke semua elemen `HTML`. Berikut adalah beberapa contoh atribut global dan fungsinya:

| Nama Atribut    |               Deskripsi atau Fungsi                                         |
| --------------- | ----------------------------------------------------------------------------|
| accesskey       | Menentukan tombol pintas untuk mengaktifkan elemen                          |
| class           | Menentukan class CSS yang akan digunakan                                    |
| contenteditable | Menentukan apakah isi elemen bisa diedit atau tidak                         |
| data-*          | Digunakan untuk menyimpan data                                              |
| dir             | Menentukan arah teks dari elemen (kiri ke kanan atau sebaliknya)            |
| draggable       | Menentukan apakah elemen dapat di-drag atau tidak                           |
| hidden          | Untuk menyembunyikan elemen                                                 |
| id              | Menentukan id unik untuk elemen                                             |
| lang            | Menentukan bahasa yang digunakan untuk isi elemen                           |
| spellcheck      | Menentukan apakah isi elemen harus dilakukan pengejaan grammar atau tidak   |
| style           | Menentukan CSS inline untuk elemen                                          |
| tabindex        | Menentukan urutan atau indeks tab dari elemen (saat tombol tab ditekan)     |
| title           | Menentukan informasi tambahan tentang elemen                                |
| translate       | Menentukan apakah konten dari elemen dapat diterjemahkan atau tidak         |
|-----------------------------------------------------------------------------------------------|

### 2. Atribut Event
Atribut event digunakan untuk menentukan aksi yang akan dilakukan saat terjadi suatu peristiwa pada elemen. Atribut ini umumnya digunakan dalam pemrograman JavaScript. Berikut adalah beberapa contoh atribut event pada jendela browser:

| Nama atribut     |      Nilai           |                  Fungsi                           |
| ---------------  | -------------------- | ------------------------------------------------- |
| onafterprint     | Kode JavaScript      | Setelah dokumen dicetak                           |
| onbeforeprint    | Kode JavaScript      | Sebelum dokumen dicetak                           |
| onbeforeunload   | Kode JavaScript      | Sebelum saat dokumen tidak ter-load               |
| onerror          | Kode JavaScript      | Saat terjadi error                                |
| onhashchange     | Kode JavaScript      | Saat terjadi perubahan pada bagian anchor di URL  |
| onload           | Kode JavaScript      | Setelah loading selesai                           |
| onmessage        | Kode JavaScript      | Saat ada pesan                                    |
| onoffline        | Kode JavaScript      | Saat tiba-tiba offline                            |
| ononline         | Kode JavaScript      | Saat tiba-tiba online                             |
| onpagehide       | Kode JavaScript      | Saat pengguna tidak sedang membuka halaman web    |
| onpageshow       | Kode JavaScript      | Saat pengguna membuka kembali halaman web         |
| onpopstate       | Kode JavaScript      | Saat histori browser berubah                      |
| onresize         | Kode JavaScript      | Saat ukuran jendela browser berubah               |
| onstorage        | Kode JavaScript      | Saat area penyimpanan (Web Storage) di-update     |
| onunload         | Kode JavaScript      | Saat web browser ditutup                          |
|---------------------------------------------------------------------------------------------|

Selain atribut tersebut, masih banyak lagi atribut event lainnya. Semuanya dapat ditemukan di: [HTML Event Attributes](https://www.w3schools.com/tags/ref_eventattributes.asp).

### 3. Atribut Khusus
Atribut khusus hanya dapat digunakan pada elemen tertentu dan tidak selalu dapat digunakan pada elemen lain. Contoh:

| Nama atribut |        Bisa dipakai di tag                     |
| ------------ | ---------------------------------------------- |
| src          | `<audio>`, `<embed>`, `<iframe>`, `<img>`, dll |
| href         | `<a>`, `<link>`                                |
| action       | `<form>`                                       |
| autoplay     | `<audio>`, `<video>`                           |
| ------------------------------------------------------------- |

Dengan memahami konsep dasar dan jenis-jenis atribut dalam `HTML`, Anda dapat membuat halaman web yang lebih profesional dan efisien. Selamat belajar!