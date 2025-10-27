# Lab6Web

**Nama         : Amelia Nurmala Dewi**

**NIM          : 312410199**

**Kelas        : TI.24.A2**

**Mata Kuliah  : Pemrograman Web 1**

## Langkah-Langkah Praktikum

### 1. Bagian `<head>`
Pada bagian `<head>` terdapat elemen-elemen penting seperti:
- **`<meta charset>` dan `<meta viewport>`** → Agar website bisa ditampilkan dengan benar di semua perangkat.
- **`<title>`** → Judul website yang muncul di tab browser (“Informatics Gallery | Home”).
- **Link Bootstrap CDN** → Bootstrap digunakan untuk mempercepat pembuatan desain agar tampak rapi dan responsif.
- **Bagian `<style>`** → Berisi kode CSS internal yang mengatur tampilan (warna, ukuran teks, jarak, efek hover, dan layout keseluruhan).

Contohnya:
```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
```
Kode di atas memanggil file CSS dari Bootstrap versi 5.3 langsung dari server CDN.

---

### 2. Desain Umum dan Warna
Warna utama yang digunakan adalah **gradasi ungu dan pink**:
```css
background: linear-gradient(to right, #8e2de2, #ff6fd8);
```
Warna ini memberi kesan lembut namun tetap modern, sesuai tema teknologi kreatif.

---

### 3. Bagian Navbar
```html
<nav class="navbar navbar-expand-sm shadow-sm sticky-top">
  ...
</nav>
```
Navbar berfungsi sebagai menu navigasi yang selalu terlihat di bagian atas halaman (*sticky-top*).  
Isi menunya terdiri dari: **Home, Gallery, Articles, dan Contact**.  
Ketika pengguna menggulir halaman, navbar tetap menempel di atas layar agar mudah diakses.

---

### 4. Bagian Header
```html
<header>
  <div class="container">
    <h1>Informatics Gallery</h1>
    <p>Tempat di mana Teknologi, Kreativitas, dan Inovasi Bertemu </p>
  </div>
</header>
```
Bagian header ini berfungsi sebagai pengenalan website.  
Tampil dengan latar belakang gradasi ungu-pink dan teks putih yang tegas agar langsung menarik perhatian pengunjung.  
Juga menggunakan efek **rounded corner** (lengkungan di bawah header) agar terlihat lebih halus.

---

### 5. Hero Section
```html
<section class="container hero mt-4">
  <div class="hero-content">
    <h2>“Teknologi Adalah Seni yang Bisa Mengubah Dunia”</h2>
    <p>Informatics Gallery menghadirkan karya, ide, dan inovasi ...</p>
    <a href="#gallery" class="btn btn-custom mt-3">Jelajahi Sekarang</a>
  </div>
</section>
```
Bagian **hero section** ini berisi gambar latar besar (background image) dengan teks motivatif dan tombol “Jelajahi Sekarang”.  
Tujuannya adalah menarik perhatian di awal dan menggambarkan semangat utama website.  
Efek gelap pada latar (rgba hitam transparan) membantu teks terlihat jelas.

---

### 6. Bagian “Tentang Informatics Gallery”
Bagian ini menjelaskan secara ringkas tujuan dan konsep web:
```html
<section class="container mt-5 text-center">
  <h3 class="section-title">Tentang Informatics Gallery</h3>
  <p class="text-muted px-4">Informatics Gallery adalah ruang inspiratif ...</p>
</section>
```
Di bawahnya ditambahkan **galeri foto empat gambar** bertema teknologi (menggunakan grid CSS).  
Tujuannya agar bagian teks tidak monoton dan tetap menarik visualnya.

---

### 7. Bagian “Proyek & Inovasi Unggulan”
```html
<section id="gallery" class="container mt-5">
  <h3 class="section-title"> Proyek & Inovasi Unggulan</h3>
  <div class="row text-center">
    <div class="col-md-4 mb-4">
      <div class="card h-100">
        <img src="gambar1.jpg" alt="">
        <div class="card-body">
          <h5 class="card-title">Desain Antarmuka (UI)</h5>
          <p class="text-muted">Desain interaktif yang memadukan estetika ...</p>
        </div>
      </div>
    </div>
  </div>
</section>
```
Bagian ini menampilkan beberapa **card Bootstrap** yang berisi gambar dan deskripsi singkat setiap proyek.  
Setiap card memiliki efek *hover* (naik sedikit dan menampilkan bayangan).  
Semua gambar bertema teknologi seperti *web design*, *AI*, *e-commerce*, dan *creative coding*.

---

### 8. Bagian “Mengapa Dunia Informatika Itu Menarik”
Bagian ini lebih ke motivasi atau filosofi:
```html
<section class="container highlight text-center">
  <h3 class="section-title"> Mengapa Dunia Informatika Itu Menarik?</h3>
  <p class="text-muted px-3">Informatika bukan hanya tentang komputer ...</p>
</section>
```
Bagian ini diberi latar warna pastel (ungu muda dan pink muda) agar terlihat lembut dan nyaman dibaca.  
Gunanya untuk membuat pembaca merasa bahwa dunia informatika bukan hal yang menakutkan, tapi menyenangkan.

---

### 9. Bagian “Tren Teknologi 2025”
Menampilkan tiga tren teknologi modern:
- **Artificial Intelligence Everywhere**
- **Cloud & Data Security**
- **Human-Centered Design**

Setiap tren dibungkus dalam kotak *trend-card* dengan efek hover ringan.  
Bagian ini mengajak pembaca untuk tahu arah perkembangan dunia teknologi secara global.

---

### 10. Bagian “Inspirasi Penutup”
Bagian terakhir memberikan motivasi dan penutup yang positif:
```html
<section class="container highlight text-center">
  <h3 class="section-title"> Dunia Informatika Adalah Dunia Kreatif</h3>
  <p class="text-muted px-4">Informatika bukan sekadar mengetik kode ...</p>
</section>
```
Disertai grid gambar tambahan agar tampilan akhir terasa lebih hidup dan berwarna.

---

### ⚙️ 11. Bagian Footer
```html
<footer class="text-center">
  <p>© 2025 - Informatics Gallery | Designed with 💜 to Inspire the Future</p>
</footer>
```
Footer berfungsi sebagai penutup halaman dengan warna dasar ungu dan teks putih.  
Menampilkan hak cipta dan kalimat penutup agar terlihat profesional.

---

### 12. Penggunaan Bootstrap
Bootstrap mempermudah Amel dalam:
- Mengatur layout responsif (`.container`, `.row`, `.col-md-4`)
- Memberi gaya tombol (`.btn`, `.btn-custom`)
- Membuat grid gambar otomatis (`display: grid`)
- Menambahkan *shadow effect* dan *hover animation*

Semua itu dilakukan tanpa perlu library tambahan selain Bootstrap dan CSS internal.

---

Berikut adalah hasil tampilan website yang saya buat:
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/c384883d-e510-4a92-907b-388c7a9099fc" />
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/84423e05-7f1b-4016-9240-319f973d5782" />
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/0a2541ec-7b5d-45df-a289-cfc2e11a94d4" />

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/03202978-5291-4240-897d-f0d749e049c5" />



