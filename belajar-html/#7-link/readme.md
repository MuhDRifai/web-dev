# 07 - LINK/HYPERLINK

`Link` atau `Hyperlink` adalah elemen `HTML` yang berfungsi untuk `menghubungkan suatu halaman web ke halaman web yang lain`. Elemen ini memberikan interaktivitas pada pengguna, yang dapat `mengklik` dan membuka halaman lain sesuai dengan alamat URL yang diberikan. Selain berfungsi sebagai penghubung antar halaman, `link` juga memiliki kemampuan untuk melakukan tugas lain seperti `scroll top`, `download file`, `menjalankan fungsi JavaScript`, dan sebagainya.

## Cara Membuat Hyperlink

Untuk membuat `link`, kita dapat menggunakan tag `<a>`, yang kemudian harus memiliki atribut `href=""` untuk menentukan URL yang akan dituju. 
Penggunaannya: `<a href="url yang akan dituju">judul atau nama dari URL</a>`

# Jenis-Jenis LINK/HYPERLINK pada HTML

1. **Internal Link:** Link yang menuju ke domain atau halaman web itu sendiri. 
    ```html
    <a href="./link.html">Link.html merupakan file dari folder `#7-link`</a>
    ```

2. **External Link:** Link yang menuju domain lain. 
    ```html
    <a href="http://www.google.com">Ini merupakan website dari Google</a>
    ```
   **Catatan: Dengan menggunakan cara ini, kita dapat memberikan pengguna pengalaman yang lebih interaktif dan terhubung dengan konten eksternal atau fungsionalitas tambahan.**

# Fungsi Lainnya dari LINK

1. **Link Buntu:**
    Dalam membuat link buntu, kita dapat menyisipkan `#` di dalam `href=""`. Contoh:
    ```html
    <a href="#">Ini merupakan Link buntu</a>
    ```
    Pada contoh tersebut, kita mengisi URL-nya dengan tanda pagar. Tanda pagar pada URL adalah anchor (jangkar), yang akan membawa kita ke lokasi tertentu di dalam dokumen HTML. Jika hanya diisi pagar saja, maka ia tidak akan menuju ke lokasi manapun. Fungsi lain dari `Link Buntu` adalah digunakan sebagai `placeholder` atau sampel saja.

2. **Link Anchor:**
    `Link anchor` adalah link yang menuju ke suatu elemen tertentu. Cara membuat `link anchor` adalah dengan mengisi alamat URL dengan tanda pagar `(#)`, lalu diisi dengan `nama id` dari elemen yang akan dituju.
    Contoh:
    ```html
    <p id="pembuka">
        <a href="#penutup">Langsung menuju ke tag p dengan id penutup</a> <!--Link Anchor-->
    </p>
    ```

3. **Link untuk Memanggil Fungsi JavaScript:**
    `Link` juga dapat memanggil fungsi dari `JS`, pemanggilan fungsi `JS` dapat menggunakan atribut `event` seperti `onClick`, `onmouseover`, `onmouseout`. Berikut adalah penjelasan singkat beserta contoh penggunaan event tersebut:

    - **`onclick`:** Menetapkan aksi yang akan dijalankan ketika pengguna mengklik elemen.
        ```html
        <a href="#" onclick="myFunction()">Klik Saya</a>
        <script>
            function myFunction() {
                alert("Anda telah mengklik tautan!");
            }
        </script>
        ```

    - **`onmouseover`:** Menetapkan aksi yang akan dijalankan ketika kursor mouse berada di atas elemen.
        ```html
        <a href="#" onmouseover="myFunction()">Arahkan Mouse ke Sini</a>
        <script>
            function myFunction() {
                alert("Mouse berada di atas tautan!");
            }
        </script>
        ```

    - **`onmouseout`:** Menetapkan aksi yang akan dijalankan ketika kursor mouse keluar dari elemen.
        ```html
        <a href="#" onmouseout="myFunction()">Arahkan Mouse ke Sini</a>
        <script>
            function myFunction() {
                alert("Mouse meninggalkan tautan!");
            }
        </script>
        ```

    Dalam contoh-contoh di atas, fungsi JavaScript (`myFunction`) dipanggil saat event yang sesuai terjadi pada tautan. Event-event ini memberikan interaktivitas tambahan kepada halaman web dengan memberikan respons terhadap tindakan pengguna pada elemen tautan.