# 13 - Menampilkan Video pada HTML

## Pendahuluan

Dalam pengembangan situs web, menampilkan video dapat dilakukan dengan menggunakan tag `<video>`. Penggunaan tag ini memungkinkan pengontrolan pemutaran video dan memberikan pengalaman yang lebih interaktif bagi pengguna.

## Contoh Penggunaan

Berikut adalah contoh penggunaan tag `<video>` dalam HTML:

```html
<div class="header">
    <h1>Menampilkan Video pada HTML</h1>
</div>
<div class="section">
    <video controls>
        <source src="/Video Downloader Pinterest - Download Videos, Images & GIFs from Pinterest Online.mp4" type="video/mp4"/>
        Upaya Pertama
    </video>
</div>
```

Pada contoh di atas, nama video disertakan secara langsung karena videonya berada dalam satu folder dengan file HTML. Jika video berada dalam folder yang berbeda, path-nya perlu ditentukan, seperti contoh berikut:

```html
<video controls>
    <source src="video/Video Downloader Pinterest - Download Videos, Images & GIFs from Pinterest Online.mp4" type="video/mp4"/>
</video>
```

Jika video berasal dari website eksternal, atribut `src` harus diisi dengan URL lengkap dari video, seperti contoh berikut:

```html
<video controls>
    <source src="https://www.example.com/videos/cat-herd.webm">
</video>
```

## Penggunaan Tag `<iframe>` untuk Video Eksternal

Jika video berasal dari platform pihak ketiga seperti YouTube, Facebook, Instagram, atau yang lainnya, kita dapat menggunakan tag `<iframe>`. Berikut adalah contoh penggunaannya dengan video YouTube:

```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/Iy3WFRWRybk" frameborder="0" allowfullscreen></iframe>
```

Tag `<iframe>` memungkinkan penyisipan konten eksternal ke dalam halaman web. Dalam konteks video, tag ini memfasilitasi penanaman pemutar video dari platform luar.

## Catatan Penting

Pastikan selalu menyertakan atribut `controls` pada tag `<video>` agar pengguna dapat mengontrol pemutaran video sesuai keinginan mereka.

Dengan menggunakan tag-tag ini, pengembang dapat memberikan pengalaman multimedia yang lebih kaya bagi pengguna situs web.

## Format Video yang Didukung

Berikut adalah format video yang didukung:

| Format FILE | Media Type   |
|-------------|--------------|
| MP4         | video/mp4     |
| WebM        | video/webm    |
| Ogg         | video/ogg     |

**TODO:** Jika kamu punya video dengan format yang berbeda dari ketiga format tersebut, maka kamu harus mengubahnya agar bisa ditambahkan ke HTML.

## Atribut untuk Video

Tag `<video>` punya beberapa atribut yang bisa diberikan:

| Nama Atribut  | Nilai      | Fungsi                                       |
|---------------|------------|----------------------------------------------|
| autoplay      | true/false | Agar video diputar otomatis                  |
| controls      | true/false | Untuk mengaktifkan kontrol pemutar video     |
| loop          | true/false | Untuk memutar video terus menerus            |
| muted         | true/false | Untuk menonaktifkan audio                    |
| poster        | Image Path | Untuk menentukan gambar cover dari video     |
| width & height| angka      | Untuk menentukan tinggi dan lebar video      |
| playsinline   | true/false | Untuk memutar video secara ‘inline’          |

Jika atribut bernilai true, maka ia boleh ditulis namanya saja.

Contoh:

```html
<video loop ="true">
    <source src="Video Downloader Pinterest - Download Videos, Images & GIFs from Pinterest Online.mp4"/>
</video>
```

Boleh ditulis seperti ini:

```html
<video loop>
    <source src="Video Downloader Pinterest - Download Videos, Images & GIFs from Pinterest Online.mp4"/>
</video>
```

Jika nilai atribut bernilai false, maka atribut tersebut boleh tidak ditulis atau juga boleh ditulis.

Contoh:

```html
<video loop = "false">
    <source src="Video Downloader Pinterest - Download Videos, Images & GIFs from Pinterest Online.mp4"/>
</video>
```

Boleh ditulis seperti ini:

```html
<video>
    <source src="Video Downloader Pinterest - Download Videos, Images & GIFs from Pinterest Online.mp4"/>
</video>
```

## Subtitle untuk Video

Subtitle adalah teks yang ditampilkan di dalam video. Biasanya digunakan untuk terjemahan atau alih bahasa dari video dan juga untuk membantu tuna rungu (orang tuli) untuk menyerap informasi pada video.

Subtitle pada HTML dapat kita tambahkan dengan tag `<track>`. Tag ini memiliki atribut src yang akan digunakan untuk menambahkan file subtitle.
Format file subtitle untuk video di dalam HTML adalah `WebVTT (.vtt)` atau Web Video Text Track. File .vtt ini bisa dibuat dengan teks editor.
Sekarang mari kita coba contohnya: subtitle-video.html

```html
<video controls>
    <source src="/Video Downloader Pinterest - Download Videos, Images & GIFs from Pinterest Online.mp4" type="video/mp4">
    <track src="/subtittle.vtt" kind="subtitles" srclang="id" label="indonesia">
</video>
```

**TODO:** Untuk kode lengkapnya ada bisa lihat pada tautan berikut: [subtitle-video.html](/subtitle-video.html).

## Catatan penting:

Subtitle tidak akan ditampilkan jika kita membuka file HTML secara langsung dari browser.

Coba perhatikan di bagian address bar, jika di sana ada tulisan File.. berarti kita membuka file HTML secara langsung.
Namun, jika di address bar ada HTTP atau HTTPS.. itu artinya kita membuka file HTML melalui web server.

..dan juga jika format file .vtt tidak benar, subtile tidak akan ditampilkan.

Pastikan formatnya valid, silahkan gunakan Live WebVTT Validator untuk pengecekan. [Live WebVTT Validator](https://www.example.com/validator).