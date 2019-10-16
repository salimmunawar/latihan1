" Latihan 1 "
Menambahkan Global Config
Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user.name dan user.email • konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository. • apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit
Config Global Repository $ git config --global user.name “nama_user” $ git config --global user.email “nama_user”
Membuat Reposiory Local
Buka direktory aktif, misal: c:\user\iip\lab_pemrograman (buka menggunakan Windows Explorer)
klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash, sehingga muncul git bash command
Buat direktory project praktikum pertama dengan nama latihan1 $ mkdir latihan1 $ cd latihan1
Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah cd (change directory) • direktory aktif menjadi: c:\user\iip\lab_pemrograman\latihan1
Jalankan perintah git init, untuk membuat repository local. $ git init
Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .git
Pada direktori tersebut, semua perubahan pada working directory akan disimpan.
Menambahkan File baru pada repository
Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)
disini kita akan coba buat satu file bernama README.md (text file) $ echo “#Latihan 1” >> README.md
File README.md berhasil dibuat. 

![Capture](https://user-images.githubusercontent.com/44824152/66884174-8a242d80-effa-11e9-966b-8363668f39e2.PNG)

Menambahkan File baru pada repository
Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add. $ git add README.md
File README.md berhasil ditambahkan.

![Capture1](https://user-images.githubusercontent.com/44824152/66884277-ef781e80-effa-11e9-8129-245b4fcc75b3.PNG)


Commit (Menyimpan perubahan ke database)
Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah git commit -m “komentar commit” $ git commit -m “File pertama saya”

![Capture2](https://user-images.githubusercontent.com/44824152/66884332-0e76b080-effb-11e9-8406-07fc622a7f41.PNG)


Perubahan berhasil disimpan.
Membuat repository server
Server reopsitory yang akan kita gunakan adalah http://github.com • Anda harus membuat akun terlebih dahulu.
Pada laman github, klik tombol start a project, atau
Dari menu (icon +) klik New Repositori.

![capture3](https://user-images.githubusercontent.com/44824152/66884397-47168a00-effb-11e9-9909-617ee6ae3432.png)


Isi nama repositorynya, misal: lab_prog1.
lalu klik tombol Create repositor.

![capture4](https://user-images.githubusercontent.com/44824152/66884444-69a8a300-effb-11e9-8532-77b0db88b435.png)


Menambahkan Remote Repository
Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.
Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url] $ git remote add origin https://github.com/itsrifki/lab_prog1
Push (Mengirim perubahan ke server)
Untuk mengirim perubahan pada local repository ke server gunakan perintah git push. $ git push -u origin master
Perintah ini akan meminta memasukkan username dan password pada akun github.com 

![Capture5](https://user-images.githubusercontent.com/44824152/66884555-d2901b00-effb-11e9-8ade-b2d96771806c.PNG)

Melihat hasilnya pada server repository
Buka laman github.com, arahkan pada repositorinya.
Maka perubahan akan terlihat pada laman tersebut. 

![capture6](https://user-images.githubusercontent.com/44824152/66884766-6530ba00-effc-11e9-928b-ebfeb84fece0.png)

Clone Repository
Clone repository, pada dasarnya adalah meng-copy repository server dan secara otomatis membuat satu direktory sesuai dengan nama repositorynya (working directory).
Untuk melakukan cloning, gunakan perintah git clone [url] 


![Capture7](https://user-images.githubusercontent.com/44824152/66884788-7a0d4d80-effc-11e9-98fd-bed2be32f121.PNG)





