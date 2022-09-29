1. Unduh dan ekstrak data Kit Mulai Cepat Natural Earth. Buka QGIS. Temukan folder mulai cepat Natural Earth di panel Browser. Luaskan folder untuk menemukan proyek Natural_Earth_quick_start_for_QGIS_v3. Ini adalah file proyek yang berisi lapisan bergaya dalam format Dokumen QGIS. Klik dua kali proyek untuk membukanya.

2. Gunakan kontrol geser dan zoom di Bilah Alat Navigasi Peta dan perbesar ke Pulau Sumatera.

3. Anda dapat menonaktifkan beberapa lapisan peta untuk data yang tidak kami perlukan untuk peta ini. Luaskan folder z5 - 1:18m dan hapus centang pada kotak di sebelah lapisan ne_10m_geography_marine_polys dan ne_10m_admin_0_disputed_areas. Sebelum kita membuat peta yang cocok untuk dicetak, kita perlu memilih proyeksi yang sesuai. CRS default untuk proyek diatur ke EPSG:3857 Pseudo-Mercator. Ini adalah CRS yang populer digunakan untuk pemetaan web dan merupakan pilihan yang layak untuk tujuan kita, sehingga kita dapat membiarkannya pada nilai defaultnya. Pergi ke Proyek Tata Letak Cetak Baru.

4.Anda akan diminta untuk memasukkan judul untuk tata letak. Anda dapat membiarkannya kosong dan klik Ok.

5. Di jendela Print Layout, klik tombol Zoom full untuk menampilkan seluruh Layout.

6. Sekarang kita harus membawa tampilan peta yang kita lihat di Kanvas QGIS ke tata letak. Pergi ke Tambah Item Go to Add Item ‣ Add Map.

7. Setelah mode Add Map aktif, tahan tombol kiri mouse dan seret persegi panjang di mana Anda ingin menyisipkan peta.

8. Anda akan melihat bahwa jendela persegi panjang akan ditampilkan dengan peta dari kanvas QGIS utama. Peta yang diberikan mungkin tidak mencakup seluruh area minat kami. Gunakan opsi Edit Pilih/Pindahkan item dan Edit Pindahkan Konten untuk menggeser peta di jendela dan memusatkannya di komposer.

9. Mari kita juga menyesuaikan tingkat zoom untuk peta. Klik pada tab Item Properties dan masukkan 10000000 sebagai nilai Skala  

10. Sekarang kita akan menambahkan inset peta yang menunjukkan tampilan yang diperbesar untuk area Tokyo. Sebelum kita membuat perubahan pada lapisan di jendela utama QGIS, centang kotak Kunci lapisan dan Gaya kunci untuk lapisan. Ini akan memastikan bahwa jika kita mematikan beberapa lapisan atau mengubah gayanya, tampilan ini tidak akan berubah.

11. Beralih ke jendela QGIS utama. Matikan grup layer z5 - 1:18m dan aktifkan grup z7 - 1:4m. Grup lapisan ini memiliki gaya yang lebih sesuai untuk tampilan yang diperbesar. Gunakan kontrol pan dan zoom di Map Navigation Toolbar dan zoom di sekitar Kab Padang Pariman.

12. Kita sekarang siap untuk menambahkan inset peta. Ganti jendela Print Layout. Pergi ke Add Item ‣ Add Map.
Seret persegi panjang di tempat Anda ingin menambahkan inset peta. Anda sekarang akan melihat bahwa kami memiliki 2 objek peta di Tata Letak Cetak. Saat membuat perubahan, pastikan Anda memilih peta yang benar.

13. Pilih objek Map 2 yang baru saja kita tambahkan dari panel Items. Pilih tab Properti item. Gulir ke bawah ke panel Frame dan centang kotak di sebelahnya. Anda dapat mengubah warna dan ketebalan batas bingkai sehingga mudah dibedakan dengan latar belakang peta.

14. Salah satu fitur rapi dari Tata Letak Cetak adalah ia dapat secara otomatis menyorot area dari peta utama yang diwakili di sisipan. Pilih objek Map 1 dari panel Items. Di tab Properti item, gulir ke bawah ke bagian Ikhtisar. Klik tombol Tambahkan ikhtisar baru.

15. Pilih Map 2 sebagai Bingkai Peta. Ini memberitahu Print Layout untuk menyorot objek Map 1 saat ini dengan luasnya peta yang ditampilkan di objek Map 2.

16. Sekarang setelah kita menyiapkan inset peta, kita akan menambahkan grid ke peta utama. Pilih objek Map 1 dari panel Items. Di tab Properti item, gulir ke bawah ke bagian Kisi. Klik tombol Add a new grid, diikuti oleh Modify grid….

17. Secara default, garis kisi menggunakan unit dan proyeksi yang sama dengan proyeksi peta yang dipilih saat ini. Namun, lebih umum dan berguna untuk menampilkan garis kisi dalam derajat. Kita dapat memilih CRS yang berbeda untuk grid. Klik tombol Change… di sebelah CRS.

18. Dalam dialog Pemilih Sistem Referensi Koordinasi, masukkan 4326 di kotak Filter. Dari hasil, pilih WGS84 EPSG:4326 sebagai CRS. Klik Oke.

19. Pilih nilai Interval sebagai 5 derajat di kedua arah X dan Y. Anda dapat menyesuaikan Offset untuk mengubah tempat munculnya garis kisi.

20. Gulir ke bawah ke bagian Bingkai kisi dan centang kotak Gambar koordinat. Format default adalah Derajat tetapi muncul sebagai angka. Kita dapat menyesuaikan adalah dengan menambahkan simbol °. Pilih Kustom dan klik tombol Ekspresi di sebelahnya.

21. Masukkan ekspresi berikut untuk membuat string yang mengambil nomor grid dan menambahkan simbol ° ke dalamnya. "concat(ke_string(@grid_number), '° ')".

22. Perhatikan bahwa kisi sekarang memiliki label khusus dari ekspresi. Sesuaikan pengaturan posisi Kiri, Kanan, Atas dan Bawah sesuai keinginan Anda.

23. Sekarang kita akan menambahkan bingkai Rectangluar untuk menampung elemen peta lainnya seperti panah utara, skala, dan label. Pergi ke Add Item Add Shape Add Rectangle.

24. Anda dapat mengubah Gaya persegi panjang agar sesuai dengan latar belakang peta.

25. Sekarang kita akan menambahkan Panah Utara ke peta. QGIS hadir dengan koleksi gambar terkait peta yang bagus - termasuk banyak jenis Panah Utara. Klik Tambah Item Tambah Gambar.

26. Sambil menahan tombol kiri mouse Anda, gambarlah sebuah persegi panjang. Di panel sebelah kanan, klik pada tab Item Properties dan perluas bagian Search directory dan pilih gambar yang Anda sukai.

27. Sekarang kita akan menambahkan bilah skala. Klik Add Item Add Scalebar.

28. Klik pada tata letak tempat Anda ingin bilah skala muncul. Di tab Item Properties, pastikan Anda telah memilih elemen peta Map 1 yang benar untuk menampilkan bilah skala. Pilih Gaya yang sesuai dengan kebutuhan Anda. Di panel Segmen, ubah Lebar tetap menjadi 200 unit dan sesuaikan segmen sesuai keinginan Anda.

29. Saatnya memberi label pada peta kita. Klik Tambah Item Tambah Label.

30. Klik pada peta dan gambar kotak di mana label seharusnya berada. Di tab Properti Item, perluas bagian Label dan masukkan label untuk peta. Demikian pula, tambahkan label lain untuk data dan kredit perangkat lunak.

31. Setelah Anda puas dengan peta, Anda dapat mengekspornya sebagai Gambar, PDF, atau SVG. Untuk tutorial ini, mari kita ekspor sebagai gambar. Klik Tata Letak Ekspor sebagai Gambar.

32. Simpan gambar dalam format yang Anda sukai. Di bawah ini adalah gambar PNG yang diekspor.
