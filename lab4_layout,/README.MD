# LAPORAN PRAKTIKUM 4 - CSS LAYOUT

## Identitas Mahasiswa
- Nama: [Nama Kamu]
- NIM: [NIM Kamu]
- Kelas: [Kelas Kamu]
- Mata Kuliah: Pemrograman Web

---

# 1. Box Element

## Penjelasan
Box Element merupakan konsep yang menganggap setiap elemen HTML sebagai sebuah kotak. Pada praktikum ini dibuat tiga elemen div.

## Coding HTML

```html
<section>
    <div class="div1">Div 1</div>
    <div class="div2">Div 2</div>
    <div class="div3">Div 3</div>
</section>
```

## Coding CSS

```css
div {
    padding: 10px;
}

.div1 {
    background: red;
}

.div2 {
    background: yellow;
}

.div3 {
    background: green;
}
```

## Screenshot Hasil Browser

<!-- Letakkan screenshot Box Element di sini -->

---

# 2. CSS Float Property

## Penjelasan
Properti float digunakan untuk mengatur posisi elemen agar dapat berada berdampingan secara horizontal.

## Coding CSS

```css
div {
    float: left;
    padding: 10px;
}

.div1 {
    background: red;
}

.div2 {
    background: yellow;
}

.div3 {
    background: green;
}
```

## Screenshot Hasil Browser

<!-- Letakkan screenshot CSS Float di sini -->

---

# 3. Clearfix Element

## Penjelasan
Properti clear digunakan untuk mengatur elemen agar tidak berada di samping elemen yang menggunakan float.

## Coding HTML

```html
<section>
    <div class="div1">Div 1</div>
    <div class="div2">Div 2</div>
    <div class="div3">Div 3</div>
    <div class="div4">Div 4</div>
</section>
```

## Coding CSS

```css
.div4 {
    background-color: blue;
    clear: left;
    float: none;
}
```

## Screenshot Hasil Browser

<!-- Letakkan screenshot Clearfix di sini -->

---

# 4. Layout Website Sederhana

## Penjelasan
Layout website merupakan pengaturan tata letak halaman web yang terdiri dari header, navigasi, konten utama, sidebar, dan footer.

## Coding HTML

```html
<div id="container">
    <header>
        <h1>Layout Sederhana</h1>
    </header>

    <nav>
        <a href="home.html" class="active">Home</a>
        <a href="artikel.html">Artikel</a>
        <a href="about.html">About</a>
        <a href="kontak.html">Kontak</a>
    </nav>

    <section id="hero"></section>

    <section id="wrapper">
        <section id="main"></section>
        <aside id="sidebar"></aside>
    </section>

    <footer>
        <p>&copy; 2021 - Universitas Pelita Bangsa</p>
    </footer>
</div>
```

## Screenshot Hasil Browser

<!-- Letakkan screenshot Layout Website di sini -->

---

# 5. Navigasi dan Hero Panel

## Penjelasan
Navigasi digunakan untuk berpindah halaman, sedangkan hero panel menampilkan judul dan deskripsi utama website.

## Coding HTML

```html
<section id="hero">
    <h1>Hello World!</h1>
    <p>
        Selamat datang di halaman website sederhana.
        Website ini dibuat untuk praktikum CSS Layout.
    </p>
    <a href="home.html" class="btn btn-large">
        Learn More
    </a>
</section>
```

## Coding CSS

```css
nav {
    display: block;
    background-color: #1f5faa;
}

nav a {
    padding: 15px 30px;
    display: inline-block;
    color: #ffffff;
    font-size: 14px;
    text-decoration: none;
    font-weight: bold;
}

nav a.active,
nav a:hover {
    background-color: #2b83ea;
}

#hero {
    background-color: #e4e4e5;
    padding: 50px 20px;
    margin-bottom: 20px;
}
```

## Screenshot Hasil Browser

<!-- Letakkan screenshot Navigasi dan Hero Panel di sini -->

---

# 6. Main Content dan Sidebar

## Penjelasan
Main content merupakan bagian utama website, sedangkan sidebar digunakan untuk menampilkan informasi tambahan.

## Coding HTML

```html
<section id="wrapper">
    <section id="main">
        <h2>Konten Utama</h2>
        <p>Ini adalah bagian konten utama website.</p>
    </section>

    <aside id="sidebar">
        <h3>Widget Header</h3>
        <ul>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
        </ul>
    </aside>
</section>
```

## Coding CSS

```css
#wrapper {
    margin: 0;
}

#main {
    float: left;
    width: 640px;
    padding: 20px;
}

#sidebar {
    float: left;
    width: 260px;
    padding: 20px;
}

footer {
    clear: both;
    background-color: #1d1d1d;
    padding: 20px;
    color: #eee;
}
```

## Screenshot Hasil Browser

<!-- Letakkan screenshot Main Content dan Sidebar di sini -->

---

# 7. Menambahkan Konten dan Artikel

## Penjelasan
Bagian ini berisi kotak konten yang dilengkapi gambar, judul, deskripsi, dan tombol.

## Coding HTML

```html
<div class="row">
    <div class="box">
        <img src="https://dummyimage.com/120/db7d25/fff.png"
             alt="Gambar Konten">
        <h3>Heading</h3>
        <p>Ini adalah deskripsi konten website.</p>
        <a href="#" class="btn btn-default">View detail</a>
    </div>
</div>

<article class="entry">
    <h2>Artikel Pertama</h2>
    <img src="https://dummyimage.com/150/7b8a70/fff.png"
         alt="Gambar Artikel">
    <p>Ini adalah contoh artikel pada halaman website.</p>
</article>
```

## Coding CSS

```css
.box {
    display: block;
    float: left;
    width: 33.333333%;
    box-sizing: border-box;
    padding: 0 10px;
    text-align: center;
}

.image-circle {
    border-radius: 50%;
}

.entry {
    margin: 15px 0;
}

.entry img {
    float: left;
    border-radius: 5px;
    margin-right: 15px;
}
```

## Screenshot Hasil Browser

<!-- Letakkan screenshot Konten dan Artikel di sini -->

---

# 8. Membuat Halaman About

## Penjelasan
Halaman About berisi informasi tentang diri sendiri, pendidikan, keahlian, dan portofolio.

## Coding HTML

```html
<section id="main">
    <h2>Profil Saya</h2>

    <img src="images/profil.jpg"
         alt="Foto Profil"
         width="150">

    <p>Nama: [Nama Kamu]</p>
    <p>Program Studi: Teknik Informatika</p>
    <p>Universitas: Universitas Pelita Bangsa</p>

    <h2>Keahlian</h2>
    <p>Saya sedang mempelajari HTML, CSS, dan pemrograman web.</p>

    <h2>Portofolio</h2>
    <p>Website sederhana untuk tugas praktikum.</p>
</section>
```

## Coding CSS

```css
#main img {
    border-radius: 50%;
    object-fit: cover;
    margin-bottom: 15px;
}
```

## Screenshot Hasil Browser

<!-- Letakkan screenshot halaman About di sini -->

---

# 9. Membuat Halaman Contact

## Penjelasan
Halaman Contact berisi formulir untuk memasukkan nama, email, dan pesan.

## Coding HTML

```html
<section id="main">
    <h2>Formulir Kontak</h2>

    <form>
        <label for="nama">Nama:</label><br>
        <input type="text" id="nama" name="nama"
               placeholder="Masukkan nama" required>

        <br><br>

        <label for="email">Email:</label><br>
        <input type="email" id="email" name="email"
               placeholder="Masukkan email" required>

        <br><br>

        <label for="pesan">Pesan:</label><br>
        <textarea id="pesan" name="pesan"
                  rows="5" placeholder="Tulis pesan"
                  required></textarea>

        <br><br>

        <button type="submit">Kirim</button>
    </form>
</section>
```

## Screenshot Hasil Browser

<!-- Letakkan screenshot halaman Contact di sini -->

---

# Kesimpulan

Praktikum 4 CSS Layout membahas pembuatan tata letak website menggunakan HTML dan CSS. Materi meliputi Box Element, CSS Float, Clear, HTML5 Semantic Elements, navigasi, main content, sidebar, footer, serta pembuatan halaman About dan Contact.
