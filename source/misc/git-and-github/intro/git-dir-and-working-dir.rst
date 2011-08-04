Git Direktory Dan Working Direktory
===================================

Satu hal yang penting dalam belajar git adalah kita harus bisa membedakan antara Git Direktory dan Working Direktory.

Git Direktory
-------------

Secara mudah git direktori adalah letak direktori .git yang didalamnya terdapat konfigurasi berserta meta informasi yang disediakan git. Jika dilihat informasinya akan tampak seperti berikut .

::

	$ tree .git/ -L 1
	.git/
	|-- branches
	|-- config
	|-- description
	|-- HEAD
	|-- hooks
	|-- info
	|-- objects
	`-- refs

	5 directories, 3 files
	$
	
File dan meta informasi tersebut secara otomatis akan dibuat oleh git pada saat pertama kita inisialisasi. Untuk lebih detil cara inisialisasi reporitory git , akan dibahan pada bab selanjutnya. 

Working Direktory
-----------------

Sedangkan working direktori mengacu pada letak branch aktif pada saat kita berkerja dengan git. Secara standar kita memiliki branch master pada pertama kali commit.
::

	$ git branch -a
	* master
	$

Atau jika kita bekerja dengan remote server kita bisa lebih dari satu branch .
::

	$ git branch -a
	* master
	  remotes/origin/HEAD -> origin/master
	  remotes/origin/master
	  remotes/upstream/master
	$

Pengertian branch akan kita bahas pada bab berikutnya.
