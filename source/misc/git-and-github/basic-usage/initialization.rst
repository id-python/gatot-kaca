
Memulai Project dengan Git
==========================

Untuk memulai sebuah project dengan git , pertama  kali kita harus membuat sebuah direktori dengan nama yang sama dengan nama project . Sebagai contoh kita akan membuar project dengan nama hello-git .
::

	$ mkdir hello-git

Seteleh hello git sudah dibuat , selanjutnya kita tinggal mengisialisasi git pada direktori .
::

	$ cd hello-git
	$ git init

Setelah kita mengetikan git ini maka git akan membuat sebuah direktori git  didalam hello-git .
::

	$ ls -a
	  .git

Sampai disini kita sudah memiliki sebuah repository kosong atau sama sekali tidak terdapat file. Untuk itu coba sekarang buat sebuah file dengan nama README .
::
	$ touch README

::

	// Isi file redme
	Selamat membaca

file README yang baru kita buat masih didalam working direktori, lalu tujuan kita adalah menaruh file tersebut kedalam repository hello-git yang baru saja kita buat tadi. Namun sebelum itu kita harus menaruh file tesebut pada staging area (jika belum tahu staging area , coba baca lagi Alur kerja dengan GIT) dengan menggunakan git add .
::

	$ git add README

dengan menggunakan file tersebut kita hanya menambahkan file README ke stagging area, kita juga bisa menambahkan secara rekursif . 
::

	$ git add .

Langkah terahir adalah kita akan mencomit hasil perubahan kedalam repository git .
::

	$ git commit -m "first commit"

-m adalah opsi utuk memberikan pesan , sehingga kelak di kemudian hari kita bisa membaca perubahan apa saja yang terjadi.
