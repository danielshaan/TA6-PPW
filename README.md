Weather Dashboard ini saya buat sebagai aplikasi web yang menampilkan informasi cuaca secara real-time dengan memanfaatkan OpenWeatherMap API. Proyek ini saya kerjakan untuk mempraktikkan cara mengambil data dari web service menggunakan AJAX (Fetch API) dan menampilkannya secara dinamis tanpa perlu memuat ulang halaman. Selain itu, saya juga menggabungkan antarmuka berbasis TailwindCSS agar tampilan aplikasi lebih rapi, responsif, dan nyaman dipakai baik di mode terang maupun mode gelap.

Aplikasi ini memungkinkan pengguna untuk mencari kota tertentu melalui kolom pencarian yang sudah dilengkapi fitur autocomplete. Setelah kota dipilih, aplikasi akan menampilkan informasi cuaca terkini secara lengkap, mulai dari suhu, deskripsi cuaca, kelembaban, hingga kecepatan angin. Semua elemen UI disusun mengikuti pola kartu sehingga mudah dibaca dan tidak membuat tampilan terasa penuh.

Agar pengguna bisa melihat kondisi cuaca ke depan, aplikasi ini juga menampilkan prakiraan lima hari yang ringkas. Setiap harinya ditampilkan dalam kartu kecil berisi ikon cuaca, suhu minimum dan maksimum, serta tanggal. Dengan begitu, pengguna bisa langsung memahami pola cuaca tanpa harus membuka halaman tambahan.

Untuk menjaga kenyamanan pengguna, saya menambahkan sistem penyimpanan preferensi menggunakan LocalStorage. Setiap perubahan satuan suhu ataupun mode tampilan akan disimpan, sehingga ketika halaman dibuka kembali, aplikasi langsung menampilkan pengaturan sesuai yang terakhir digunakan. Hal yang sama juga berlaku untuk daftar kota favorit, sehingga pengguna tidak perlu menandai ulang setiap kali membuka ulang aplikasinya.

Berikut beberapa fitur utama yang saya implementasikan:
- Pencarian kota dengan autocomplete, lengkap dengan pemilihan lokasi yang akurat melalui data geocoding.
- Tampilan cuaca terkini yang mencakup suhu, deskripsi kondisi, kelembaban, kecepatan angin, dan ikon cuaca.
- Prakiraan cuaca lima hari yang dirangkum dalam bentuk kartu agar mudah dibaca.
- Pengaturan satuan suhu (°C dan °F) yang bisa diganti kapan saja dan disimpan otomatis.
- Mode terang dan gelap dengan penyimpanan preferensi pengguna di LocalStorage.
- Daftar kota favorit yang dapat ditambahkan dan dipilih kembali dengan cepat.
- Auto-refresh setiap lima menit untuk memastikan data cuaca selalu terbaru.

<img width="2560" height="1600" alt="Screenshot 2025-11-29 212637" src="https://github.com/user-attachments/assets/6ad258cf-968e-4260-bc1d-d7d079d04fc2" />
<img width="2560" height="1600" alt="Screenshot 2025-11-29 212620" src="https://github.com/user-attachments/assets/3c3fbedd-e38b-48a7-9202-beafa483909e" />

Dua tangkapan layar yang saya sertakan dalam README menunjukkan bagaimana aplikasi tampil dalam dua mode tema. Gambar pertama menampilkan mode gelap dengan nuansa warna yang lebih redup dan nyaman untuk penggunaan di ruangan gelap. Sementara gambar kedua menunjukkan mode terang yang terlihat lebih cerah, bersih, dan modern. Perbedaan kedua gambar ini menegaskan bahwa sistem tema berjalan dengan baik tanpa mengubah struktur tampilan dan fungsi aplikasi.

Semua proses aplikasi ini berjalan sepenuhnya di sisi klien. Untuk menjalankannya, cukup buka file weather_dashboard_index.html melalui browser modern dan pastikan perangkat memiliki koneksi internet karena data cuaca diambil langsung dari API OpenWeatherMap.
