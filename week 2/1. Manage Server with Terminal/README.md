# Task : Manage Server with Terminal


## 1. Apa itu terminal
Terminal adalah interface di mana Anda bisa mengetikkan baris-baris perintah berbasis teks untuk sistem operasi Linux. Biasanya, sebutan lain terminal adalah Shell. Jika Anda familiar dengan OS Windows, Terminal pada Linux memiliki fungsi yang mirip dengan CMD (Command Prompt). 
Terminal memungkinkan pengguna komputer untuk menjalankan berbagai fungsi pada komputer melalui baris-baris perintah. Walaupun saat ini kebanyakan sistem operasi sudah memiliki tampilan grafis, tapi hal itu terkadang belum cukup. Ada beberapa fungsi yang hanya dapat Anda jalankan dengan baris perintah, di sinilah peran Terminal dalam membantu Anda. 

## 2. BASH script untuk update dan upgrade server, lalu install nginx/apache2

* #### Pertama lihat list di dalam ubuntu kita
![01](assets/30.jpg)

* #### Ketik nano (nama_file) pada kasus saya ini saya buat nama file update_upgrade_server.sh. Lalu masukkan perintah untuk update dan upgrade server juga install nginx di ubuntu.
![02](assets/2.jpg)

* #### Jika sudah tersimpan pada list direktori akan terbuat file update_upgrade_server.sh..
![03](assets/3.jpg)

* #### Untuk menjalankan bash script di ubuntu server gunakan perintah sh nama_file (update_upgrade_server.sh). Maka proses akan dilakukan secara otomatis oleh server kita.
![04](assets/4.jpg)

## 3. BASH script untuk memberi akses ke port 22,80,443
* #### Untuk memberikan akses port kita harus mengecek dahulu apakah settingan firewall diubuntu server kita sudah active atau belum dengan perintah sudo ufw status. Maka akan muncul tulisan active atau inactive.
![05](assets/5.jpg)

* #### Buat file untuk menjalankan bash script. Pada kasus ini saya beri nama allow_22_80_443.sh..
![06](assets/6.jpg)

* #### Masukkan perintah sudo ufw allow (port_yang_di_allow) pada file allow_22_80_443.sh. sudo ufw allow bertujuan untuk memberikan akses untuk port 22, 80, dan 443 untuk bisa diakses dari luar server ubuntu kita
![07](assets/7.jpg)

* #### Untuk memastikan bahwa perintah yang kita jalankan nantinya bisa berjalan dengan lancar. Coba cek ulang perintah yang kita masukkan di file allow_22_80_443.sh. Dengan perintah cat allow_22_80_443.sh
![08](assets/8.jpg)

* #### Pertama coba terlebih dahulu untuk ssh ke server ubuntu kita melalui cmd. Maka akan muncul pesan error pada saat kita mau akses melalui ssh, dikarenakan pada server ubuntu kita belum memberikan akses port 22 untuk diakses melalui luar server dari ubuntu kita
![09](assets/9.jpg)

* #### Untuk menkalankan perintah bash script cukup dengan sh nama_file (allow_22_80_443.sh). Maka akan muncul tulisan "Rule added" yang artinya memberikan akses port kita untuk diakses dari luar server ubuntu sudah berhasil
![10](assets/10.jpg)

* #### Untuk mengeceknya apakah sudah berhasil atau belum, bisa kita coba untuk ssh di ubuntu server kita. Jika sudah berhasil untuk mengakses server ubuntu melalui ssh. Berarti akses port dari luar server ubuntu sudah berhasil
![11](assets/11.jpg)

## 4. Tugas text manipulation

* ### - contoh penggunaan cat, grep, echo & sort
* ### - mengganti text 'Dumbways' ke 'Bootcamp'

1. Cat 

* ### cat (file-name)
![12](assets/12.jpg)

keterangan : untuk melihat isi dari suatu file

* ### cat > (file-name)
![13](assets/13.jpg)

keterangan : untuk membuat suatu file baru serta memasukkan teks, Jika sudah menambakan teks kalian dapat keluar dengan klik CTRL + C.

* ### cat file1 file2 > file3
![14](assets/14.jpg)

keterangan : untuk menggabungkan dua buah file, dan menyimpannya ke dalam file3

2. Send 

* ### sed -i 's/hallo dumbways/Bootcamp/g' file3
![15](assets/15.jpg)

keterangan : mengganti semua kata hallo dumbways menjadi Bootcamp pada file3

3. Grep

* ### grep Bootcamp file3
![16](assets/16.jpg)

keterangan : akan mencari kata Bootcamp pada file3

* ### grep -c Bootcamp file3
![17](assets/17.jpg)

keterangan : akan menghitung jumlah kata “Bootcamp” pada filetiga

* ### grep Bootcamp *
![18](assets/18.jpg)

keterangan : akan mencari semua file yang berisikan kata Bootcamp

4. Echo & Short

* ### sort file4
![19](assets/19.jpg)

keterangan : untuk mengurutkan berdasarkan ascending

* ### sort -r file4
![20](assets/20.jpg)

keterangan : untuk mengurutkan berdasarkan descending

* ### echo "Hello Dumbways!"
![21](assets/21.jpg)

keterangan : untuk mencetak string **

* ### echo "Hello Dumbways!" >> file3
![22](assets/22.jpg)

keterangan : untuk mencetak kata Hello Dumbways! di file

* ### echo "Replace semua data" > file5
![23](assets/23.jpg)

keterangan : untuk mereplace semua data di file5 dan menggantinya dengan "Replace semua data"

## 4. Gunakan nmon untuk tampilkan CPU usage, RAM usage, Disk dan Resources OS & Proc
![24](assets/24.jpg)
![25](assets/25.jpg)
![26](assets/26.jpg)
