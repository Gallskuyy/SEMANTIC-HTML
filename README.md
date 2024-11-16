# SEMANTIC-HTML
Latihan praktikum 1 SEMANTIC HTML

**Semantic HTML Project**
  
  Project ini berfokus pada penerapan struktur SEMANTIC HTML. Penggunaan Semantic HTML dapat menggantikan fungsi div dengan atributnya, sehingga baris kode menjadi lebih ringkas.

## index.html
### kekurangan
1. Tag pembuka <html> hilang atribut lang, seperti (html lang="en").
2. Tag (body) hilang, tag (header), (nav), (section), (footer) seharusnya berada di dalam tag (body).
   
### Perbaikan
1. Tag (html) dan (body) diperbaiki dan dilengkapi.
2. Tag (head) ditambahkan untuk memasukkan metadata, judul halaman, dan pengaturan karakter.

## styles.css
### Kekurangan
1. Selector Header, Nav, Section, Footer Tidak Spesifik:

   Elemen header, nav, section, dan footer diatur tanpa memastikan apakah mereka ada dalam elemen body. Akan lebih baik jika menggunakan selektor yang lebih spesifik untuk menghindari kemungkinan konflik dengan elemen di tempat lain.


3. Warna Latar Belakang Tidak Berkontras Tinggi:

   Warna latar belakang yang dipilih (#C9BFBF, #707070, dan #ABABAB) mungkin kurang kontras, terutama di area header dan footer. Hal ini bisa membuat teks atau elemen lain sulit dibaca.


4. Kurang Fleksibel untuk Tampilan Responsif:
   
   Pengaturan grid-template-areas, grid-template-rows, dan grid-template-columns bersifat statis dan tidak fleksibel pada perangkat dengan ukuran layar lebih kecil, seperti tablet atau handphone.


5. grid-gap vs gap:
   
   grid-gap adalah cara lama untuk menambahkan jarak antar-elemen pada CSS Grid, yang sekarang sudah digantikan dengan properti gap agar lebih fleksibel dan seragam dalam CSS Grid dan Flexbox.


6. height: 100vh pada Body:
   
   Penggunaan height: 100vh pada body bisa bermasalah pada perangkat seluler karena bisa menyebabkan pemotongan pada konten saat tampilan berubah akibat bilah navigasi atau bilah alat. Menggunakan min-height bisa lebih aman untuk tampilan yang lebih fleksibel.


7. Elemen yang Tidak Terpusat Vertikal:
   
   Pada header, footer, atau section, mungkin lebih baik jika konten di dalamnya dipusatkan secara vertikal. Ini bisa dilakukan dengan menambahkan display: flex dan align-items: center ke elemen-elemen ini.
