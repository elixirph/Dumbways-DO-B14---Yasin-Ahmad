MANAGE SERVER WITH TERMINAL

A. Perbedaan antara Shell dan BASH

Shell : di windows sebagai media untuk ragam kontrol file, lebih sederhana & cepat

Bash : untuk linux/unix sebgai penerjemah


B. BASH script untuk update dan upgrade server
1. buat file bash terlebih dahulu dengan command sudo nano file1 saya menamakannya dengan file1, kemudian inputkan script berikut: #!/usr/bin/env bash kemudian tambahkan command di dalamnya dengan command sudo apt update; sudo apt upgrade
untuk lebih jelasnya silahkan lihat gambar berikut ini : (jgn lupa simpan file dengan ekstensi .sh)

![Screenshot (145)](https://user-images.githubusercontent.com/117638290/203786964-ffc90c5c-1082-4ff3-a616-f431d1619029.png)

2. lalu coba jalankan file tersebut dengan command sh file1.sh seperti gambar di bawah ini:

![Screenshot (147)](https://user-images.githubusercontent.com/117638290/203787288-5c8825c4-757d-4121-a103-56c47042e455.png)

C. BASH script untuk memberi akses ke port 22,80,443

1. buat file lagi seperti sebelumnya, kali ini saya menamakannya dengan file2, lakukan kembali dengan command sudo nano file2
2. Lalu inputkan script seperti pada gambar & jangan lupa menambahkan ekstensi .sh pada filenya

![Screenshot (150)](https://user-images.githubusercontent.com/117638290/203787772-2e37dbcd-b587-470d-815f-593769028ccf.png)

3. Kemudian coba jalankan file tersebut dengan command sh file2.sh maka hasilnya akan seperti pada gambar 

![Screenshot (151)](https://user-images.githubusercontent.com/117638290/203788592-42400b2e-4f27-4dd0-b951-44e43c2d553b.png)


D. -Buatlah Script BASH dalam penggunaan cat, grep, echo & sort
   -Mengganti text 'Dumbways' ke 'Bootcamp'
  
1. Buat file baru dengan isi script running #!/usr/bin/env bash lalu isikan command-command cat, grep, echo & sort
untuk lebih jelasnya lihat gambar berikut & jangan lupa simpan setiap file script dengan ekstensi .sh

Pertama untuk command cat
![Screenshot (188)](https://user-images.githubusercontent.com/117638290/203809489-4585b33e-6e4d-403e-9994-98fc069977d5.png)
![Screenshot (187)](https://user-images.githubusercontent.com/117638290/203809902-cdab9ee6-b005-4a32-aaac-e992c7358368.png)


Command grep dalam script bash
![Screenshot (199)](https://user-images.githubusercontent.com/117638290/203811705-be426fe2-b33b-434d-90cf-db68e9148036.png)
![Screenshot (198)](https://user-images.githubusercontent.com/117638290/203811763-b82107d2-b670-4bef-aab0-88975b9d9afd.png)


Command echo dalam script bash
![Screenshot (200)](https://user-images.githubusercontent.com/117638290/203811987-39956075-bcaf-4de9-9883-4611f90c38b6.png)
![Screenshot (201)](https://user-images.githubusercontent.com/117638290/203812603-c7164d90-a6cb-42d3-bcf5-616fda303833.png)


Command sort dalam script
![Screenshot (196)](https://user-images.githubusercontent.com/117638290/203813460-ab106b05-72a6-45f3-8f30-3c58eb5cbc78.png)
![Screenshot (197)](https://user-images.githubusercontent.com/117638290/203813478-656b2a4b-04f1-4e2c-975a-23439095311d.png)


Mengganti teks dumbways ke bootcamp lihat gambar berikut ini & ikuti setiap commandnya
![Screenshot (158)](https://user-images.githubusercontent.com/117638290/203816111-3454a63a-5ff3-4695-a64d-b4fe712e0620.png)


E. Contoh penggunaan aplikasi monitoring

Disini saya menggunakan htop, install terlebih dahulu app dari monitoring dengan command sudo apt install htop -y lalu jalankan dengan command htop
lihat gambar untuk lebih jelasnya
![Screenshot (206)](https://user-images.githubusercontent.com/117638290/203816674-6cc7cacb-7c44-4133-acad-2f3409dc2f3c.png)
![Screenshot (205)](https://user-images.githubusercontent.com/117638290/203816692-e4d12bcf-dc8b-4cb8-b1fa-9d553ced1fec.png)


F. Buat script instalasi node version manager menggunakan BASH

buat file script baru dengan command nano node.sh kemudian inputkan command-command tersebut
![Screenshot (204)](https://user-images.githubusercontent.com/117638290/203815020-6e13bfd7-f55f-45e9-b3b0-f51cbb86e651.png)
![Screenshot (203)](https://user-images.githubusercontent.com/117638290/203815058-e392e682-22f6-450a-870d-40b99e26c1eb.png)
