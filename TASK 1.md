# Dumbways-DO-B14---Yasin-Ahmad
DevOps Introduction & Installing Ubuntu via VMWare
1.	Definisi DevOps
Devops merupakan development & operation, jadi menurut saya devops ini sebuah ruangan untuk bertukar informasi antara keduanya, dan dengan ruangan ini kerja dari masing-masing tim dapat berjalan baik karena adanya sebuah jalan pintas/ automasi dimana saat keduanya bekerja & ada masalah tidak mengganggu pekerjaan tim yang lain & aplikasi bisa tetap berjalan sebagaiman mestinya. 

![image](https://user-images.githubusercontent.com/117638290/202674253-5122e87f-1252-4fb8-9974-17959a2ae281.png)

2.	Sebutkan 2 lifecycle DevOps & jelaskan definisinya

![image](https://user-images.githubusercontent.com/117638290/202674351-a0abda51-f114-4b62-b6f7-433ab3e9a937.png)

a.	Planning, Pada tahap pertama, tim melakukan analisis kebutuhan proyek berdasarkan masukan dari pelanggan, departemen penjualan, hasil survei pemasaran, dan pandangan expert di industri tersebut. Data dan informasi yang terkumpul digunakan dalam perencanaan dan studi proyek dalam aspek ekonomi, operasional, dan teknikal.

b.	Deployment, produk selesai melalui proses deployment dan kemudian dirilis untuk segmen yang terbatas. produk mendapatkan berbagai umpan balik saat testing. Umpan balik tersebut digunakan untuk pengembangan software. Selanjutnya, produk dapat dirilis ke pasar dan melakukan aktivitas pemeliharaan produk secara berkala.

3.	Install Ubuntu Server (1 CPU, 2GB RAM & 20GB Storage (2GB untuk swap), setup ip static, install OpenSSH Server
a.	Pertama pilih Create a New File

![image](https://user-images.githubusercontent.com/117638290/202674682-e9eae350-3db7-4eeb-85cd-a6a3fbb357ce.png)

b.	Kedua browse file iso ubuntu server 20.04 yang telah di download, jika belum download silahkan download di web resmi ubuntu.com

![image](https://user-images.githubusercontent.com/117638290/202674730-9bcb40a5-6e70-49a9-aac8-e907702470f4.png)

c.	Ketiga, isi semua kolom sesuai keinginan kita dan klik next

![image](https://user-images.githubusercontent.com/117638290/202674775-d98fe8d4-7cf1-4fa2-a931-80e6a27a7abb.png)

d.	Selanjutnya, masukan nama virtual machine dan pilih lokasi atau target penyimpanan filenya, jika sudah ada secara default langsung saja

![image](https://user-images.githubusercontent.com/117638290/202674806-ac759438-c597-4705-8d23-6ba7cfea3bb9.png)

e.	Pilih jumlah kapasitas storage yang diinginkan, di sini saya memilih 20GB karena tugasnya di perintahkan 20GB, selanjutnya pilih virtual disk into multiple agar kita dengan mudah melakukan split atau seting kapasitas storage, next

![image](https://user-images.githubusercontent.com/117638290/202674829-339b514e-a318-4a33-a574-efc355e7f676.png)

f.	Pilih customize kemudian ubah network connection menjdi bridge, agar kita bisa mendapatkan ip default dan mengubahnya menjadi ip static, dan menggunakan 1 CPU sesuai dengan tugas yang diberikan, klik finish

![image](https://user-images.githubusercontent.com/117638290/202674869-5233b37d-b8ed-4a56-877b-b3f35d533f8f.png)

g.	Tunggu hingga proses selesai sampai menampilkan pilihan bahasa

![image](https://user-images.githubusercontent.com/117638290/202674906-15c1ea9a-e424-4a10-8ff8-7e9f943051d0.png)

h.	Pilih English kemudian tekan enter

![image](https://user-images.githubusercontent.com/117638290/202674938-46c027c5-ba46-4d3a-875f-2e71193c780b.png)

i.	Setelah itu skip 2 kali atau pilih done 2 kali sampai menampilkan konfigurasi network seperti ini, kemudian pilih ens33 & pilih ipv4, ubah itu menjadi manual

![image](https://user-images.githubusercontent.com/117638290/202674999-5b993670-6e73-45d9-8e93-d730655e165d.png)

j.	Tampilanny menjadi seperti ini, isi kolom-kolom tersebut sesuai ip masing-masing, cek ip di cmd dengan ipconfig (untuk windows) atau ifconfig (untuk ubuntu desktop) Sesuaikan denga ip gateway masing-masing, bisa diliat di contoh gambar tersebut, untuk subnet isikan denga nip gateway namun tidak pada angka dalam titik terakhir & ubah menjadi .0/24 agar kalian bis seting address di angka terakhir sampai 255, di sini saya memilih .231 & ingat batasnya hanya 255

![image](https://user-images.githubusercontent.com/117638290/202675018-8fc49817-6bdf-446b-8538-5dcbcda1d0bd.png)

k.	Hasilnya akan seperti ini, kalian akan mendapat ip static sesuai yang kalian inginkan pada angka terkhir static 172.10.48.231/24

![image](https://user-images.githubusercontent.com/117638290/202675040-0ee111e7-af18-4eaf-b8e5-51923cd47a3b.png)

l.	Kemudian klik atau pilih done 2kali sampai tampilan seperti ini, kemudian set 2gb untuk swap dan sisa 18gb (ubah menjadi GPT) kemudian done & pilih continue
 
![image](https://user-images.githubusercontent.com/117638290/202675079-73828b2f-1f4b-4aa6-8b1c-6de4ae9c8e16.png)

m.	Setelah itu kalian akan melihat tampilan seperti ini, isikan setiap kolom sesuai keinginan

![image](https://user-images.githubusercontent.com/117638290/202675098-7f719988-cde1-4a32-8919-b2639b05f11f.png)

n.	Selanjutnya install OpenSSH server kemudian pilih done

![image](https://user-images.githubusercontent.com/117638290/202675130-913167e8-c775-4a8d-941d-369250b457dc.png)

o.	Ini silahkan di next atau done saja

![image](https://user-images.githubusercontent.com/117638290/202675169-10151f1e-349e-4364-99f1-8e1564e88501.png)

p.	Tunggu sampai selesai

![image](https://user-images.githubusercontent.com/117638290/202675203-4047bc1e-c119-414b-b626-06653b1dddee.png)

q.	Selesai, kemudian reboot & login sesuai yang telah diisikan

![image](https://user-images.githubusercontent.com/117638290/202675247-c5f4d198-24f1-4d16-9f0d-e10b1dab0318.png)

r.	Selanjutnya cek apakah terkoneksi baik keinternet dengan command <ping google.com> jika muncul seperti dibawah berarti semua telah selesai 

![image](https://user-images.githubusercontent.com/117638290/202675288-b2dceda5-f3a9-4b48-a517-68416157fe3b.png)











