VERSION CONTROL SYSTEM

A. Definisi git, git itu sebuah web/aplikasi tempat menyimpan kode bagi para development ataupun yang sedang melakukan coding & dimana semua developer dapat berbagi kode ke masyarakat umum, dan mereka dapat melakukan editing/ perbaikan, jadi saya menyebutnya ini sebuah perpustakan code digital yang sangat besar & terbuka bagi umum.

B. Merubah IP address di PC (tes menggunakan command ssh)

1. Langkah awal kita akan merubah isi file setingan networknya terlebih dahulu dengan command sudo nano /etc/netplan/50-cloud-init.yaml
2. selanjutnya rubah ip addresses sesuai yang diinginkan, ingat!!! setiap kolom isikan dengan ip gateway yang sesuai dengan koneksi internet kalian saat ini, jadi kita hanya bisa merubah angka setelah titik terakhir & untuk subnet isikan dengan 0/24 agar kita bisa memilih sampai angka maksimal 255, lihat seprti gambar dibawah ini

![image](https://user-images.githubusercontent.com/117638290/202944109-4e950504-8125-4650-bbc6-ca15cd8aebec.png)

3. selanjutnya kita akan apply setingan tersebut dengan command sudo netplan apply kemudian inputkan command ssh username@ip .inputkan sesuai username & ip masing-masing. setelah itu kita test menggunakan command ping google.com hasilnya seperti gambar dibawah ini

![image](https://user-images.githubusercontent.com/117638290/202944361-8782297a-3baf-44d5-b1df-6c99fa2cbada.png)


C. Menghubungkan git ke server masing-masing
1. Pertama buat repositori baru seprti gambar di bawah ini

![Screenshot (111)](https://user-images.githubusercontent.com/117638290/202944589-e90f69ba-bc5b-4f2e-8e19-a1e64d3e7df4.png)

2. kemudian buat kunci dengan command ssh-keygen enter sampai selesai.
3. selanjutnya kita copykan isi key dari file yang berada dalam file dengan command cat id_rsa.pub
4. kita copy key tersebut kemudian pastekan di dalam pengaturan akun git pada tab SSH & GPS KEY kemudian tambahkan ssh key
5. selanjutnya kita configurasi akun kita dengan command git config --global user.name "Yasin Ahmad"
6. kemudian set email kita yang berada di git dengan command git config --global user.email "yasinahmad999@gmail.com"
7. langkah terkhir dengan cek apakah terhubung atau tidak dengan command ssh -T git@github.com
liat gambar di bawah ini untuk urutannya

![Screenshot (113)](https://user-images.githubusercontent.com/117638290/202952649-c23d6fb9-bc5b-4d18-a0d8-5cadd86b271e.png)
![Screenshot (116)](https://user-images.githubusercontent.com/117638290/202952677-45eca3d9-1039-400d-aba0-2de0e8b4c8d6.png)
![Screenshot (114)](https://user-images.githubusercontent.com/117638290/202952791-9693bd91-cc19-40cf-9bc0-a063354febc1.png)
![Screenshot (115)](https://user-images.githubusercontent.com/117638290/202952827-b28ee99c-957d-4628-aebd-f2a597b8a173.png)

8. selanjutnya membuat proyek baru dengan push ke git dengan command git init tas-newbie
9. kemudian menambahkan teks dengan command echo "coba aja" > test.txt
10. kemudian command ls untuk melihat isi folder tersebut
11. jika sudah lakuka command git add test.txt
12. cek dengan command git status
13. setelah itu masukkan ke repositori dengan command git commit -m "upload test.txt"
14. lalu koneksikan secara ssh dengan command git remote add origin git@github.com:elixirph/TEST_CLONE.git
15. selanjutnya cek dengan command git remote -v
16. selanjutnya kita push dengan command git push --set-upstream origin master
17. file telah terupload
untuk lebih jelasnya silahkan liat gambar berikut ini

![Screenshot (118)](https://user-images.githubusercontent.com/117638290/202955244-ccd660d1-33d9-48b0-8792-3076abf6855b.png)

![Screenshot (120)](https://user-images.githubusercontent.com/117638290/202955277-1eb0184e-30a6-43c6-92e1-f11b63d04fdc.png)


D. Membuat 3 buah branch
1. cukup membuat nama branch baru dengan contoh command 
git branch development
git branch stagging
git branch production

2. untuk melihat yang telah dibuat cukup dengan command git branch
3. untuk lebih jelasnya silahkan liat gambar di bawah ini

![Screenshot (121)](https://user-images.githubusercontent.com/117638290/202956788-511ac32e-c1b0-4dbe-9187-942da224909c.png)

E. 3 command git lainnya

git diff (menampilkan semua konflik yang ada)

git log (melihat track pada daftar commit yang ada)

git show (untuk menampilkan informasi pada objek git)

![Screenshot (126)](https://user-images.githubusercontent.com/117638290/202959758-a58a9f3f-b1b3-4115-9afd-052b4a6f5fd6.png)

