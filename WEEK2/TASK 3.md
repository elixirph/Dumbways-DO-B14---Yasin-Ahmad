Web Server & Load Balancing

A. Definisi Web Server ? 

Web Server adalah sebuah layanan untuk mengakses http/https kemudian web server akan mengirimkan permintaan dalam bentuk halaman & bekerja secara bolak balik dari request data & dikembalikan ke client dalam bentuk halaman


B. Menjalankan 2VM 

1. Menggunakan vmware untuk appserver dumbflix

![Screenshot (207)](https://user-images.githubusercontent.com/117638290/203821147-2eac9f26-bfcd-459a-a2e2-4c495b1bd644.png)

2. Menggunakan multipass untuk Nginx

![Screenshot (178)](https://user-images.githubusercontent.com/117638290/203821506-9e535e19-cea1-4fc1-ba14-275d2f6a290c.png)


C. Menggunakan VM1 untuk dumbflix-frontend dengan pm2

![Screenshot (172)](https://user-images.githubusercontent.com/117638290/203821786-de0640dc-3219-4292-8a63-1d1f3f32d566.png)
![Screenshot (174)](https://user-images.githubusercontent.com/117638290/203821807-48decb20-47c2-46de-8294-0363ad8963c1.png)


D. Menjalankan Nginx dengan VM2

![Screenshot (183)](https://user-images.githubusercontent.com/117638290/203821970-b60d92bc-cc99-4f75-99e2-e50350adff27.png)

E. Membuat konfigurasi reverse proxy dengan domain (gunakan nama kalian) mengarah ke app di VM1

![Screenshot (211)](https://user-images.githubusercontent.com/117638290/203850574-a4b3524c-ff39-48c6-8c43-a13495bc9352.png)
![Screenshot (212)](https://user-images.githubusercontent.com/117638290/203850587-2a66ee6d-841f-4f47-b59f-0654230fd753.png)
![Screenshot (213)](https://user-images.githubusercontent.com/117638290/203850604-e7f08f61-86f1-406e-96c1-d2d9cf9af013.png)

F. buat konfigurasi load balance antara VM1 dan VM2
![Screenshot (216)](https://user-images.githubusercontent.com/117638290/203850784-b4645209-5ab9-40cb-b1fe-95d89a67ee87.png)
![Screenshot (217)](https://user-images.githubusercontent.com/117638290/203850792-531d1fdf-a2e7-4a8b-9d4d-2db7a86e6555.png)

G. Domain bisa diakses melalui web browser kalian
![Screenshot (219)](https://user-images.githubusercontent.com/117638290/203850804-d0233452-8b21-49b1-8697-bb6b1b139200.png)
![Screenshot (220)](https://user-images.githubusercontent.com/117638290/203850809-209b8330-b44c-4a3e-8733-2b282cf02833.png)
![Screenshot (221)](https://user-images.githubusercontent.com/117638290/203850835-965e6785-cbfa-4959-8045-d5e223decd1a.png)

Load Balancing telah berjalan dengan semepurna

