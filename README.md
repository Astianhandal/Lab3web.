# Lab3web.
# Praktikum 3: CSS Dasar

Repository ini dibuat untuk memenuhi tugas Praktikum 3 mata kuliah Pemrograman Web, dengan materi CSS Dasar. Praktikum ini membahas penggunaan CSS untuk mengatur tampilan halaman web, cara penulisan CSS, serta penggunaan selector pada elemen HTML.

## Tujuan Praktikum

1. Memahami konsep dasar CSS.
2. Memahami aturan penulisan pada CSS.
3. Memahami selector sebagai pengontrol CSS.
4. Membuat pengaturan CSS pada HTML.

## Persiapan Praktikum

Perangkat dan file yang digunakan dalam praktikum ini adalah:

* Text editor Visual Studio Code.
* Web browser untuk melihat hasil tampilan halaman.
* File HTML `lab2_css_dasar.html`.
* File CSS eksternal `style_eksternal.css`.
* Repository GitHub dengan nama `Lab3Web`.

## Langkah 1: Membuat Dokumen HTML

Pada langkah pertama, dibuat dokumen HTML dengan nama `lab2_css_dasar.html`. Dokumen ini berisi struktur dasar HTML, yaitu `head` dan `body`, serta beberapa elemen seperti `header`, `nav`, `div`, `h1`, `p`, dan `a`.

Bagian `header` digunakan untuk menampilkan judul halaman. Bagian `nav` berisi tautan menuju halaman CSS Dasar, CSS Eksternal, dan HTML Dasar. Sementara itu, bagian `div` dengan ID `intro` berisi judul Hello World, paragraf pengantar, serta tautan informasi selengkapnya.

Pada tahap ini, halaman masih menggunakan tampilan HTML dasar sebelum diberikan pengaturan CSS.

**Screenshot 1 — Tampilan HTML Dasar**

<img width="932" height="413" alt="Screenshot 2026-10-08 215459" src="https://github.com/user-attachments/assets/71452b2b-6043-40d7-9074-594912b66bd5" />


## Langkah 2: Mendeklarasikan Internal CSS

Pada langkah kedua, ditambahkan Internal CSS pada bagian `head` dokumen HTML menggunakan tag `<style>`. CSS ini digunakan untuk mengatur tampilan elemen yang terdapat pada halaman.

Pengaturan yang ditambahkan meliputi:

* `body`: menentukan jenis font menggunakan Open Sans dengan sans-serif sebagai alternatif.
* `header`: memberikan tinggi minimum dan garis bawah.
* `h1`: mengatur ukuran teks, warna, perataan teks, dan padding.
* `h1 i`: memberikan warna berbeda pada teks yang berada di dalam elemen italic pada judul.

Internal CSS memudahkan pengaturan tampilan beberapa elemen HTML tanpa harus menambahkan atribut `style` satu per satu.

**Screenshot 2 — Tampilan Setelah Penambahan Internal CSS**

<img width="940" height="461" alt="Screenshot 2026-10-08 215945" src="https://github.com/user-attachments/assets/31093b2e-2af0-46f6-856a-56578da4354c" />


## Langkah 3: Menambahkan Inline CSS

Pada langkah ketiga, ditambahkan Inline CSS pada elemen paragraf menggunakan atribut `style`.

Contoh deklarasi yang digunakan:

```html
<p style="text-align: center; color: #ccd8e4;">
```

Deklarasi tersebut mengatur perataan teks menjadi rata tengah menggunakan `text-align: center` dan mengatur warna teks menggunakan `color: #ccd8e4`.

Inline CSS diterapkan secara langsung pada elemen HTML yang diberikan atribut `style`, sehingga pengaturannya ditujukan pada elemen tersebut.

**Screenshot 3 — Tampilan Setelah Penambahan Inline CSS**

<img width="912" height="463" alt="Screenshot 2026-10-08 220209" src="https://github.com/user-attachments/assets/dfafdcb4-70db-4214-b8ff-f0a54b19c7b3" />


## Langkah 4: Membuat CSS Eksternal

Pada langkah keempat, dibuat file baru bernama `style_eksternal.css`. File ini digunakan untuk mengatur tampilan navigasi pada halaman web.

Pengaturan CSS yang ditambahkan meliputi:

* `nav`: memberikan warna latar belakang hijau, warna teks putih, dan padding.
* `nav a`: mengatur warna tautan, menghilangkan garis bawah, dan memberikan jarak pada tautan.
* `nav .active`: mengatur tampilan tautan yang memiliki class `active`.
* `nav a:hover`: memberikan perubahan warna latar belakang ketika kursor diarahkan ke tautan.

Agar file CSS eksternal dapat digunakan oleh dokumen HTML, ditambahkan tag `<link>` pada bagian `head`.

Contoh penggunaannya:

```html
<link rel="stylesheet" href="style_eksternal.css" type="text/css">
```

Dengan cara ini, pengaturan CSS disimpan dalam file terpisah dari dokumen HTML sehingga lebih mudah dikelola dan digunakan kembali.

**Screenshot 4 — Tampilan Setelah Penambahan External CSS**

<img width="1365" height="646" alt="WhatsApp Image 2026-10-08 at 22 47 18" src="https://github.com/user-attachments/assets/8c00a05c-99e3-40cc-9f5f-cab66017d78c" />


## Langkah 5: Menambahkan CSS ID Selector dan Class Selector

Pada langkah kelima, ditambahkan ID Selector dan Class Selector ke dalam file `style_eksternal.css`.

### A. ID Selector

ID Selector menggunakan tanda pagar (`#`) sebelum nama ID. Pada praktikum ini, selector `#intro` digunakan untuk mengatur bagian pengantar halaman.

Pengaturan yang diberikan meliputi:

* Warna latar belakang biru.
* Border berwarna hijau.
* Tinggi minimum elemen.
* Padding untuk memberikan jarak antara isi dan batas elemen.

Selain itu, selector `#intro h1` digunakan untuk mengatur judul `h1` yang berada di dalam elemen dengan ID `intro`. Pengaturannya meliputi perataan teks ke kiri, menghilangkan border, dan mengubah warna teks menjadi putih.

### B. Class Selector

Class Selector menggunakan tanda titik (`.`) sebelum nama class.

Pada praktikum ini, class `.button` digunakan untuk mengatur tampilan tautan agar menyerupai tombol. Pengaturannya meliputi padding, warna latar belakang, warna teks, jenis tampilan `inline-block`, margin, dan penghilangan garis bawah.

Selanjutnya, class `.btn-primary` digunakan untuk memberikan warna latar belakang merah pada tombol utama.

Pada HTML, elemen tautan menggunakan dua class sekaligus, yaitu `button` dan `btn-primary`. Dengan demikian, elemen tersebut menerima pengaturan dari kedua class tersebut.

**Screenshot 5 — Tampilan Setelah Penambahan ID Selector dan Class Selector**

<img width="1365" height="646" alt="WhatsApp Image 2026-10-08 at 22 47 17" src="https://github.com/user-attachments/assets/5ee8b5ca-1de3-45a4-ba9b-cc564f8d067b" />


## Pertanyaan dan Tugas

### 1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet.

Eksperimen CSS dilakukan dengan mengubah dan menambahkan properti serta nilai CSS untuk melihat pengaruhnya terhadap tampilan halaman web.

Beberapa properti yang digunakan dalam praktikum ini adalah:

| Properti          | Fungsi                                        |
| ----------------- | --------------------------------------------- |
| `background`      | Mengatur latar belakang elemen.               |
| `color`           | Mengatur warna teks.                          |
| `font-family`     | Mengatur jenis font.                          |
| `font-size`       | Mengatur ukuran teks.                         |
| `text-align`      | Mengatur perataan teks.                       |
| `padding`         | Mengatur jarak antara isi dan batas elemen.   |
| `margin`          | Mengatur jarak di luar batas elemen.          |
| `border`          | Mengatur garis batas elemen.                  |
| `min-height`      | Menentukan tinggi minimum elemen.             |
| `text-decoration` | Mengatur dekorasi teks, misalnya garis bawah. |

Perubahan properti dan nilai tersebut dapat diamati langsung melalui browser setelah file disimpan dan halaman dimuat ulang.

**Screenshot 6 — Hasil Eksperimen Perubahan Properti CSS**

<!-- MASUKKAN SCREENSHOT 6 DI SINI -->

### 2. Apa perbedaan deklarasi CSS elemen `h1 { ... }` dengan `#intro h1 { ... }`?

Deklarasi `h1 { ... }` merupakan Element Selector yang berlaku untuk semua elemen `h1` pada dokumen HTML yang sesuai dengan aturan tersebut.

Sementara itu, deklarasi `#intro h1 { ... }` merupakan selector gabungan yang menargetkan elemen `h1` yang berada di dalam elemen dengan ID `intro`.

Contoh:

```css
h1 {
    color: blue;
    text-align: center;
}

#intro h1 {
    color: white;
    text-align: left;
}
```

Pada contoh tersebut, elemen `h1` yang berada di dalam `#intro` akan menggunakan warna putih dan perataan teks ke kiri karena selector `#intro h1` lebih spesifik. Elemen `h1` lain yang tidak berada di dalam `#intro` tetap mengikuti aturan `h1`, selama tidak ada aturan lain yang mengubahnya.

### 3. Apabila terdapat CSS internal, eksternal, dan inline pada elemen yang sama, deklarasi manakah yang akan ditampilkan pada browser?

Secara umum, apabila ketiga deklarasi mengatur properti yang sama pada elemen yang sama, Inline CSS akan diprioritaskan dibandingkan deklarasi CSS internal dan eksternal yang memiliki tingkat kepentingan normal.

Namun, hasil akhir juga dipengaruhi oleh tingkat spesifisitas selector, deklarasi `!important`, serta aturan cascade CSS lainnya.

Contoh:

```html
<head>
    <style>
        p {
            color: blue;
        }
    </style>

    <link rel="stylesheet" href="style_eksternal.css">
</head>

<body>
    <p style="color: red;">Belajar CSS Dasar</p>
</body>
```

Misalnya, file `style_eksternal.css` berisi:

```css
p {
    color: green;
}
```

Pada contoh tersebut, teks paragraf akan berwarna merah karena Inline CSS memiliki prioritas lebih tinggi daripada kedua deklarasi lainnya yang menggunakan aturan normal.

### 4. Apabila sebuah elemen HTML memiliki ID dan Class, deklarasi manakah yang akan ditampilkan pada browser?

ID Selector memiliki tingkat spesifisitas yang lebih tinggi daripada Class Selector. Oleh karena itu, apabila kedua selector mengatur properti yang sama dan tidak ada aturan cascade lain yang mengubah hasilnya, deklarasi dari ID Selector akan diterapkan.

Contoh HTML:

```html
<p id="paragraf-1" class="text-paragraf">
    Ini adalah contoh paragraf.
</p>
```

Contoh CSS:

```css
#paragraf-1 {
    color: red;
}

.text-paragraf {
    color: blue;
}
```

Pada contoh tersebut, teks paragraf akan berwarna merah karena selector `#paragraf-1` memiliki spesifisitas lebih tinggi daripada `.text-paragraf`.

Apabila kedua selector mengatur properti yang berbeda, keduanya tetap dapat diterapkan secara bersamaan. Hasil akhir juga dapat dipengaruhi oleh `!important` dan aturan cascade lainnya.

## Kesimpulan

Berdasarkan Praktikum 3: CSS Dasar, CSS digunakan untuk mengatur tampilan halaman web agar lebih terstruktur dan menarik. Praktikum ini memperkenalkan tiga cara penulisan CSS, yaitu Internal CSS, External CSS, dan Inline CSS.

Selain itu, penggunaan Element Selector, ID Selector, Class Selector, serta selector gabungan dapat membantu mengatur elemen HTML sesuai kebutuhan. Dengan memahami spesifisitas selector dan aturan cascade CSS, pengaturan tampilan halaman web dapat dilakukan secara lebih terarah.

Praktikum ini juga memberikan pengalaman dalam menghubungkan file CSS eksternal dengan HTML dan melihat perubahan tampilan secara langsung melalui browser.

## Validasi CSS

Sesuai instruksi praktikum, dokumen CSS dapat divalidasi melalui layanan CSS Validator dari W3C untuk memeriksa kesesuaian penulisan CSS.

Link validasi: https://jigsaw.w3.org/css-validator/

**Screenshot 7 — Hasil Validasi CSS (Jika Dilakukan)**

<!-- MASUKKAN SCREENSHOT 7 DI SINI -->

## Repository

Nama repository: `Lab3Web`

Repository ini berisi file praktikum HTML dan CSS, dokumentasi pengerjaan melalui README.md, serta screenshot hasil praktikum.
