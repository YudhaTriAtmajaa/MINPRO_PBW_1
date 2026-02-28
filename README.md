# Portfolio Website - Yudha Tri Atmaja

Website portfolio pribadi yang dibuat menggunakan HTML, CSS, dan Bootstrap 5. Berisi informasi singkat tentang diri, pengalaman organisasi, skill, dan sertifikat yang pernah diperoleh.

---

## Tampilan Section

1. Navbar berisi YTAPorto pada sisi kiri dan menu navigasi ke tiga section utama (Home, About Me, Certificates). Navbar bersifat fixed sehingga tetap terlihat saat halaman di-scroll. Pada layar kecil, menu akan berubah menjadi menu button.
> <img width="1906" height="61" alt="image" src="https://github.com/user-attachments/assets/0787bc4c-5fcb-41ed-9e5d-9ec6b9582bc1" />

2. Home section pembuka yang menampilkan nama, deskripsi singkat sebagai mahasiswa Sistem Informasi Universitas Mulawarman, foto profil, serta dua tombol navigasi menuju section About Me dan Certificates.
> <img width="1904" height="930" alt="image" src="https://github.com/user-attachments/assets/6976d904-3bca-4dd3-97c4-3133667a4839" />

3. About Me berisi dua bagian utama. Bagian kiri memuat deskripsi diri secara singkat. Bagian kanan menampilkan daftar pengalaman organisasi dan kepanitiaan beserta tahun pelaksanaannya. Di bagian bawah terdapat blok Skills berupa progress bar yang menampilkan persentase kemampuan.
> <img width="1901" height="871" alt="image" src="https://github.com/user-attachments/assets/df6e7157-52f6-4dea-b2a1-817c7414858d" />

4. Certificates menampilkan koleksi sertifikat dalam format card grid, dibagi menjadi dua kelompok yaitu Organisasi dan Akademik. Setiap card memuat foto sertifikat, kategori, judul, penerbit, tahun, dan deskripsi singkat.
> <img width="1900" height="887" alt="image" src="https://github.com/user-attachments/assets/d952fad0-78e6-4f63-9807-bfe702aa5103" />

5. Footer menampilkan teks hak cipta beserta identitas pemilik portfolio.
> <img width="1903" height="89" alt="image" src="https://github.com/user-attachments/assets/136c3f27-5664-4812-a055-2e7fee2bd2f1" />

---

## Penjelasan Code

- ### Navbar 
Menggunakan komponen `navbar` dari Bootstrap dengan class `fixed-top` agar posisi tetap di bagian atas layar. Menu navigasi menggunakan anchor link (`#home`, `#about`, `#certificates`) untuk berpindah antar section.

- ### Home
Menggunakan grid Bootstrap dua kolom, `col-lg-7` untuk area teks dan `col-lg-5` untuk foto. Foto profil ditampilkan menggunakan tag `<img src="yuda.jpeg">` di dalam `div.photo-box`. Atribut `alt` diisi untuk keperluan aksesibilitas.

- ### About Me
Layout dua kolom Bootstrap untuk memisahkan deskripsi diri dan daftar pengalaman. Judul section menggunakan class `.section-title` dengan dekorasi garis bawah dari `div.title-underline`. Teks deskripsi menggunakan class `.about-text` dengan `text-align: justify`.

- ### Experience
Setiap item pengalaman menggunakan struktur `div.exp-item` yang terdiri dari `span.exp-year` untuk tahun, `div.exp-role` untuk nama jabatan, dan `div.exp-place` untuk nama organisasi yang disusun secara vertikal.

- ### Skills
Setiap skill menggunakan komponen `progress` dari Bootstrap. Persentase kemampuan ditampilkan melalui teks dan lebar bar yang diatur langsung via atribut `style="width: XX%"` pada elemen `div.progress-bar`. Skills yang ditampilkan:
1. MySQL & Database Design (80%)
2. Computer Network (75%)
3. HTML/CSS/JavaScript (40%)
4. Leadership (80%)
5. Problem Solving (75%)
6. Public Speaking (70%)

- ### Certificates
Sertifikat dikelompokkan menggunakan heading `h5.cert-sub-title` menjadi dua kategori: Organisasi dan Akademik. Setiap card menggunakan grid `col-md-6 col-lg-4` sehingga tampil 3 kolom di layar besar dan 2 kolom di tablet. Foto sertifikat ditampilkan langsung menggunakan tag `<img>`. Informasi sertifikat ditampilkan di `div.cert-info` yang berisi tag kategori, judul, penerbit, dan deskripsi.

- ### Footer
Menggunakan tag `<footer>` dengan teks copyright. Diberi border atas sebagai pemisah dari section terakhir.

---

## Penjelasan CSS

- **Style** - `box-sizing: border-box` diterapkan ke semua elemen. Body menggunakan font Poppins dengan background biru gelap `#0d1b4b` dan `padding-top: 64px` untuk mengimbangi navbar fixed.
- **Navbar** - Background lebih gelap dari body (`#091236`) untuk memberi kontras. Warna teks menggunakan transparansi putih dengan efek hover biru.
- **Home** - Section menggunakan `min-height: calc(100vh - 64px)` agar mengisi penuh layar. Foto profil menggunakan `object-fit: cover` di dalam `.photo-box` berukuran `420px × 520px` agar gambar tetap proporsional.
- **Certificate Card** - Efek hover menerapkan `translateY(-4px)` dan `box-shadow` biru agar card terlihat terangkat saat kursor diarahkan.

---

## Teknologi yang Digunakan

- HTML5
- CSS3
- Bootstrap 5.3.3
- Google Fonts (Poppins)
