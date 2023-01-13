# Task : Application in Server


## 1. Menjalankan aplikasi Webserver (nginx/apache2)

* #### Buka browser dan masukkan ip dari server.
![01](assets/1.jpg)


## 2. Menjalankan 3 aplikasi "hello world" menggunakan nodejs, golang dan python

### nodejs
Pertama-tama kita harus meng-install terlebih engine-nya dahulu. Untuk instalasi kalian bisa menggunakan beberapa perintah dibawah ini.
![01](assets/2.jpg)

keterangan : disini kita menggunakan nvm

nvm merupakan singkatan dari Node Version Manager. nvm adalah sebuah program yang akan membantu kita untuk menggunakan lebih dari satu versi Nodejs di dalam satu komputer..

![01](assets/28.jpg)

keterangan : Jika nvm belum terdeteksi gunakan perintah di atas ini

![02](assets/29.jpg)

keterangan : perintah di atas berguna untuk menginstall node.js dengan versi 16. Jika kalian ingin menggunakan node.js denganversion 14, maka Jalankan perintah nvm install 14.

![03](assets/3.jpg)

keterangan : Untuk menggunakan node.js dengan versi 16

Jika tahapan di atas sudah kalian lakukan, maka kalian sudah berhasil untuk melakukan instalasi node.js. Untuk melakukan pengecekan kalian bisa menggunakan perintah di bawah ini.

![04](assets/4.jpg)

Selanjutnya kita akan menjalankan perintah npm init gunanya untuk mengisiasi project, Hasil dari kalian menjalankan perintah akan membuat file baru dengan nama package.json, package.json ini berisikan isi informasi dari aplikasi yang akan kalian buat.

mkdir my-app-nodejs

![05](assets/5.jpg)

Selanjutnya kita akan menginstall Express JS. Express JS adalah framework dari NodeJS yang dirancang secara fleksibel dan sederhana untuk membantu tahap pengembangan aplikasi back end. Menginstall express js dapat dilakukan menggunakan NPM dengan perintah berikut:

![06](assets/6.jpg)

Jika sudah buat file dengan nama index.js, lalu masukan script dibawah ini

nano index.js

![07](assets/7.jpg)

Jika sudah sekarang kita akan coba untuk menjalankan aplikasi sederhana yang sudah kita buat. Untuk menjalankan dapat menggunakan perintah berikut ini.

![08](assets/8.jpg)

keterangan : untuk keluar bisa menggunakan CTRL + X

Sekarang coba akses web browser kalian setelah itu kalian coba akses dengan ip server:3000 dan jika dilokal coba akses dengan localhost:3000

![08](assets/9.jpg)

### golang
Pertama-tama sama seperti sebelumnya, kita harus mendownload engine-nya terlebih dahulu.
![08](assets/30.jpg)
![09](assets/31.jpg)

Selanjutnya masukkan path go pada .bashrc

![10](assets/10.jpg)
![11](assets/11.jpg)

Jika sudah sekarang dapat verifikasi go dengan cara berikut.
![12](assets/12.jpg)

Sekarang kita akan membuat aplikasi sederhana menggunakan go. Kalian dapat menjalankan beberapa perintah berikut ini.

![13](assets/14.jpg)

Setelah itu masukkan script dibawah ini.

![14](assets/13.jpg)

Sekarang jalankan aplikasi go dengan menggunakan perintah berikut.

![15](assets/15.jpg)

### python
Pertama-tama kita harus install terlebih dahulu Pyhton3. Untuk instalasi ikuti beberapa perintah di bawah ini.
![16](assets/16.jpg)

Python3 sudah ada secara default, untuk melakukan pengecekan jalankan perintah berikut.

![17](assets/17.jpg)

Sekarang kita install package manager dari python3. Kalian dapat menggunakan perintah berikut ini.

![18](assets/19.jpg)
![19](assets/20.jpg)
![20](assets/21.jpg)
![21](assets/22.jpg)

Jika sudah sekarang jalankan aplikasi dengan menggunakan perintah berikut ini.

![22](assets/23.jpg)

Sekarang coba akses web browser kalian setelah itu kalian coba akses dengan curl 127.0.0.1:5000

![23](assets/24.jpg)

keterangan : untuk case ini karena gak bisa melakukan localhost dibrowser jika python akan tetapi aksesnya dicli ubuntu server dengan curl 127.0.0.1:5000

## 3. Gunakan localtunnel untuk menjalankan "Hello world!" nodejs
![24](assets/25.jpg)
![25](assets/26.jpg)
![26](assets/27.jpg)

