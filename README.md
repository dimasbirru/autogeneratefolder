# autogeneratefolder
# Auto Rangkai Folder Tugas

Proyek sederhana berbasis web yang memungkinkan Anda membuat struktur folder tugas perkuliahan secara otomatis dan mengemasnya dalam format ZIP. Ini sangat berguna untuk mengatur folder mata kuliah dengan subfolder standar (Template Folder) seperti "Tugas", "Catatan", "Materi", dll., dalam satu langkah cepat.



## 🚀 Fitur Utama

* **Pembuatan Struktur Folder Cepat:** Otomatis membuat struktur folder untuk beberapa mata kuliah sekaligus.
* **Template Folder Kustom:** Anda dapat menambah, mengubah, atau menghapus subfolder template yang akan dibuat di dalam setiap folder mata kuliah.
* **Ekspor ZIP:** Struktur folder yang telah dibuat akan dikemas dalam file ZIP dan langsung diunduh ke komputer Anda.
* **Dependencies Ringan:** Hanya memerlukan library **JSZip** dan **FileSaver.js** yang dimuat dari CDN.

## 🛠️ Cara Menggunakan

### Persiapan

1.  Pastikan Anda memiliki tiga file berikut dalam satu direktori:
    * `index.html`
    * `style.css`
    * `script.js`
2.  Buka file `index.html` di *browser* modern mana pun (seperti Chrome, Firefox, Edge, dll.).

### Langkah-Langkah

1.  **Nama Folder Utama:** (Opsional) Masukkan nama untuk folder utama yang akan menampung semua folder mata kuliah.
    * *Contoh:* `Semester 5`
2.  **Masukkan Mata Kuliah:** Tuliskan nama-nama mata kuliah Anda, **satu per baris**.
    * *Contoh:*
        ```
        Pemrograman Web
        Basis Data
        Jaringan Komputer
        ```
3.  **Template Folder:** Lihat daftar folder template yang akan dibuat di dalam setiap folder mata kuliah.
    * Gunakan tombol **Tambah Folder Template** untuk menambahkan subfolder baru (misalnya: "Project Akhir").
    * Gunakan tombol **Hapus** pada item template untuk menghapus subfolder yang tidak diperlukan.
    * *Default Template:* `Tugas`, `Catatan`, `Materi`, `UTS`, `UAS`.
4.  **Generate ZIP:** Setelah selesai memasukkan input dan mengatur template, klik tombol **Generate ZIP**.
    * **Catatan:** Dalam kode saat ini, file ZIP juga akan otomatis di-*generate* ketika Anda selesai mengetik di area teks mata kuliah dan mengklik di luar area tersebut (*on blur*).

### Contoh Hasil

Jika Anda memasukkan:
* **Nama Folder Utama:** `Semester 5`
* **Mata Kuliah:** `Pemrograman Web`, `Basis Data`
* **Template Folder:** `Tugas`, `Catatan`

Maka struktur folder dalam file ZIP akan terlihat seperti ini: