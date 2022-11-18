TASK (DevOps Introduction & Installing Ubuntu via Vmware)

1. Definisi DevOps

Devops merupakan development & operation, jadi menurut saya devops ini sebuah ruangan untuk bertukar informasi antara keduanya, dan dengan ruangan ini kerja dari masing-masing tim dapat berjalan baik karena adanya sebuah jalan pintas/ automasi dimana saat keduanya bekerja & ada masalah tidak mengganggu pekerjaan tim yang lain & aplikasi bisa tetap berjalan sebagaiman mestinya. 

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.001.png)







1. Sebutkan 2 lifecycle DevOps & jelaskan definisinya

![DevOps Methodology, Lifecycle and Best Practices explained](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.002.jpeg)









1. Planning, Pada tahap pertama, tim melakukan analisis kebutuhan proyek berdasarkan masukan dari pelanggan, departemen penjualan, hasil survei pemasaran, dan pandangan expert di industri tersebut. Data dan informasi yang terkumpul digunakan dalam perencanaan dan studi proyek dalam aspek ekonomi, operasional, dan teknikal.

1. Deployment, produk selesai melalui proses deployment dan kemudian dirilis untuk segmen yang terbatas. produk mendapatkan berbagai umpan balik saat testing. Umpan balik tersebut digunakan untuk pengembangan software. Selanjutnya, produk dapat dirilis ke pasar dan melakukan aktivitas pemeliharaan produk secara berkala.

1. Install Ubuntu Server (1 CPU, 2GB RAM & 20GB Storage (2GB untuk swap), setup ip static, install OpenSSH Server
   1. Pertama pilih Create a New File

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.003.png)











1. Kedua browse file iso ubuntu server 20.04 yang telah di download, jika belum download silahkan download di web resmi ubuntu.com

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.004.png)












1. Ketiga, isi semua kolom sesuai keinginan kita dan klik next

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.005.png)











1. Selanjutnya, masukan nama virtual machine dan pilih lokasi atau target penyimpanan filenya, jika sudah ada secara default langsung saja

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.006.png)
















1. Pilih jumlah kapasitas storage yang diinginkan, di sini saya memilih 20GB karena tugasnya di perintahkan 20GB, selanjutnya pilih virtual disk into multiple agar kita dengan mudah melakukan split atau seting kapasitas storage, next

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.007.png)











1. Pilih customize kemudian ubah network connection menjdi bridge, agar kita bisa mendapatkan ip default dan mengubahnya menjadi ip static, dan menggunakan 1 CPU sesuai dengan tugas yang diberikan, klik finish

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.008.png)












1. Tunggu hingga proses selesai sampai menampilkan pilihan bahasa

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.009.png)












1. Pilih English kemudian tekan enter

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.010.png)















1. Setelah itu skip 2 kali atau pilih done 2 kali sampai menampilkan konfigurasi network seperti ini, kemudian pilih ens33 & pilih ipv4, ubah itu menjadi manual

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.011.png)












1. Tampilanny menjadi seperti ini, isi kolom-kolom tersebut sesuai ip masing-masing, cek ip di cmd dengan ipconfig (untuk windows) atau ifconfig (untuk ubuntu desktop) Sesuaikan denga ip gateway masing-masing, bisa diliat di contoh gambar tersebut, untuk subnet isikan denga nip gateway namun tidak pada angka dalam titik terakhir & ubah menjadi .0/24 agar kalian bis seting address di angka terakhir sampai 255, di sini saya memilih .231 & ingat batasnya hanya 255

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.012.png)











1. Hasilnya akan seperti ini, kalian akan mendapat ip static sesuai yang kalian inginkan pada angka terkhir static 172.10.48.231/24

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.013.png)












1. Kemudian klik atau pilih done 2kali sampai tampilan seperti ini, kemudian set 2gb untuk swap dan sisa 18gb (ubah menjadi GPT) kemudian done & pilih continue

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.014.png)

1. Setelah itu kalian akan melihat tampilan seperti ini, isikan setiap kolom sesuai keinginan

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.015.png)












1. Selanjutnya install OpenSSH server kemudian pilih done

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.016.png)














1. Ini silahkan di next atau done saja

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.017.png)











1. Tunggu sampai selesai

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.018.png)
















1. Selesai, kemudian reboot & login sesuai yang telah diisikan

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.019.png)












1. Selanjutnya cek apakah terkoneksi baik keinternet dengan command <ping google.com> jika muncul seperti dibawah berarti semua telah selesai 

![](Aspose.Words.a2bb6c57-0473-4589-8c6f-98335ec8523f.020.png)











