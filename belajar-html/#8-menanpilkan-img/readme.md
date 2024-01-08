# 08 - Menampilkan Gambar pada HTML

Untuk mempercantik halaman HTML Anda dengan gambar, dapatkan wawasan mendalam tentang penggunaan tag `<img>` dan tambahan tag khusus pada HTML versi 5.

## Penggunaan Tag `<img>`:

Gunakan tag `<img>` untuk menampilkan gambar dengan atribut `src` yang menunjukkan lokasi file gambar dan atribut `alt` untuk memberikan deskripsi gambar. Berikut adalah format file gambar yang sering digunakan dalam web:

| Nama Format | Nama Panjang                                       | Ekstensi                                |
|-------------|----------------------------------------------------|-----------------------------------------|
| APNG        | Animated Portable Network Graphics                 | .apng                                   |
| GIF         | Graphics Interchange Format                        | .gif                                    |
| ICO         | Microsoft Icon                                     | .ico, .cur                              |
| JPEG        | Joint Photographic Expert Group image              | .jpg, .jpeg, .jfif, .pjpeg, .pjp        |
| PNG         | Portable Network Graphics                          | .png                                    |
| SVG         | Scalable Vector Graphics                           | .svg                                    |
| WebP        | Web Picture                                        | .webp                                   |

**Atribut untuk Tag `<img>`:**

Beberapa atribut yang sering digunakan:

- **alt:** Teks alternatif untuk gambar.
- **width:** Lebar gambar.
- **height:** Tinggi gambar.
- **style:** Style CSS untuk gambar.

## Panduan Penggunaan:

### 1. Gambar di Folder yang Sama:

```html
<img src="nama-file-gambar.jpg" alt="Deskripsi gambar" width="300" height="200" style="border: 1px solid #ccc;">
```

### 2. Gambar di Folder yang Berbeda (1 Tingkat):

```html
<img src="images/nama-file-gambar.jpg" alt="Deskripsi gambar" width="300" height="200" style="border: 1px solid #ccc;">
```

### 3. Gambar di Folder yang Berbeda (2 Tingkat):

```html
<img src="../images/myfolder/nama-file-gambar.jpg" alt="Deskripsi gambar" width="300" height="200" style="border: 1px solid #ccc;">
```

### 4. Gambar di Folder yang Berbeda (3 Tingkat):

```html
<img src="../../images/myfolder/subfolder/nama-file-gambar.jpg" alt="Deskripsi gambar" width="300" height="200" style="border: 1px solid #ccc;">
```

### 5. Mengambil Gambar dari Internet:

```html
<img src="https://www.contohwebsite.com/path/ke/gambar/nama-file-gambar.jpg" alt="Deskripsi gambar" width="300" height="200" style="border: 1px solid #ccc;">
```

## Tag Tambahan untuk Gambar di HTML:

### 1. `<figure>` Tag:

Membungkus gambar dengan elemen terkait seperti teks caption atau keterangan.

```html
<figure>
  <img src="gambar.jpg" alt="Deskripsi gambar">
  <figcaption>Keterangan gambar</figcaption>
</figure>
```

### 2. `<picture>` Tag:

Menangani variasi gambar berdasarkan ukuran layar atau resolusi yang berbeda.

```html
<picture>
  <source media="(min-width: 768px)" srcset="gambar-large.jpg">
  <source media="(min-width: 480px)" srcset="gambar-medium.jpg">
  <img src="gambar-small.jpg" alt="Deskripsi gambar">
</picture>
```

Dengan panduan ini, tampilkan gambar dengan atraktif dan profesional sesuai lokasi dan kebutuhan desain halaman HTML Anda.