## 14 - Menyisipkan Audio

# Pendahuluan
Konten dalam web tidak hanya terbatas pada teks dan gambar, melainkan juga dapat berupa multimedia seperti audio dan video. Pada tutorial ini, kita akan membahas cara menyisipkan audio menggunakan HTML. Konten audio umumnya berupa podcast, audiobook, dan musik.

# Cara Menambahkan Audio di HTML
Menambahkan audio dalam HTML dapat dilakukan dengan menggunakan tag `<audio>`. Selanjutnya, kita dapat menentukan file audio yang akan diputar menggunakan tag `<source>`. Berikut adalah contoh penggunaan tag `<audio>`:

```html
<legend>AUDIO</legend>
<fieldset>
    <audio controls>
        <source src="/AS_IF_ITS_YOUR_LAST.mp3" type="audio/mpeg"/>
    </audio>
</fieldset>
```

TODO: Pastikan untuk menyertakan atribut `controls` pada tag `<audio>` untuk memberikan kontrol pemutaran kepada pengguna. Selain itu, tentukan sumber audio dengan atribut `src` dan jenis file dengan atribut `type`.

Dengan implementasi ini, pengguna dapat dengan mudah memutar dan mengontrol audio langsung dari halaman web.

Pada atribut src, kita menulis langsung nama file audio yang akan diputar. Ini karena kita menaruh file tersebut dalam satu folder yang sama dengan file HTML. Jika file audio tersimpan di folder yang berbeda, maka harus ditulis alamat path menuju folder tersebut.

Misalkan, saya menaruhnya di dalam folder 📁 audio, maka atribut src bisa diisi seperti ini:

```html
<audio controls>
    <source src="audio/AS_IF_ITS_YOUR_LAST.mp3" type="audio/mpeg"/>
</audio>
```

…dan jika file audio-nya tersimpan di website yang berbeda, maka kita harus mengisinya dengan alamat URL.

```html
<audio controls>
    <!-- Ganti "URL_FILE_AUDIO" dengan URL langsung ke file audio di Netlify -->
    <source src="URL_FILE_AUDIO" type="audio/mpeg">
</audio>
```

## Format File Audio yang didukung
Audio player di HTML tidak mendukung semua jenis format file audio. Berikut ini daftar format file audio yang bisa diputar di HTML.

Format | Container | MIME type
-------|-----------|----------
PCM    | WAV       | audio/wav
MP3    | MP3       | audio/mpeg
AAC    | MP4       | audio/mp4
AAC    | AAC       | audio/aac
AAC    | AAC       | audio/aacp
Vorbis | Ogg       | audio/ogg
Vorbis | WebM      | audio/webm
Opus   | Ogg       | audio/ogg
Opus   | WebM      | audio/webm
FLAC   | FLAC      | audio/flac
FLAC   | Ogg       | audio/ogg

Format file yang biasanya digunakan adalah MP3 dan MP4 (M4A), karena ukuran filenya relatif kecil. Sementara format FLAC adalah format file audio dengan kualitas tinggi dan ukuran filenya relatif lebih besar.

# Atribut untuk Audio
Tag `<audio>` punya beberapa atribut yang sering digunakan:

1. **controls**
Atribut ini berfungsi untuk mengaktifkan tombol kontrol seperti tombol play, pause, stop, scroll, dan volume).

Contoh penggunaan:

```html
<audio controls="true">
    <source src="audio/Ngoni.mp3" type="audio/mpeg">
    Browsermu tidak mendukung tag audio, upgrade donk!
</audio>
```

<!-- atau -->

```html
<audio controls>
    <source src="audio/Ngoni.mp3" type="audio/mpeg">
    Browsermu tidak mendukung tag audio, upgrade donk!
</audio>
```

Jika bernilai true, maka nilainya boleh tidak diisi. Nilai true artinya, kita akan mengaktifkan tombol kontrol dan jika nilainya false maka artinya tombol kontrol tidak diaktifkan.

2. **autoplay**
Atribut ini berfungsi untuk memutar audio secara otomatis. Nilai yang bisa diberikan pada atribut ini adalah true dan false.

Nilai true artinya kita akan memutar audio secara otomatis, dan false artinya audio tidak akan diputar secara otomatis.

Contoh:

```html
<audio autoplay="true">
    <source src="audio/Ngoni.mp3" type="audio/mpeg">
    Browsermu tidak mendukung tag audio, upgrade donk!
</audio>
```

<!-- atau -->

```html
<audio autoplay>
    <source src="audio/Ngoni.mp3" type="audio/mpeg">
    Browsermu tidak mendukung tag audio, upgrade donk!
</audio>
```

✍️ Catatan: Atribut ini mungkin saja tidak akan bekerja pada Google Chrome, karena ada perubahan policy (kebijakan) dalam memutar audio secara otomatis.

3. **loop**
Atribut loop berfungsi untuk mengulang-ulang pemutaran audio. Ini seperti repeat one. Nilai yang bisa diberikan adalah true dan false.

Contoh:

```html
<audio loop="true">
    <source src="audio/Ngoni.mp3" type="audio/mpeg">
    Browsermu tidak mendukung tag audio, upgrade donk!
</audio>
```

<!-- atau -->

```html
<audio loop>
    <source src="audio/Ngoni.mp3" type="audio/mpeg">
    Browsermu tidak mendukung tag audio, upgrade donk!
</audio>
```

4. **muted**
Atribut ini berfungsi untuk mensenyapkan audio. Nilai yang bisa diberikan adalah true dan false.

Contoh:

```html
<audio muted="true">
    <source src="audio/Ngoni.mp3" type="audio/mpeg">
    Browsermu tidak mendukung tag audio, upgrade donk!
</audio>
```

<!-- atau -->

```html
<audio muted>
    <source src="audio/Ngoni.mp3" type="audio/mpeg">
    Browsermu tidak mendukung tag audio, upgrade donk!
</audio>
```

# Audio Sebagai Background
Audio kadang sering digunakan sebagai background. Biasanya menggunakan musik.

Tujuan menambahkan background agar menambah kesan tertentu pada web. Misalkan, ingin membuat pengunjung merasa santai.. maka kita bisa memutar audio musik yang santai.

Cara membuat musik sebagai background adalah dengan menambahkan atribut autoplay, loop, dan menghilangkan kontrol (hidden).

Contoh:

```html
<body>
  <h1>Contoh audio sebagai background</h1>
  <audio hidden autoplay loop>
    <source src="Ngoni.mp3" type="audio/mpeg">
    Browsermu tidak mendukung tag audio
  </audio>
</body>

```

Hasilnya:

File audio dan HTML
Nggak ada suaranya?

Sekali lagi, atribut autoplay mungkin tidak bekerja di Google Chrome karena ada pembaharuan kebijakan dalam memutar audio.

Sekarang kita coba buka dengan Mozilla Firefox.

File audio dan HTML
Hasilnya sama saja, tidak ada suaranya.

Ini karena autoplay diblokir otomatis.

Sekarang kita coba ubah izin untuk memutar audio secara otomatis. Klik ikon autoplay pada address bar di dekat ikon (i), sehingga muncul seperti ini:

Autoplay di Firefox
Pada bagian Autoplay, ubah Block Audio menjadi Allow Audio and Video.

Setelah itu, coba refresh atau reload.

Maka suaranya akan terdengar.