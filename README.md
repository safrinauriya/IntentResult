# Intent
Intent adalah sebuah kelas dalam programming Android yang berfungsi untuk perpindahan halaman. Intent juga merupakan suatu objek yang terdapat dalam suatu activity dimana objek tersebut dapat komunikasi dengan activity yang lain, baik activity pada fungsi internal android misal seperti memanggil activity dalam satu package atau beda package yang masih berada dalam satu project.
Fungsi Intent
-	Untuk berpindah halaman dari satu Activity ke Activity lain. Contohnya : Kita membuat aplikasi dengan 3 Activity. Activity utama berisi tombol informasi dan login. Ketika tombol informasi di klik akan tampil activity informasi begitupun dengan tombol login ketika di klik akan menampilkan activity login.
-	Untuk transfer data dari satu Activity ke Activity lain. Contohnya : Pada saat kita mengisi data pada Activity login maka nanti akan ditampilkan informasinya pada Activity infomasi user.
-	Untuk memanggil activity pada internal android seperti Melakukan Dial Number, Open Email ataupun lainnya.

Intent memiliki dua bentuk yaitu:
1.	Explicit Intent adalah tipe Intent yang digunakan untuk menjalankan komponen dari dalam sebuah aplikasi. Explicit intent bekerja dengan menggunakan nama kelas yang dituju misal : com.dicoding.activity.DetailActivity. Umumnya intent ini digunakan untuk mengaktifkan komponen pada satu aplikasi.
2.	Implicit Intent adalah tipe intent yang tidak memerlukan detail nama kelas yang ingin diaktifkan. Model ini memungkinkan komponen dari aplikasi lain bisa merespon request intent yang dijalankan. Penggunaan tipe intent ini umumnya diperuntukkan untuk menjalankan fitur/fungsi dari komponen aplikasi lain. Contohnya ketika kita membutuhkan fitur untuk mengambil foto. Daripada membuat sendiri fungsi kamera, lebih baik kita menyerahkan proses tersebut pada aplikasi kamera bawaan dari peranti atau aplikasi kamera lain yang telah terinstal sebelumnya di peranti. Hal yang sama misalnya ketika kita membutuhkan fungsi berbagi konten. Kita bisa memanfaatkan intent untuk menampilkan aplikasi mana saja yang bisa menangani fitur tersebut. Implementasi implicit intent ini akan sangat memudahkan bagi pengembang agar tetap fokus pada proses bisnis inti dari aplikasi yang dikembangkan.

# Intent Result
Berbeda dengan project intent sebelumnya, Intent Result ini dapat mengirim data ke activity lainnya. Data tersebut bisa berupa String, int, float, double, byte, char, dsb. Tidak semua tipe data mendukung untuk dikirim, ada beberapa data yang tidak bisa dikirim menggunakan Intent atau Bundle seperti data yang berukuran besar, yaitu gambar (image bitmap) atau file, tidak bisa dikirim antar Activity. Ada 2 cara untuk mengirimkan data/nilai antar activity didalam aplikasi Android, yaitu dengan menggunakan Intent dan Bundle, keduanya mempunyai fungsi yang sama, yaitu untuk passing data, tetapi dengan menggunakan Bundle, akan terlihat lebih rapi, karena dikemas terlebuh dahulu didalam bundle sebelum dikirimkan.

# Contoh penerapan Intent

Tampilan teks yang ingin dimasukkan, yang nantinya akan dikirim dan ditampilkan di activity lainnya. Button "save text" untuk menyimpan data teks yang akan dikirimkan pada halaman activity kedua.

![Screenshot_20210225-215636_IntentResult](https://user-images.githubusercontent.com/60589670/109184752-e0de7180-77c1-11eb-8921-7d6d111f5e38.jpg)

Tampilan teks yang dikirim dari activity pertama, kemudian button "edit text" untuk menyunting teks yang kemudian akan dialihkan pada halaman activity petama.

![Screenshot_20210225-215642_IntentResult](https://user-images.githubusercontent.com/60589670/109184737-dde38100-77c1-11eb-93f7-c9fbfeed0812.jpg)
