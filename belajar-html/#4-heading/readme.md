# 04: HEADING

`Heading` merupakan judul yang umumnya diberikan pada sebuah halaman atau bagian artikel. Pada HTML, judul dapat dimulai dengan tag `<h1>` hingga `<h6>`. Setiap judul akan ditampilkan dengan ukuran teks yang berbeda, dimulai dari `<h1>` sebagai yang terbesar hingga `<h6>` sebagai yang terkecil. 

Contoh penggunaan:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>Ini adalah judul 1</h1>
    <h2>Ini adalah judul 2</h2>
    <h3>Ini adalah judul 3</h3>
    <h4>Ini adalah judul 4</h4>
    <h5>Ini adalah judul 5</h5>
    <h6>Ini adalah judul 6</h6>
</body>
</html>
```
**Hasil kode diatas**
<body>
    <h1>Ini adalah judul 1</h1>
    <h2>Ini adalah judul 2</h2>
    <h3>Ini adalah judul 3</h3>
    <h4>Ini adalah judul 4</h4>
    <h5>Ini adalah judul 5</h5>
    <h6>Ini adalah judul 6</h6>
</body>

**NB:**
- Tag `<h1>` umumnya digunakan untuk judul artikel, sedangkan tag `<h2>`, `<h3>`, `<h4>`, `<h5>`, dan `<h6>` digunakan untuk sub judul atau sub-heading.

Contoh penggunaan pada artikel:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Tutorial Heading di HTML</title>
</head>
<body>
    <h1>Belajar Heading di HTML</h1>
    <p>
      Terdapat enam tingkatan Heading di HTML, yaitu H1, H2, H3, H4, H5, dan H6.
      Heading berfungsi sebagai judul untuk artikel dan sub judul pada bagian artikel.
    </p>
    <h2>Membuat Sub Judul</h2>
    <p>
      Sub judul dimulai dengan tag H2 dan diikuti oleh tag H3 sampai H6. 
      Tag H1 hanya digunakan untuk judul artikel.
    </p>
</body>
</html>
```
**Hasil kode diatas**
<body>
    <h1>Belajar Heading di HTML</h1>
    <p>
      Terdapat enam tingkatan Heading di HTML, yaitu H1, H2, H3, H4, H5, dan H6.
      Heading berfungsi sebagai judul untuk artikel dan sub judul pada bagian artikel.
    </p>
    <h2>Membuat Sub Judul</h2>
    <p>
      Sub judul dimulai dengan tag H2 dan diikuti oleh tag H3 sampai H6. 
      Tag H1 hanya digunakan untuk judul artikel.
    </p>
</body>

# Perbedaan Heading dengan Title dan Header
Meskipun semuanya digunakan untuk judul, ada perbedaan di antara ketiganya:

- `Heading` adalah judul untuk artikel dan bagian artikel yang dibuat dengan tag `<h1>` sampai `<h6>`.
- `Title` adalah judul dari halaman web yang dibuat dengan tag `<title>`.
- `Header` adalah bagian kepala (kop) pada halaman web yang dibuat dengan tag `<header>`.