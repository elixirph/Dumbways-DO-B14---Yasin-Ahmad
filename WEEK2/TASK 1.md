A. Definisi CI/CD 

B. Fork repository Dumbflix
1. Sebagai langkah awal kita masuk ke dalam link github dari repository yang akan kita fork disini saya menggunakan https://github.com/dumbwaysdev/dumbflix-frontend , kemudian klik fork pada bagian kanan atas

![1](https://user-images.githubusercontent.com/117638290/203056979-bf601ae4-3896-40dc-b66c-97802653adf3.jpg)

2. Selanjutnya isikan repository name dengan nama apa saja, asal bisa & langsung saja create new fork

![2](https://user-images.githubusercontent.com/117638290/203057104-f8312a62-adf4-4fc7-a228-23ab374bbce8.png)

3. Cek apakah sudah tersalin kedalam repository kita atau belum, jika sudah maka akan seperti ini

![3](https://user-images.githubusercontent.com/117638290/203057132-4dd0c972-a541-4a69-aa5d-9fd9c917b127.jpg)


C. Deploy aplikasi melalui cloudflare pages

1. Buat akun cloudflare terlebih dahulu, jika sudah silahkan masuk ke dalam menu pages di sebelah kiri & koneksikan ke akun git 

![4](https://user-images.githubusercontent.com/117638290/203057200-cb640f46-457a-45cb-9259-194b692b4f9d.jpg)

2. Kemudian pilih repository yang ingin kita deploy, di sini saya memilih repository yang telah saya fork sebelumnya lalu klik Begin Setup

![5](https://user-images.githubusercontent.com/117638290/203057238-177e1755-0c44-4342-91a3-7242a1f6dbbc.jpg)

3. Isikan kolom project name dengan nama bebas & itu akan menjadi keyword link dari web tersebut lalu isikan Framework preset dengan React App untuk membuildnya, karena repo tersebut menggunakan basecode react

![6](https://user-images.githubusercontent.com/117638290/203057259-f2218d3a-321a-45d5-96fb-ea85ed94247c.jpg)

4. Save & Deploy lalu tunggu hingga proses selesai!

![7](https://user-images.githubusercontent.com/117638290/203057284-44adba7c-8528-4aa3-8f16-dfbef481c4eb.png)

5. Kemudian klik Continue to project & klik site tersebut maka hasilnya akan seperti ini

![8](https://user-images.githubusercontent.com/117638290/203057326-93dc2f3f-eaa6-4cba-919e-465f28e65367.png)

![9](https://user-images.githubusercontent.com/117638290/203057514-bab15b9d-a981-407f-996c-932521a68ac6.png)

6. Jika kita ingin mengubah tulisan yang tertera pada tab tittle ubah melalui repo yang ada pada git kita dengan memilih folder public > index.html & open file tersebut lalu ganti dengan nama yang diinginkan
lebih jelasnya silahkan lihat pada gambar dibawah ini

![10](https://user-images.githubusercontent.com/117638290/203057858-8b08f92f-c819-4ee8-b3d6-e2e5d0c8079c.jpg)

7. Kemudian klik commit changes untuk menyimpan perubahan & silahkan buka kembali cloudflarenya karena disana akan ada respon dari perubahan tersebut

![11](https://user-images.githubusercontent.com/117638290/203057952-c1207ea5-423c-4304-89f4-a8478aa947ea.jpg)

8. Terakhir klik visit site untuk melihat perubahannya

![12](https://user-images.githubusercontent.com/117638290/203057977-18c19740-2d12-4e8e-9362-096c6824e107.jpg)

![13](https://user-images.githubusercontent.com/117638290/203058007-937f523e-70b9-4fa9-aa64-a986d8184cc1.jpg)

D. Deploy 2 branch yang berbeda



