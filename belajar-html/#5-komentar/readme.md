# 05: Komentar dalam Kode HTML

## Pendahuluan
`Komentar` merupakan elemen pada `HTML` yang diabaikan oleh browser dan tidak ditampilkan pada web. Meskipun demikian, `Komentar` sangat penting untuk memberikan informasi tambahan mengenai kode `HTML`. Dalam panduan ini, akan dijelaskan cara membuat `Komentar` serta berbagai fungsi pentingnya dalam pengembangan web.

## Cara Membuat Komentar
Ada dua cara umum untuk membuat `Komentar` dalam `HTML`:

1. `<!---->`: Komentar dalam bentuk ini memiliki sintaks yang umum digunakan untuk memberikan penjelasan pada bagian tertentu dalam kode.

2. Shortcut `Ctrl + /`: `Tekan Ctrl + /` pada keyboard untuk secara cepat membuat `komentar`. Meskipun hasilnya sama dengan cara pertama, penggunaan shortcut dapat meningkatkan efisiensi.

## Fungsi Komentar dalam Kode HTML
1. **Menjelaskan Arti Tag**
   Komentar dapat digunakan untuk memberikan penjelasan atas arti sebuah `tag`, memudahkan pembacaan dan pemahaman kode.
   ```html
   <!DOCTYPE html> <!-- Ini adalah tag pembuka HTML -->
   </html> <!-- Ini adalah tag penutup HTML -->
   ```

2. **Menyimpan Todo List**
   Komentar dapat berfungsi sebagai catatan untuk menyimpan `todo list`, memberikan panduan pada bagian kode tertentu yang memerlukan perhatian.
   ```html
   <!DOCTYPE html>
   <html lang="en">
       <head>
           <meta charset="UTF-8">
           <meta name="viewport" content="width=device-width, initial-scale=1.0">
           <title>Document</title>
       </head>
       <body>
           <!-- TODO: Menambahkan fitur Dropdown -->
           <div class="dropdown">

           </div>
       </body>
   </html>
   ```

3. **Menonaktifkan Code**
   Komentar dapat digunakan untuk menonaktifkan sebagian kode tanpa menghapusnya secara permanen, memungkinkan eksperimen atau debugging.
   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Document</title>
   </head>
   <body>
       <!-- <div class="dropdown">
       </div> -->
   </body>
   </html>
   ```

## Kesimpulan
Penggunaan `Komentar` dalam `HTML` membantu menjelaskan kode, menyimpan catatan, dan memberikan fleksibilitas dalam pengelolaan proyek pengembangan web. Selalu gunakan dengan bijak untuk meningkatkan kolaborasi dan pemahaman tim pengembang.