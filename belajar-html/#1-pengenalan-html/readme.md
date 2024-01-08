# 01: PENGANTAR HTML

## Ikhtisar
Selamat datang di dunia HTML, singkatan dari Hypertext Markup Language. HTML berfungsi sebagai batu bata dasar dalam membangun struktur sebuah situs web.

## Latar Belakang Sejarah
HTML pertama kali diperkenalkan pada tahun 1980 oleh Tim Berners-Lee selama masa kerjanya di CERN. Pada tahun 1991, beliau menerbitkan dokumen berjudul "HTML-tags," yang menjelaskan 18 tag awal yang membentuk konsep dasar HTML.

## Dasar dalam SGML
HTML dirancang berdasarkan prinsip-prinsip dari Standard Generalized Markup Language (SGML). SGML, standar internasional untuk membuat dokumen yang ditandai, mencakup berbagai elemen markup seperti paragraf, daftar, dan judul.

## POIN-POIN UTAMA

1. **Dasar SGML HTML:** HTML berfungsi sebagai implementasi dari SGML, mewarisi kemampuan markup yang kuat.

2. **Kelanjutan Tag SGML di HTML:** Beberapa tag dari SGML tetap ada di HTML, termasuk:
    1. `<title></title>`
    2. `<p></p>`
    3. `<li></li>`
    4. `<h1></h1>` hingga `<h6></h6>`

## STRUKTUR HTML5

HTML5 memperkenalkan struktur yang disederhanakan dan ditingkatkan dibanding pendahulunya. Berikut adalah struktur dasar dari dokumen HTML5:

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dokumen</title>
</head>
<body>
    <!-- Isi konten Anda disini -->
</body>
</html>
```

### Penjelasan:

- `<!DOCTYPE html>`: Mendeklarasikan versi HTML sebagai HTML5, memastikan kompatibilitas dengan browser modern.

- `<html lang="id">`: Elemen utama dari dokumen HTML. Atribut `lang` menentukan bahasa dokumen (dalam hal ini, bahasa Indonesia).

- `<head>`: Berisi meta-informasi tentang dokumen HTML, seperti set karakter, pengaturan viewport, dan judul dokumen.

- `<meta charset="UTF-8">`: Menentukan pengkodean karakter untuk dokumen (UTF-8 dalam hal ini).

- `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Mengatur properti viewport, memastikan tampilan yang tepat pada berbagai perangkat.

- `<title>Dokumen</title>`: Mendefinisikan judul dokumen HTML, yang muncul di bilah judul atau tab browser.

- `<body>`: Berisi konten dokumen HTML, seperti teks, gambar, tautan, dll.

Silakan tambahkan konten Anda di antara tag `<body>` untuk membuat dokumen HTML5 yang sepenuhnya fungsional. Happy coding!