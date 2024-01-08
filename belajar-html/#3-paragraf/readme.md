# 03 PARAGRAF

`Paragraf` adalah kumpulan kalimat yang biasanya digunakan pada web untuk menampilkan artikel atau teks tertentu. Dalam `HTML`, `Paragraf` dimulai dengan tag `<p>`. Selain itu, terdapat beberapa tag pendukung seperti:

------------------------------------------------------------------------------------------------------------
|  TAG  |   FUNGSI                                                                                          |     
| ----- | ------------------------------------------------------------------------------------------------- |
|  div  | membuat blok dalam dokumen HTML, sering digunakan bersama dengan atribut `class` atau `id`      |
|  hr   | digunakan untuk membuat garis horizontal atau pemisah di dalam dokumen                            |
|  br   | digunakan untuk membuat jeda baris atau "line break"                                              |
| pre   | digunakan untuk menampilkan teks dengan format yang dipertahankan, termasuk spasi dan baris baru  |
-------------------------------------------------------------------------------------------------------------

* Contoh penggunaannya:

1. **\<div> (Division):**
   ```html
   <div class="container">
       <!-- Konten di dalam div -->
   </div>
   ```

2. **\<hr> (Horizontal Rule):**
   ```html
   <p>Paragraf pertama</p>
   <hr>
   <p>Paragraf kedua setelah garis horizontal</p>
   ```

3. **\<br> (Line Break):**
   ```html
   <p>Satu baris teks <br> baris teks baru</p>
   ```

4. **\<pre> (Preformatted Text):**
   ```html
   <pre>
       Ini adalah teks
       dengan format
       yang dipertahankan.
   </pre>
   ```