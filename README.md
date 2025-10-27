# Lab6Web

**Nama         : Amelia Nurmala Dewi**

**NIM          : 312410199**

**Kelas        : TI.24.A2**

**Mata Kuliah  : Pemrograman Web 1**

## 🧩 Langkah-Langkah Praktikum

### 1. Persiapan Awal
Saya mempersiapkan text editor yaitu **Visual Studio Code**, kemudian membuat folder baru dengan nama `lab6_css_framework`.  
Di dalam folder tersebut saya membuat file `index.html` yang akan menjadi halaman utama website.

---

### 2. Menambahkan Bootstrap ke Dalam HTML
Agar dapat menggunakan komponen dari Bootstrap, saya menambahkan link CDN Bootstrap di bagian `<head>` HTML seperti berikut:

```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
```

---

### 3. Membuat Struktur Layout Dasar
Sesuai instruksi praktikum, saya membuat struktur layout sederhana yang terdiri dari:
- Header  
- Navbar  
- Main content (bagian kiri)  
- Sidebar (bagian kanan)  
- Footer  

Semua bagian tersebut diatur menggunakan **grid system Bootstrap** agar tampilan web rapi dan responsif.

---

### 4. Membuat Header
Bagian header berisi judul website dan deskripsi singkat.  
Agar tampil menarik, saya menambahkan **gambar background** serta efek transparan pada teks agar tetap terbaca.

```html
<header class="text-center text-white p-4"
        style="background: url('header.jpg') no-repeat center/cover;">
    <div style="background-color: rgba(255,182,193,0.7); padding:25px; border-radius:10px;">
        <h1>Amel’s Inspiration Blog</h1>
        <p>Berbagi Semangat & Cerita Positif Setiap Hari 🌸</p>
    </div>
</header>
```

---

### 5. Membuat Navbar
Di bawah header saya menambahkan **navbar** menggunakan komponen `navbar` dari Bootstrap.  
Isi menunya yaitu:
- Home  
- Artikel  
- Kutipan  
- Tentang  
- Kontak  

Setiap menu dibuat menggunakan elemen `<a>` dengan class `nav-link`.

```html
<nav class="navbar navbar-expand-sm navbar-light" style="background-color:#ffebf5;">
    <div class="container-fluid justify-content-center">
        <ul class="navbar-nav">
            <li class="nav-item"><a href="#" class="nav-link text-danger fw-semibold">Home</a></li>
            <li class="nav-item"><a href="#" class="nav-link text-danger fw-semibold">Artikel</a></li>
            <li class="nav-item"><a href="#" class="nav-link text-danger fw-semibold">Kutipan</a></li>
            <li class="nav-item"><a href="#" class="nav-link text-danger fw-semibold">Tentang</a></li>
            <li class="nav-item"><a href="#" class="nav-link text-danger fw-semibold">Kontak</a></li>
        </ul>
    </div>
</nav>
```

---

### 6. Membuat Konten Utama
Bagian konten utama berisi teks sambutan dan tiga kolom fitur inspirasi, masing-masing berisi:
- Motivasi Kuliah  
- Kisah Inspiratif  
- Me Time  

Setiap kolom dibuat menggunakan class `.col-md-4` agar sejajar dalam satu baris.

```html
<div class="row text-center">
    <div class="col-md-4 mb-3">
        <div class="border rounded p-3 bg-light">
            <div class="bg-pink rounded-circle d-flex justify-content-center align-items-center mx-auto mb-2"
                 style="width:60px;height:60px;background-color:#ffd6e8;">🌼</div>
            <h5 class="text-danger">Motivasi Kuliah</h5>
            <p>Temukan semangat baru untuk menghadapi hari-hari kuliahmu.</p>
            <button class="btn btn-sm text-white" style="background-color:#ff7eb9;">Selengkapnya</button>
        </div>
    </div>
</div>
```

---

### 7. Membuat Sidebar
Sidebar diletakkan di sisi kanan halaman.  
Isi dari sidebar terdiri dari dua bagian:
- Daftar kategori cerita  
- Form kirim pesan positif  

Keduanya dibuat menggunakan komponen `card` dan `form-control` dari Bootstrap.

```html
<aside class="col-md-4">
    <div class="bg-light p-3 mb-3 border rounded">
        <h5 class="text-danger">Kategori Cerita</h5>
        <ul class="list-unstyled">
            <li>Motivasi</li>
            <li>Kehidupan</li>
            <li>Belajar</li>
            <li>Desain</li>
        </ul>
    </div>
    <div class="bg-light p-3 border rounded">
        <h5 class="text-danger">Kirim Pesan Positifmu 💬</h5>
        <form>
            <input type="text" class="form-control mb-2" placeholder="Nama Kamu">
            <textarea class="form-control mb-2" placeholder="Tulis pesanmu di sini..."></textarea>
            <button class="btn text-white w-100" style="background-color:#ff7eb9;">Kirim</button>
        </form>
    </div>
</aside>
```

---

### 8. Membuat Footer
Bagian footer diletakkan di bawah dengan warna yang sama seperti header agar tampilan konsisten.

```html
<footer class="text-center p-3" style="background-color:#ffd6e8;">
    <p class="mb-0 text-muted">© 2025 - Amel’s Inspiration Blog | Amelia Nurmala Dewi - Universitas Pelita Bangsa</p>
</footer>
```

---

## Hasil Tampilan
Tampilan akhir website saya adalah sebagai berikut:

- Menggunakan tema **pink pastel dan putih**.  
- Layout sudah lengkap (header, navbar, main content, sidebar, footer).  
- Website terlihat lembut dan inspiratif sesuai tema “Amel’s Inspiration Blog”.  
- Semua elemen menggunakan **komponen Bootstrap**.

---

Berikut adalah hasil tampilan website yang saya buat:
<img width="1366" height="679" alt="Screenshot (954)" src="https://github.com/user-attachments/assets/c30a80f6-2b72-41d4-bf04-130a0561de43" />
<img width="1366" height="679" alt="Screenshot (955)" src="https://github.com/user-attachments/assets/df265813-6cb9-466a-8350-37ac275dea13" />
<img width="1366" height="675" alt="Screenshot (956)" src="https://github.com/user-attachments/assets/0521be0f-3866-48a6-bbf9-3d2c3e962678" />
<img width="1366" height="669" alt="Screenshot (957)" src="https://github.com/user-attachments/assets/1181a415-9695-4994-bca4-b4cc8cc1847c" />
<img width="1366" height="669" alt="Screenshot (957)" src="https://github.com/user-attachments/assets/9a37d706-62f1-4b78-bbc7-cca2b68d1ced" />
<img width="1366" height="675" alt="Screenshot (951)" src="https://github.com/user-attachments/assets/cdf49353-667b-44ec-8e77-6329c441a8c1" />



