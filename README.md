# 01-git-github
LAPORAN PERTEMUAN PERTAMA
PRAKTIK GIT DAN GITHUB

Pegertian Git dan GitHub 
Git adalah sebuah VCS (Version Control System)  sistem yang mengelola perubahan dari sebuah dokumen, program komputer, website dan kumpulan informasi lain. Sederhananya  Git dapat menyimpan rekaman perubahan pada source code sehingga kita dapat kembali ke keadaan sebelum perubahan
Github adalah sebuah website yang menyediakan layanan cloud untuk mengelola dokumen, projek/ repo 

Langakah langakah install git di Windows
1. pertama download Git di https://git-scm.com/downloads sesuaikan dengan versi bit laptop nya
2. Setelah download Git, klik dua kali file yang di download tadi dan file akan langsung install git. lalu munculkan lisensi. Klik Next untuk lanjut.
3. pilih lokasi instalasi. Secara default akan terisi C:\Program Files\Git. Ganti lokasi jika ingin lokasi lain,lalu klik Next
4. lalu terdapat berbagai komponen. Jika tidak yakin dengan pilihan komponen sebaiknya tidak perlu diubah biarkan default saja. klik Next
5. Akan terdapat pilihan Text Editor yang akan digunakan dengan git, Pilih sesuai Text editor yang biasa digunakan atau yang diinginkan
6. Git juga menyediakan akses untuk menggunkan git melalui Bash maupun Command Prompt, akan ada opsi dimana penggunaan Bash ataupun CMD  saat instalasi, disarankan Menggunakan Keduanya agar dapat dijalankan dengan Bash dan CMD
7. Pilih OpenSSL untuk HTTPS. Git menggunakan https untuk akes ke repo GitHub
8. Setelah itu akan muncul opsi Configuring ekstra option centang Enable file system caching untuk menambah performace boost, kemudian klik install 
9. Setelah install selesai klik finish (Untuk cek apakah Git sudah terinstall dengan masukkan command "git --version" di CMD kalau sudah muncul versi git berarti git sudah terinstall)
10. Untuk menjalankan GIt dapat melalui Icon di desktop atau dengan search GIT dan akan muncul git bash lalu jalankan 

Konfigurasi Git 

Pertama kita harus membuat akun di github terlebih dahulu berikut link github https://github.com/ setelah mempunyai akun github kita d harus memberitahu Git tentang username serta email yang digunakan agar setiap kali terjadi perubahan pada repo Git. Username serta email ini yang akan dimasukkan oleh Git ke catatan perubahan di repo. 

Untuk langkah langkah 
1. Jalankan Git Bash lalu ketik command seperti ini $ git config --global user.name "Nama USer sesuai akun di GitHub"
$ git config --global user.email "Nama Email yang digunakan"

2. untuk mengecek ketik comannd seperti ini $ git config --list . Lalu akan muncul nama user dan email yang di masukkan. Konfigurasi ini juga disimpan di $HOME/.gitconfig. Untuk sistem operasi Linux, dan untuk Sistem Operasi Windows disimpan di C:\Document and Settings\NamaUser dengan nama file .gitconfig

Penjelasan Repo Dan Cara membuat Repo

Seperti pengertian diatas GitHub adalah layanan Web yang menggunakan Kendali Git.Di GitHub terdapat salah satu fitur gratis disebut repository(disingkat dengan repo) repo adalah direktori atau folder untuk menyimpan berbagai file yang kita buat seperti Source Code, Dokumen, Foto ,dan Lain lain. Setelah membuat Repo, repo tersebut dapat diisi dengan membuat file baru maupun upload file kita sendiri ke repo . file yang berada di repo dapat di download atau clone, serta dengan fitur commit kita dapat menyimpan semua perubahan pada file tersebut. jika sudan mendownload file di Repo yang ada dari GitHub, kita bisa membuka nya melalui text editor yang kita pilih saat instalasi. Dengan demikian, untuk setiap file repo, kita dapat membuka di komputer lokal dan melakukan berbagai manipulasi di komputer lokal, setelah itu mengirimkan hasilnya ke repo GitHub. Proses ini disebut dengan proses push.     

Cara membuat repo

1. Pertama buka GitHub dan pastikan akun sudah terhubung lalu klik tombol plus di kanan lalu klik new Repository
2. Isi nama Repo dan Deskripsi san pilih jenis repo publik atau private setelah itu klik Create repository
3. Setelah itu kita dapat langsung membuat file dengan klik "Creating new file" untuk file baru dan "Upload" untuk mengupload file yang sudah ada , dan kita juga dapat membuat file menggunkan command line di bawah ini
    echo "# Coba" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M main
    git remote add origin https://github.com/FarhanWidyanaM/Coba.git
    git push -u origin main
4. Untuk membuat file dengan command line kita harus membuat folder di Komputer lokal lalu masuk ke folder dan klik kanan, lalu klik Git bash Here setelah itu masukkan command line satu persatu 
5. Setelah itu mucul file README.md dan lakukan First Commit dengan  git commit -m "first commit"
6. Lalu lakukan Remote Repository dengan  git remote add origin https://github.com/FarhanWidyanaM/Coba.git
7. Terakhir lakukan push ke github dengan git push -u origin main

