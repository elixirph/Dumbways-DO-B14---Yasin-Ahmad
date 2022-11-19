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
5. 











