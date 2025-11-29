Weather Dashboard ini saya buat sebagai aplikasi web yang menampilkan informasi cuaca secara real-time dengan memanfaatkan OpenWeatherMap API. Tujuan utamanya adalah mempraktikkan bagaimana mengambil data dari web service menggunakan AJAX (melalui Fetch API), kemudian menampilkannya secara dinamis di halaman tanpa perlu reload. Selain itu, proyek ini juga menjadi latihan untuk menggabungkan antarmuka modern menggunakan TailwindCSS agar tampilannya bersih, responsif, dan nyaman digunakan.

Di dalam aplikasi ini, pengguna dapat mencari kota tertentu melalui kolom pencarian. Fitur pencarian sudah dilengkapi autocomplete yang akan menampilkan saran kota ketika pengguna mengetik setidaknya tiga karakter. Setelah kota dipilih, aplikasi langsung menampilkan data cuaca terkini seperti suhu, kondisi cuaca, kelembaban, dan kecepatan angin. Informasi tersebut ditampilkan dalam sebuah kartu utama yang dirancang agar mudah dibaca.

Selain cuaca saat ini, aplikasi juga menyediakan prakiraan cuaca lima hari. Setiap harinya ditampilkan dalam bentuk kartu kecil yang berisi tanggal, ikon cuaca, serta kisaran suhu minimum dan maksimum. Dengan cara ini, pengguna bisa mendapat gambaran umum kondisi cuaca beberapa hari ke depan hanya lewat satu tampilan.

Aplikasi ini juga mendukung pengaturan satuan suhu antara Celcius dan Fahrenheit. Perubahan satuan tidak hanya mengubah tampilan suhu, tetapi juga disimpan menggunakan LocalStorage supaya pengaturan tetap sama ketika halaman dibuka ulang. Hal yang sama juga diterapkan pada mode tampilan: pengguna bisa memilih untuk menggunakan tampilan terang atau gelap, dan preferensi tersebut akan diingat secara otomatis.

Untuk memudahkan pengguna, saya menambahkan fitur kota favorit. Kota yang ditandai akan masuk ke daftar favorit dan dapat dipilih kembali hanya dengan satu klik. Fitur ini sangat membantu untuk pengguna yang sering memeriksa kota yang sama. Seluruh daftar favorit disimpan di LocalStorage sehingga tidak hilang meskipun browser ditutup.

<img width="2560" height="1600" alt="Screenshot 2025-11-29 212637" src="https://github.com/user-attachments/assets/6ad258cf-968e-4260-bc1d-d7d079d04fc2" />
<img width="2560" height="1600" alt="Screenshot 2025-11-29 212620" src="https://github.com/user-attachments/assets/3c3fbedd-e38b-48a7-9202-beafa483909e" />

Dua tangkapan layar yang disertakan menunjukkan bagaimana tampilan aplikasi pada dua mode yang berbeda. Gambar pertama memperlihatkan tampilan mode gelap dengan nuansa warna yang lebih pekat, cocok digunakan di ruangan minim cahaya. Sedangkan gambar kedua memperlihatkan mode terang yang lebih cerah dan bersih. Perbedaan visual ini menunjukkan bahwa sistem tema berjalan dengan baik dan dapat menyesuaikan preferensi pengguna tanpa mengubah struktur halaman.

Aplikasi ini sepenuhnya berjalan di sisi klien. Untuk mencobanya, cukup buka file weather_dashboard_index.html di browser modern dan pastikan perangkat terhubung ke internet karena data cuaca diambil langsung dari API. Tidak ada proses instalasi tambahan.

Secara keseluruhan, proyek ini menjadi latihan yang cukup lengkap karena mencakup beberapa aspek penting: integrasi API eksternal, manipulasi DOM, penanganan event, penyimpanan data lokal, serta penerapan desain responsif dan tema dinamis. Melalui proyek ini, saya bisa mempraktikkan bagaimana membangun mini-aplikasi web yang fungsional, interaktif, dan tetap nyaman digunakan.
