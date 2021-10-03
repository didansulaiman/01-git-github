# Langkah langkah praktik git hub

## Instalasi git
1. Download git di https://git-scm.com/downloads 
2. instal git
3. buat akun github 
## Konfigurasi git
4. konfigurasi git 
    ```
    $ git config --global user.name "Nama Anda di GitHub"
    $ git config --global user.email email@domain.tld
    ```
    disesuaikan dengan nama serta email yang di gunakan untuk mendaftar github. dan untuk melihat konfigurasi yang sudah ada
    ```
    $ git config --list
    user.email=didansulaiman1234@gmail.com
    user.name=didansulaiman
    color.ui=true
    $
    ```
## Mengelola repositori sendiri
5. membuat repositori di github
6. clone repositori tersebut di komputer lokal 
    ```
    $ git clone https://github.com/didansulaiman/01-git-github.git
    ```
7. buat file .md di folder yang sudah di clone dengan text editor yang kalian gunakan
### Mengubah Isi - Push Tanpa Branching dan Merging
8. setelah selesai, setelah itu untuk mengetahui status dari repository lokal :
    ```
    $ git status
    ```
9. untuk membuat repository pada file lokal yang nantinya ada folder .git
    ```
    $ git init
    ```
10. untuk menambahkan file baru pada repository yang dipilih:
    ```
    $ git add namafile.md
    ```

11. untuk menyimpan perubahan yang dilakukan, tetapi tidak ada perubahan pada remote repository :
    ```
    $ git commit -m
    ```
12. untuk mengirimkan perubahan file setelah di commit ke remote repository :
    ```
    $ git push -u origin main
    ```
### Mengubah Isi dengan Branching and Merging

Dengan menggunakan cara ini, setiap kali akan melakukan perubaham, perubahan itu dilakukan di komputer lokal dengan membuat suatu cabang yang nantinya digunakan untuk menampung perubahan-perubahan tersebut. Setelah itu, cabang itu yang akan dikirim ke repo GitHub untuk dimintai review kemudian digabungkan (merge) ke main. Secara umum, repo yang dibuat biasanya sudah mempunyai satu branch yang disebut dengan main. Cara ini lebih aman, terstruktur, terkendali, dan mempunyai history yang lebih baik. Jika perubahan yang kita buat sudah terlalu kacau dan kita menyesal, maka ada cara untuk "membersihkan" repo lokal kita.

13. untuk melihat cabang gunakan perintah
    ```
    git branch
    ```
    jika belum ada akan memunculkan master/main saja
14. untuk membuat cabang baru 
    ```
    git branch "nama branch"
    ```
15. untuk pindah ke cabang baru adalah
    ```
    git checkout "nama branch"
    ```
16. kita bisa menambahkan file atau sekedar argumen
    ```
    $ git add -A
    $ git commit -m "Add: isi README.md"
    ```
17. untuk menggabungkan cabang dan main gunakan perintah
    ```
    git checkout master
    ```
18. untuk berpindah ke main/master dahulu beikutnya untuk menggabungkan perintahnya 
    ```
    git merge "nama branch"
    ```
### sinkronasi
Suatu saat, bisa saja terjadi kita menggunakan komputer lain dan mengedit repo melalui repo lokal di komputer lain, setelah itu pindah ke kamputer lain lagi. Saat itu, kita perlu melakukan sinkronisasi ke kemputer lokal. Perintah untuk sinkronisasi adalah:
```
git pull
```