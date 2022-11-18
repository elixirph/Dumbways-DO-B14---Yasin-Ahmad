# Dumbways-DO-B14---Yasin-Ahmad
TASK (DevOps Introduction & Installing Ubuntu via Vmware)
1.	Definisi DevOps
Devops merupakan development & operation, jadi menurut saya devops ini sebuah ruangan untuk bertukar informasi antara keduanya, dan dengan ruangan ini kerja dari masing-masing tim dapat berjalan baik karena adanya sebuah jalan pintas/ automasi dimana saat keduanya bekerja & ada masalah tidak mengganggu pekerjaan tim yang lain & aplikasi bisa tetap berjalan sebagaiman mestinya. 

![image](https://user-images.githubusercontent.com/117638290/202674253-5122e87f-1252-4fb8-9974-17959a2ae281.png)

2.	Sebutkan 2 lifecycle DevOps & jelaskan definisinya

![image](https://user-images.githubusercontent.com/117638290/202674351-a0abda51-f114-4b62-b6f7-433ab3e9a937.png)

a.	Planning, Pada tahap pertama, tim melakukan analisis kebutuhan proyek berdasarkan masukan dari pelanggan, departemen penjualan, hasil survei pemasaran, dan pandangan expert di industri tersebut. Data dan informasi yang terkumpul digunakan dalam perencanaan dan studi proyek dalam aspek ekonomi, operasional, dan teknikal.

b.	Deployment, produk selesai melalui proses deployment dan kemudian dirilis untuk segmen yang terbatas. produk mendapatkan berbagai umpan balik saat testing. Umpan balik tersebut digunakan untuk pengembangan software. Selanjutnya, produk dapat dirilis ke pasar dan melakukan aktivitas pemeliharaan produk secara berkala.

3.	Install Ubuntu Server (1 CPU, 2GB RAM & 20GB Storage (2GB untuk swap), setup ip static, install OpenSSH Server
a.	Pertama pilih Create a New File












b.	Kedua browse file iso ubuntu server 20.04 yang telah di download, jika belum download silahkan download di web resmi ubuntu.com













c.	Ketiga, isi semua kolom sesuai keinginan kita dan klik next












d.	Selanjutnya, masukan nama virtual machine dan pilih lokasi atau target penyimpanan filenya, jika sudah ada secara default langsung saja

















e.	Pilih jumlah kapasitas storage yang diinginkan, di sini saya memilih 20GB karena tugasnya di perintahkan 20GB, selanjutnya pilih virtual disk into multiple agar kita dengan mudah melakukan split atau seting kapasitas storage, next













f.	Pilih customize kemudian ubah network connection menjdi bridge, agar kita bisa mendapatkan ip default dan mengubahnya menjadi ip static, dan menggunakan 1 CPU sesuai dengan tugas yang diberikan, klik finish













g.	Tunggu hingga proses selesai sampai menampilkan pilihan bahasa













h.	Pilih English kemudian tekan enter
















i.	Setelah itu skip 2 kali atau pilih done 2 kali sampai menampilkan konfigurasi network seperti ini, kemudian pilih ens33 & pilih ipv4, ubah itu menjadi manual













j.	Tampilanny menjadi seperti ini, isi kolom-kolom tersebut sesuai ip masing-masing, cek ip di cmd dengan ipconfig (untuk windows) atau ifconfig (untuk ubuntu desktop) Sesuaikan denga ip gateway masing-masing, bisa diliat di contoh gambar tersebut, untuk subnet isikan denga nip gateway namun tidak pada angka dalam titik terakhir & ubah menjadi .0/24 agar kalian bis seting address di angka terakhir sampai 255, di sini saya memilih .231 & ingat batasnya hanya 255












k.	Hasilnya akan seperti ini, kalian akan mendapat ip static sesuai yang kalian inginkan pada angka terkhir static 172.10.48.231/24













l.	Kemudian klik atau pilih done 2kali sampai tampilan seperti ini, kemudian set 2gb untuk swap dan sisa 18gb (ubah menjadi GPT) kemudian done & pilih continue
 

m.	Setelah itu kalian akan melihat tampilan seperti ini, isikan setiap kolom sesuai keinginan













n.	Selanjutnya install OpenSSH server kemudian pilih done















o.	Ini silahkan di next atau done saja












p.	Tunggu sampai selesai

















q.	Selesai, kemudian reboot & login sesuai yang telah diisikan













r.	Selanjutnya cek apakah terkoneksi baik keinternet dengan command <ping google.com> jika muncul seperti dibawah berarti semua telah selesai 












