# 11 - Membuat Form pada HTML

## PENDAHULUAN

Selamat datang dalam tutorial singkat mengenai pembuatan formulir (form) pada HTML. Formulir ini bertujuan untuk mengumpulkan data atau informasi dari pengunjung (client) web, mirip dengan formulir di dunia nyata. Dengan formulir web, pengguna dapat mengisi informasi yang akan diolah oleh program tertentu.

## Cara Mudah Membuat Form pada HTML

Pada HTML, pembuatan formulir dapat dilakukan dengan menggunakan tag `<form>`. Tag ini memiliki dua atribut utama yang perlu diperhatikan:

1. **`method`**: Menentukan cara pengiriman data. Metode yang umum digunakan adalah "GET" atau "POST".

2. **`action`**: Menentukan tindakan yang akan diambil saat data formulir dikirim. Tindakan ini bisa berupa URL atau alamat file yang akan memproses data.
   **CATATAN: Isilah atribut `action` dengan alamat URL dari endpoint yang akan memproses formulir.**

   **Contoh:**
   ```html
   <form action="proses_form.php" method="POST">
       <!-- Tempat untuk menambahkan elemen formulir seperti input, textarea, dll. -->
   </form>
   ```

   **Pada contoh di atas, kita menggunakan metode `"POST"` dan menentukan bahwa formulir akan diarahkan ke file `"proses_form.php"` saat data dikirim. Perlu diingat bahwa elemen formulir, seperti `input`, `textarea`, dan lainnya, bisa ditambahkan di antara tag `<form>` dan `</form>` sesuai kebutuhan.**
   
**CATATAN: Kode HTML di atas tidak akan menghasilkan apa pun karena kita belum membuat `field` formulirnya.**

Apa itu `field`? `Field` adalah ruas yang dapat diisi dengan data.
Contoh:
```html
<input type="text" name="nama"/>
```
**Penjelasan dari contoh di atas:**
    1. `input` merupakan `tag` dari `field`.
    2. `type` adalah atribut `field` yang menentukan tipe data yang akan digunakan.
    3. `name` adalah atribut `field` yang mengunci variabel.

# Latihan Membuat Form Login

Dalam latihan membuat form login ini, Anda akan menggunakan beberapa field dan elemen sebagai berikut:

1. Field untuk input username atau email.
2. Field untuk input password.
3. Checkbox untuk remember me.
4. Tombol untuk login.

Untuk melihat hasil latihan tersebut, silakan klik tautan berikut [Form Login](/form.html).

```html
<form action="login.php" method="post">
    <fieldset>
        <legend>LOGIN</legend>
        <p>
            <label for="email">Email</label>
            <input type="text" id="email" name="email" placeholder="Email" />
        </p>
        <p>
            <label for="password">Password</label>
            <input type="password" id="password" name="password" placeholder="Password" />
        </p>
        <p>
            <label for="remember">Remember Me</label>
            <input type="checkbox" name="rememberme" id="remember" />
        </p>
        <input type="submit" value="Login">
    </fieldset>
</form>
```

**Penjelasan dari Latihan yang sudah dikerjakan:**
1. Kita mempunyai `title` pada `web` yaitu `Belajar HTML | Membuat Form Login`.
2. Kita juga mempunyai `<form action="login.php" method="post">` 
   yang berfungsi untuk Mendefinisikan formulir dengan aksi (action) yang mengarah ke `"login.php"` dan metode (method) `"post"`. Artinya, data formulir akan dikirimkan ke server menggunakan metode POST saat formulir disubmit.
3. `<fieldset>`: Ini adalah elemen untuk mengelompokkan elemen formulir menjadi satu kelompok dengan garis batas.
    Di dalamnya terdapat elemen-elemen yang akan dijelaskan di bawah:

    1. `<legend>LOGIN</legend>`: Menetapkan judul atau legenda untuk kelompok elemen formulir (fieldset).
    2. `<p>` : Elemen paragraf, digunakan untuk mengelompokkan elemen-elemen formulir dengan label dan input.
    3. `<label for="email">Email</label>`: Label untuk kolom input email,
        dengan atribut `"for"` yang sesuai dengan id elemen input.
    4. `<input type="text" id="email" name="email" placeholder="Email" />`:
        Kolom input teks untuk memasukkan alamat email dengan id "email" dan nama "email".
    5. Serupa dengan bagian `email`, ada juga bagian `password` dan `remember me`.
    6. `<input type="submit" value="Login">`: Tombol submit yang akan mengirimkan data formulir ke server.

    **Alur kerja:**
1. Pengguna membuka halaman web ini.
2. Melalui formulir, pengguna diminta untuk memasukkan `alamat email`, `password`, dan opsi `"Remember Me"`.
3. Ketika formulir disubmit (dengan mengklik tombol `"Login"`), 
   data formulir dikirimkan ke server ke file "login.php" menggunakan metode POST.