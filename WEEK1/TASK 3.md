APPLICATION IN SERVER

A. Perbandingan antara monolith & Microservices

Monolith itu sebuah basis database system yang tersusun & terhubung secara vertikal dalam satu garis yang sama dimana jika salah satu fitur aplikasi tidak dapat diakses maka semua fitur demikian, berbeda dengan microservices, memiliki beberapa database yang sama dan menggunakan banyak server untuk setiap fitur aplikasi, jika salah satu fitur/databse down, mereka secara tidak langsung mengalihkan ke database/ server lainnya yang masih berfungsi.

B. Deploy Aplikasi wayshub-frontend (NodeJS)

Inputkan setiap urutan command yang seperti digambar

![Screenshot (88)](https://user-images.githubusercontent.com/117638290/202864435-a8a43d3a-47f8-4e65-8b8f-55246928f4c3.png)

Penjelasan setiap command:
1. curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash (command tersebut untuk install tool yang berfungsi mengunduh dan menginstal Node.js (nvm) )
2. exec bash (untuk reset aplikasi)
3. nvm install 16 (untuk menginstall nvm versi 16)
4. git clone https://github.com/dumbwaysdev/wayshub-frontend (untuk melakukan cloning terhadap salah satu aplikasi yang berada di git)
5. ls (untuk cek apakah sudah ada dirrektori wayshub-frontend)
6. cd wayshub-frontend (untuk masuk ke direktorinya jika sudah ada)
7. npm install (untuk menginstall packge managernya)
8. npm run start (untuk menjalankan aplikasinya)
9. selesai hasilnya akan menjadi seperti ini

![Screenshot (91)](https://user-images.githubusercontent.com/117638290/202864853-7add80ea-6dc6-42dd-a67e-6b1d74ef262c.png)

C. Deploy Golang dengan menampilkan nama masing-masing

1. Install package dari golang itu sendiri dengan command sudo apt install golang-go

![Screenshot (95)](https://user-images.githubusercontent.com/117638290/202865122-d6598b01-fe40-4722-918e-91718f84b4bf.png)

2. Install file tambahan dari golang tersebut dengan command wget https://golang.org/dl/go1.16.5.linux-amd64.tar.gz

![Screenshot (122)](https://user-images.githubusercontent.com/117638290/202865320-d4c30c7c-7bf1-4eb4-8d7f-7044491977cd.png)

3. Ekstrak file yang tadi kita unduh dengan command sudo tar -C /usr/local -xzf go1.16.5.linux-amd64.tar.gz
4. Cari file bash.rc untuk kita edit inputkan command find ~  -maxdepth 1  -name '.bashrc'
5. Setelah menemukannya ketikkan command  nano /home/yasin/.bashrc (inputkan sesuai nama direktori masing-masing)
6. Kemudian inputkan di baris paling bawah seperti gambar di bawah dengan command export PATH=$PATH:/usr/local/go/bin

![Screenshot (96)](https://user-images.githubusercontent.com/117638290/202865630-aa98cf9f-fa7e-430d-9e5a-6358ba99abd8.png)

7. silahkan keluar dari editor dengan menekan ctrl X kemudian Y kemudian enter
8. Buat aplikasi sederhana dengan nama kalian, dengan command nano app.go
9. nanti akan muncul seperti ini kemudian tekan ctrl X kemudian Y kemudian enter untuk save & exit

![Screenshot (97)](https://user-images.githubusercontent.com/117638290/202865768-6a9fd1a8-2ff0-4edb-8d34-8666b5b3f5cb.png)

10. Jalankan aplikasi tersebut, jika berhasil maka akan muncul nama kalian, jalankan dengan commad go run app.go

![Screenshot (123)](https://user-images.githubusercontent.com/117638290/202865969-5e379c05-45b3-4445-9bf0-4f1ff6a55dd5.png)


D. Deploy Python dengan menampilkan nama masing-masing

1. Buatlah direktori baru akan file tidak berantakan, dengan command mkdir my-app-python
2. Selanjutnya masuk ke direktori tersebut dengan command cd my-app-python
3. Install aplikasinya dengan command sudo apt install python3
4. kemudian cek versi dengan command python3 --version
5. selanjutnya kita unduh package manager dari python itu sendiri seperti halnya npm, inputkan dengan command sudo apt install python3 pip
Ikuti seperti gambar di bawah ini

![Screenshot from 2022-11-19 21-11-25](https://user-images.githubusercontent.com/117638290/202938550-4e06bb78-6308-4a43-9cb2-dc3e8b75dc4b.png)

6. kemudian inputkan untuk frameworknya dengan command pip install flask

![Screenshot from 2022-11-19 21-11-54](https://user-images.githubusercontent.com/117638290/202938917-569bc27f-bd43-4f68-8d1d-7d817590c8ca.png)

7. selanjutnya kita buat file pythonnya, saya memberi nama filenya pyton & isikan sesuai gambar di bawah ini untuk menampilkan nama kita, jadi saya inputkan command nano pyton.py

![Screenshot from 2022-11-19 21-21-32](https://user-images.githubusercontent.com/117638290/202939245-40022e2c-1476-4cf7-9982-35001081ad36.png)

8. Terakhir jalankan apilikasi tersebut dengan command pyhton3 pyton.py. lalu buka browser dengan link localhost:5000 karena python bekerja pada port tersebut

![Screenshot from 2022-11-19 21-14-55](https://user-images.githubusercontent.com/117638290/202939671-d383d7bf-01bd-4620-bbfd-976eb00b5254.png)


E. Menjalankan localtunnel untuk aplikasi wayshub-frontend 

1. karena kita sebelumnya telah melakukan instalasi pada aplikasi tersebut, jadi sekarang kita hanya menjalankannya dengan command lt --port 3000 --subdomain
2. setelah mendapatkan urlnya copy & pastekan dibrowser kalian, lakukan seperti gambar dibawah ini

![Screenshot (106)](https://user-images.githubusercontent.com/117638290/202942663-c6b6b174-78fa-418b-bcd6-c7a1d36d8df3.png)


F. Menjalankan semua aplikasi dengan PM2

1. karena kita telah melakukan instalasi pada ketiga aplikasi tersebut, kita tinggal menginstall pm2 lalu menjalankan masing-masing aplikasinya
2. Install PM2 terlebih dahulu dengan command npm install -g pm2
3. setelah itu jalankan aplikasi masing-masing
untuk npm nodejs dengan command pm2 start npm -- start
untuk golang dengan command pm2 start app.go
untuk python dengan command pm2 start pyton.py
4. hasilnya akan seprti gambar dibawah ini

![Screenshot (110)](https://user-images.githubusercontent.com/117638290/202943534-e473f5a8-6df6-4b53-9a59-778ee9e470f7.png)








