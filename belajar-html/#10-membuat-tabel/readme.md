# Membuat Tabel pada HTML

Presentasi informasi dalam web dapat dilakukan dengan menggunakan elemen `Table`. **Elemen `Table` terdiri dari 4 unsur utama:**
1. Baris
2. Kolom
3. Sel
4. Garis

**Tag untuk membuat Tabel pada HTML:**
# Membuat Tabel pada HTML

Penting untuk diingat beberapa `tag` saat membuat `table` pada `HTML`:

| No | Tag       | Keterangan                                       |
|---|-----------|--------------------------------------------------|
| 1  | `<table>` | Digunakan untuk membungkus tabel.                |
| 2  | `<thead>` | Digunakan untuk membungkus bagian kepala tabel.  |
| 3  | `<tbody>` | Digunakan untuk membungkus bagian isi tabel.     |
| 4  | `<tr>`    | Digunakan untuk membuat baris dalam tabel.       |
| 5  | `<td>`    | Digunakan untuk membuat sel/data dalam tabel.    |
| 6  | `<th>`    | Digunakan untuk membuat judul pada kepala tabel. |

**Penting untuk memahami penggunaan setiap tag di atas agar dapat membuat tabel `HTML` dengan benar dan efisien. Tag yang paling penting untuk diingat adalah `<table>`, `<tr>`, dan `<td>`. Sementara tag yang lain bersifat tambahan (opsional) dan dapat digunakan atau tidak.**

Contoh penggunaan tag:
```html
<table>
    <tr>
        <td>baris 1</td>
        <td>baris 2</td>
    </tr>
    <tr>
        <td>kolom 1</td>
        <td>kolom 2</td>
    </tr>
</table>
```
**Hasil dari kode di atas:**
<table>
    <tr>
        <td>baris 1</td>
        <td>baris 2</td>
    </tr>
    <tr>
        <td>kolom 1</td>
        <td>kolom 2</td>
    </tr>
</table>

Pada contoh di atas, ketika ditampilkan pada browser, tabel tidak memiliki `garis (border)`. Bagaimana cara menambahkan `garis`? Untuk menambahkan `garis`, kita perlu menggunakan atribut `border=""` pada tag `<table>`. Berikut contohnya:
```html
<table border="2">
    <tr>
        <td>baris 1</td>
        <td>baris 2</td>
    </tr>
    <tr>
        <td>kolom 1</td>
        <td>kolom 2</td>
    </tr>
</table>
```
**Hasil dari kode di atas:**
<table border="2">
    <tr>
        <td>baris 1</td>
        <td>baris 2</td>
    </tr>
    <tr>
        <td>kolom 1</td>
        <td>kolom 2</td>
    </tr>
</table>

**Nilai "2" pada atribut border adalah ukuran garisnya. Semakin besar ukurannya, maka semakin besar pula ukuran garisnya.**

**Mengatur Jarak Sel dengan Cellpadding**
Atribut `cellpadding` digunakan untuk mengatur jarak antara `teks` dengan `garis` di dalam `sel`. Atribut ini dapat digunakan di dalam tag `table`. Contohnya:
```html
<body>
    <table border="2" cellpadding="15">
        <tr>
            <td>baris 1</td>
            <td>baris 2</td>
        </tr>
        <tr>
            <td>kolom 1</td>
            <td>kolom 2</td>
        </tr>
    </table>
</body>
```
**Hasil dari kode di atas:**
<body>
    <table border="2" cellpadding="15">
        <tr>
            <td>baris 1</td>
            <td>baris 2</td>
        </tr>
        <tr>
            <td>kolom 1</td>
            <td>kolom 2</td>
        </tr>
    </table>
</body>

**Nilai "15" pada atribut cellpadding adalah ukuran jarak antara teks sel dengan garis.**

**Menambahkan Warna pada Sel dan Baris**
Untuk menambahkan warna pada sel dan baris, kita bisa menggunakan atribut `bgcolor="` pada tag `<tr>` untuk baris
dan pada `<td>` pada sel.
Contoh:
```html
<body>
    <table border="2" cellpadding="15">
        <tr bgcolor="yellow">
            <td>baris 1</td>
            <td>baris 2</td>
        </tr>
        <tr>
            <td bgcolor="#0000ff">kolom 1</td>
            <td>kolom 2</td>
        </tr>
    </table>
</body>
```
**Hasil dari kode di atas:**
<body>
    <table border="2" cellpadding="15">
        <tr bgcolor="yellow">
            <td>baris 1</td>
            <td>baris 2</td>
        </tr>
        <tr>
            <td bgcolor="#0000ff">kolom 1</td>
            <td>kolom 2</td>
        </tr>
    </table>
</body>

**Nilai atribut bgcolor bisa kita isi dengan kode warna dalam heksadesimal atau nama warna dalam bahasa Inggris.**

**Menggabungkan Sel Tabel**

Untuk menggabungkan sel, kita dapat menggunakan atribut `rowspan` dan `colspan`.

    | Atribut  | Penjelasan                  |
    |----------|-----------------------------|
    | rowspan  | Digunakan untuk menggabungkan baris   |
    | colspan  | Digunakan untuk menggabungkan sel     |

**Atribut ini dapat digunakan pada tag `<td>` atau `<th>`.**
Contoh:
```html
<table border="1">
    <tr>
        <th rowspan="2" bgcolor="#3cb371">Bulan</th>
        <th colspan="2" bgcolor="#00ffbf">Hasil Panen</th>
    </tr>
    <tr>
        <th>Jagung Manis</th>
        <th>Kacang Tanah</th>
    </tr>
    <tr>
        <td>Januari</td>
        <td>500 Kg</td>
        <td>250 Kg</td>
    </tr>
    <tr>
        <td>Februari</td>
        <td>750 Kg</td>
        <td>350 Kg</td>
    </tr>
</table>
```
**Hasil dari kode di atas

:**
<table border="1">
    <tr>
        <th rowspan="2" bgcolor="#3cb371">Bulan</th>
        <th colspan="2" bgcolor="#00ffbf">Hasil Panen</th>
    </tr>
    <tr>
        <th>Jagung Manis</th>
        <th>Kacang Tanah</th>
    </tr>
    <tr>
        <td>Januari</td>
        <td>500 Kg</td>
        <td>250 Kg</td>
    </tr>
    <tr>
        <td>Februari</td>
        <td>750 Kg</td>
        <td>350 Kg</td>
    </tr>
</table>

**Dengan menggunakan atribut `rowspan` dan `colspan`, kita dapat menggabungkan sel sesuai kebutuhan pada tabel.**

**Menyisipkan Elemen yang Lain ke dalam Sel**
Didalam sel `<td>` dan `<th>` kita bisa menyisipkan elemen `HTML` yang lain,
seperti: `gambar`, `audio`,`link`,`video`,`dsb`.
~ Contoh:
```html
<body>
    <table border="1">
        <tr>
            <th colspan="3" style="background-color: green;">Produk Unggulan</th>
        </tr>
        <tr>
            <td rowspan="1">
                <img src="https://down-id.img.susercontent.com/file/id-11134207-7r98y-loqdadgmj3zk3e" alt="Deskripsi Gambar" style="height: 228px;">
            </td>            
            <td>Nama Barang</td>
            <td>PC + MONITOR full AMD Series</td>
        </tr>
        <tr>
            <td>Harga Barang</td>
            <td>Rp. 5.000.000</td>
        </tr>
        tr>
            <td>Fitur</td>
            <td colspan="2">
                <ul>
                    <li>LED 24 Inch Full HD</li>
                    <li>MB Asrock A520M</li>
                    <li>AMD Ryzen 5 5600G</li>
                    <li>VGA Integrated AMD Radeon Vega Series Graphics</li>
                    <li>HDD Seagate 500GB Sata</li>
                </ul>
            </td>
        </tr>
    </table>
</body>
```
**Hasil kode diatas**
<body>
    <table border="1">
        <tr>
            <th colspan="3" style="background-color: green;">Produk Unggulan</th>
        </tr>
        <tr>
            <td rowspan="1">
                <img src="https://down-id.img.susercontent.com/file/id-11134207-7r98y-loqdadgmj3zk3e" alt="Deskripsi Gambar" style="height: 228px;">
            </td>            
            <td>Nama Barang</td>
            <td>PC + MONITOR full AMD Series</td>
        </tr>
        <tr>
            <td>Harga Barang</td>
            <td>Rp. 5.000.000</td>
        </tr>
        <tr>
            <td>Fitur</td>
            <td colspan="2">
                <ul>
                    <li>LED 24 Inch Full HD</li>
                    <li>MB Asrock A520M</li>
                    <li>AMD Ryzen 5 5600G</li>
                    <li>VGA Integrated AMD Radeon Vega Series Graphics</li>
                    <li>HDD Seagate 500GB Sata</li>
                </ul>
            </td>
        </tr>
    </table>
</body>