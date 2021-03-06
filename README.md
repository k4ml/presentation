# Tutorial github 

pertama sekali apa yang anda perlukan adalah sebuah akaun github dan [git for windows](https://msysgit.github.io/),jika sekiranya anda menggunakan windows.

kemudian anda digalakkan untuk mengikuti tutorial di 
[youtube](https://www.youtube.com/watch?v=_tN0T7jYn0A) untuk proses configuration.sekiranya anda mengikuti video tutorial tersebut,anda tidak perlulah berulangkali memasukkan password anda.

sekarang saya mengandaikan anda telah mempunyai akaun github dan telah mengikuti video tutorial di link yang telah saya berikan.


##1) Hasilkan Repository baru dan folder projek

untuk menghasilkan repository baru di github amatlah mudah..

anda hanya perlu klik pada butang tambah dan pilih new repository untuk hasilkan repo baru..Namakan repository anda , kemudian klik butang hijau "create repository"


![new repo](https://github.com/farouqzakwan/presentation/blob/master/screenshot/new%20repo.PNG) 


![ create new repo](https://github.com/farouqzakwan/presentation/blob/master/screenshot/create%20new%20repo.PNG) 

dalam gambar di atas, saya namakan repository saya yourRepoName.Memandangkan saya telah sedia ada mempunyai sebuah repository yang kosong, saya akan menggunakan repository "presentation" untuk tutorial ini.

kemudian hasilkan sebuah folder yang anda akan gunakan untuk projek anda..


saya telah menghasilkan sebuah folder baru di desktop saya dan saya namakanya "tutorial" dan di dalam folder tersebut saya hasilkan sebuah lagi folder "screenshot". folder screenshot adalah bertujuan untuk menyimpan semua gambar yang diperlukan dalam tutorial ini.


##2) jalankan perisian Git Bash

Sekarang jalankan perisian Git Bash anda dan tukar directory ke directory folder projek anda.Cara yang saya gunakan ialah, saya membuka folder "tutorial" kemudian klik butang kanan tetikus dan saya pilih "git bash here".

Bagi saya cara begini lebih menyenangkan kerana saya tidak perlu untuk menaip directory yang panjang..

##3) hasilkan file / code

Di dalam folder tutorial saya akan hasilkan sebuah file "farouq.txt" dan isi kandungannya adalah

```
hai saya farouq
```
![farouq txt](https://github.com/farouqzakwan/presentation/blob/master/screenshot/create%20farouq%20txt.PNG)


tujuan saya hasilkan sebuah file text dan mempunyai kandungan yang amat ringkas adalah supaya memudahkan anda membuat perbandingan setelah kandungan file ini di ubah.

##4) git init

Di dalam perisian git bash anda, taip 

```
$ git init
```

Arahan ini bermaksud anda sedia menjadikan directory dan subdirectories yang anda berada sekarang sebagai sebuah repository.

![git init](https://github.com/farouqzakwan/presentation/blob/master/screenshot/git%20init.PNG)

##5) git add

Arahan seterusnya adalah 

```
$ git add .
```

atau 

```
$ git add farouq.txt
```

git add merupakan arahan untuk anda meletakkan file dan code anda dalam keadaan staging atau dalam erti kata lain bersedia sebelum anda commit code anda.


perbezaan kedua-dua arahan di atas ialah, arahan pertama meletakkan semua file yang belum anda jejaki/rekod(file baru) atau file yang telah di ubah dalam keadaan sedia untuk di commit manakala arahan kedua lebih bersifat memilih file-file tertentu sahaja.

![git add](https://github.com/farouqzakwan/presentation/blob/master/screenshot/git%20add%201.PNG)

dalam gambar di atas,terdapat dua baris perkataan yang berwarna merah..ini bermaksud terdapat dua file yang belum git jejak/rekod.

##6) git status

```
$ git status
```

Arahan git status di gunakan untuk memeriksa status-status file anda.

setelah anda menaip arahan ini,anda akan dipaparkan status-status file anda samada terdapat file yang diubah (berwarna merah),sedia untuk di commit(berwarna hijau),konflik (berwarna merah),file yang telah di buang(berwarna merah),atau directory yang bersih.

##7) git commit

```
$ git commit -m "ruang tulis komen"
```

![git commit](https://github.com/farouqzakwan/presentation/blob/master/screenshot/git%20commit%201.PNG)

Arahan in digunakan setelah anda meletakkan file dan code anda dalam keadaan sedia dan anda berpuas hati dengan hasil kerja anda.Disinilah point-point atau titik rujukan yang akan disimpan oleh git.github membenarkan anda kembali kepada titik-titik rujukan ini sekiranya code anda selepas ini bermasalah atau anda membangunkan dua atau tiga versi yang berbeza. 

##8) git log

arahan
```
$ git log
```

![log commit](https://github.com/farouqzakwan/presentation/blob/master/screenshot/git%20log%201.PNG)

akan memaparkan log-log commit dan message anda.


##9) file yang diubah

seterusnya saya akan mengubah kandungan "farouq.txt" dan menambah beberapa image kedalam folder screenshot

kandungan baru dalam farouq.txt ialah

```
nama : farouq zakwan
umur : 23 (2015)
```

![ubah kandungan](https://github.com/farouqzakwan/presentation/blob/master/screenshot/change%20farouq%20txt.PNG)

setelah melakukan perubahan apa yang perlu di buat ialah mengulangi arahan git add dan git commit..

![add image](https://github.com/farouqzakwan/presentation/blob/master/screenshot/git%20add%203.PNG)

![commit file](https://github.com/farouqzakwan/presentation/blob/master/screenshot/git%20commit%202.PNG)

##10) push to github

jika anda masih ingat lagi,di awal tutorial ini saya telah mengajar bagaimana untuk menghasilkan sebuah repository baharu di github dan saya menyatakan yang saya akan  menggunakan repository "presentation" untuk tutorial ini.sehingga sekarang saya masih lagi belum menulis bagaimana untuk menggunakan nya.

terdapat arahan yang perlu anda taip sebelum anda boleh push code anda ke repository github.

```
$ git remote add origin https://github.com/farouqzakwan/presentation.git
```

setiap kali anda ingin push code anda ke repository ini,anda perlu menaip

```
$ git push -u origin master
```

##11) lain-lain

sehingga saat tutorial ini,banyak lagi perkara yang belum di bincangkan tentang cara penggunaan github..
antara perkara tersebut adalah bagaimana menggunakan github untuk kerjasama kumpulan,menulis README.md dalam format markdown.report an issue.kembali ke snapshot commit yang lepas.

oleh itu saya amat mengharapkan anda dapat menambah baik tutorial ini dari semasa ke semasa.