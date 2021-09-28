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

