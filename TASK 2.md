LINUX SHELL & COMPUTER NETWORKING

A. Perbedaan antara IP Private & Public? IP Private sebuah jaringan internet local atau pribadi dimana seseorang yang ingin terhubung secara bersamaan harus dalam satu lingkup koneksi yang sama & memerlukan bantuan router. Sedangkan ip public sebuah jaringan internet yang bisa diekspos secara global, dimana setiap orang diseluruh dunia yang memiliki internet dapat memiliki akses langsung & tidak mungkin ada ip public yang sama.

![image](https://user-images.githubusercontent.com/117638290/202678389-0a770465-2cce-48df-aedb-cae3c66c2165.png)

B. Perbedaan antara IP Dinamic & Static, ip dinamic dapat berubah-ubah karena di dapat secara default dari system DHCP atau dari isp itu sendiri, biasanya digunakan yang penting bisa internetan xD. Sedangkan ip static memiliki ip yang tetap, meskipun terkoneksi dalam beberapa jaringan yang berbedaa-beda karena telah dikonfigurasi secara manual, biasanya untuk bisnis perusahaan.

C. Deploy aplikasi web server apache menggunakan apt package

pertama inputkan command sudo apt update

![Screenshot (75)](https://user-images.githubusercontent.com/117638290/202679484-34912c19-1ce4-430d-aabc-464f963c46d5.png)

kedua input dengan command sudo apt install apache2

![Screenshot (78)](https://user-images.githubusercontent.com/117638290/202680460-0077a8cc-5666-471a-aaf8-66bf2765cdee.png)

ketiga cek dengan command apache2 -version

![Screenshot (76)](https://user-images.githubusercontent.com/117638290/202679862-d0b938a0-a9da-4d7e-9ab1-95885b1de318.png)

selanjutnya firewall konfigurasi, ketikkan command  sudo ufw app list

![Screenshot (81)](https://user-images.githubusercontent.com/117638290/202681107-3ec80681-e62d-49d8-84b8-725e42b1dd1c.png)

kemudian enable port 80 dengan command sudo ufw allow ‘Apache’

![Screenshot (83)](https://user-images.githubusercontent.com/117638290/202684728-7b4650b9-64ec-4ad1-a5b9-f1850eed7502.png)

Kemudian pastikan jika aplikasi apache telah berjalan dengan command sudo systemctl status apache2

![Screenshot (84)](https://user-images.githubusercontent.com/117638290/202685342-e43c5188-85e1-413a-b4c8-2e457cb054da.png)

Terakhir inputkan command hostname –I

![Screenshot (85)](https://user-images.githubusercontent.com/117638290/202685993-39aeaa0a-1960-4831-9d30-0465f03a2f3a.png)

Lalu copy ip tersebut & salin ke dalam browser kalian, maka hasilnya akan seperti ini

![Screenshot (32)](https://user-images.githubusercontent.com/117638290/202686363-d932cce4-f9a5-45a9-8010-4c3ea6ff5d75.png)


untuk melihat ip & silahkan copykan alamat ip ke web browser
