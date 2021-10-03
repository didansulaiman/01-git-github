## Langkah langkah praktik git hub
1. Download git di https://git-scm.com/downloads 
2. instal git
3. buat akun github 
4. konfigurasi git 
    ```
    $ git config --global user.name "Nama Anda di GitHub"
    $ git config --global user.email email@domain.tld
    ```
    disesuaikan dengan nama serta email yang di gunakan untuk mendaftar github. dan untuk melihat konfigurasi yang sudah ada
    ```
    $ git config --list
    user.email=phylossophie@gmail.com
    user.name=Bambang Purnomosidi D. P.
    color.ui=true
    $
    ```
5. membuat repositori di github
6. clone repositori tersebut di komputer lokal 
    ```
    $ git clone https://github.com/oldstager/awesome-project
    ```
7. buat file .md di text editor yang kalian gunakan
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

