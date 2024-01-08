# 09 - Membuat List pada HTML

Untuk mengimplementasikan daftar dalam HTML, kita dapat memanfaatkan tag `<li>`. Tag `<li>` (list item) umumnya digunakan bersama dengan tag `<ul>` (unordered list) untuk menciptakan daftar tanpa urutan, atau bersama dengan tag `<ol>` (ordered list) untuk membuat daftar berurutan. Selain itu, tag `<dl>` (description list) dapat digunakan untuk membuat daftar yang terdiri dari pasangan istilah (term) dan definisi (description). Setiap pasangan ini direpresentasikan oleh tag `<dt>` (term) untuk istilah dan tag `<dd>` (description) untuk definisi.

## Penjelasan dan Contoh Penggunaan `<ol>`, `<ul>`, `<dl>`

1. **Ordered List (`<ol>`):**
    - Contoh:
        ```html
        <ol>
            <li>apel</li>
            <li>jeruk</li>
            <li>semangka</li>
        </ol>
        ```
        **Hasil Kode diatas:**
        <ol>
            <li>apel</li>
            <li>jeruk</li>
            <li>semangka</li>
        </ol>

    - Keterangan:
        1. `<ol>` digunakan untuk membuat *ordered list*.
        2. `<li>` adalah tag pembuka setiap item.
        3. 'apel', 'jeruk', dll., merupakan teks dari masing-masing item.
        4. `</ol>` adalah tag penutup.
    - Hasil dari contoh di atas: 
        1. apel
        2. jeruk
        3. semangka

    Untuk mengubah urutan default angka menjadi alfabet atau angka romawi, kita dapat menambahkan atribut `type` pada `<ol>`:
    
    - Menggunakan alfabet kecil ('a'):
        ```html
        <ol type="a">
            <li>apel</li>
            <li>jeruk</li>
            <li>semangka</li>
        </ol>
        ```
        **Hasil kode diatas:**
         <ol type="a">
            <li>apel</li>
            <li>jeruk</li>
            <li>semangka</li>
        </ol>

    - Menggunakan alfabet besar ('A'):
        ```html
        <ol type="A">
            <li>apel</li>
            <li>jeruk</li>
            <li>semangka</li>
        </ol>
        ```
        **Hasil kode diatas:**
        <ol type="A">
            <li>apel</li>
            <li>jeruk</li>
            <li>semangka</li>
        </ol>

    - Menggunakan angka romawi kecil ('i'):
        ```html
        <ol type="i">
            <li>apel</li>
            <li>jeruk</li>
            <li>semangka</li>
        </ol>
        ```
        **Hasil kode diatas:**
        <ol type="i">
            <li>apel</li>
            <li>jeruk</li>
            <li>semangka</li>
        </ol>

    - Menggunakan angka romawi besar ('I'):
        ```html
        <ol type="I">
            <li>apel</li>
            <li>jeruk</li>
            <li>semangka</li>
        </ol>
        ```
        **Hasil kode diatas:**
        <ol type="I">
            <li>apel</li>
            <li>jeruk</li>
            <li>semangka</li>
        </ol>

2. **Unordered List (`<ul>`):**
    Secara default, simbol yang digunakan oleh unordered list adalah lingkaran kecil (disc). Simbol ini dapat diubah dengan atribut `type`.

    - Contoh untuk simbol disc:
    ```html
    <ul>
        <li>apel</li>
        <li>jeruk</li>
        <li>semangka</li>
    </ul>
    ```
    **Hasil kode diatas:**
    <ul>
        <li>apel</li>
        <li>jeruk</li>
        <li>semangka</li>
    </ul>

    Jika ingin menggunakan simbol lain, dapat menggunakan atribut `type`. Selain itu, simbol dapat digantikan dengan gambar:
    ```html
    <ul style="list-style-image: url(https://assets.ubuntu.com/sites/ubuntu/latest/u/img/favicon.ico)">
        <li>apel</li>
        <li>jeruk</li>
        <li>semangka</li>
    </ul>
    ```
    **Hasil kode diatas:**
    <ul style="list-style-image: url(https://assets.ubuntu.com/sites/ubuntu/latest/u/img/favicon.ico)">
        <li>apel</li>
        <li>jeruk</li>
        <li>semangka</li>
    </ul>

3. **Description List (`<dl>`):**
    Description List adalah list yang berisi deskripsi atau penjelasan dari sesuatu. Ada tiga tag yang digunakan untuk membuat description list:
    - `<dl>` (description list): tag pembuka untuk memulai description list;
    - `<dt>` (description term): tag pembuka untuk membuat kata yang akan dideskripsikan;
    - `<dd>` (description description): tag pembuka untuk membuat penjelasan dari kata.

    Contoh penggunaan:
    ```html
    <dl>
        <dt>Kata 1</dt>
        <dd>Penjelasan 1</dd>
        <dt>Kata 2</dt>
        <dd>Penjelasan 2</dd>
    </dl>
    ```
    **Hasil kode diatas:**
    <dl>
        <dt>Kata 1</dt>
        <dd>Penjelasan 1</dd>
        <dt>Kata 2</dt>
        <dd>Penjelasan 2</dd>
    </dl>

4. **List Didalam List (Nested List):**
    List dapat dibuat di dalam list lain. Contohnya, kita dapat menggabungkan unordered list dengan ordered list.
    ```html
    <h1>Macam-Macam Framework untuk FE dan BE</h1>
    <ol>
        <li>Front End
            <ul>
                <li>React JS</li>
                <li>Vue JS</li>
                <li>Next JS</li>
            </ul>
        </li>
        <li>Back End
            <ul>
                <li>Express JS</li>
                <li>Hapy</li>
                <li>Laravel</li>
            </ul>
        </li>
    </ol>
    ```
    **Hasil kode diatas

:**
    <h1>Macam-Macam Framework untuk FE dan BE</h1>
    <ol>
        <li>Front End
            <ul>
                <li>React JS</li>
                <li>Vue JS</li>
                <li>Next JS</li>
            </ul>
        </li>
        <li>Back End
            <ul>
                <li>Express JS</li>
                <li>Hapy</li>
                <li>Laravel</li>
            </ul>
        </li>
    </ol>