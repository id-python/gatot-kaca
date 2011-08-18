
Membaca Log
===========

Dari hasil commit yang kita lakukan sebelumnya , kita selalu memberikan opsi -m pada saat commit . Itulah sangat penting , karena dari situ kisa bisa membaca perubahan apa saja yang terjadi dari awal coding sampai selesainya sebuah project . 

Untuk membaca log sangat mudah sekali , kita bisa menggunakan perintah git log .
::

	$ git log 
	commit 99f5b9a4a7b9cf2835a7ea35073cee81a6fdb529
	Author: Fanani M. Ihsan <contact@fanani.net>
	Date:   Thu Aug 18 10:11:16 2011 +0700

	    first commit

Itu adalah cara standar untuk melihat log . Kita juga bisa membaca log agar tampilannya singkat seperti berikut.
::

	$ git log --pretty=oneline 
	99f5b9a4a7b9cf2835a7ea35073cee81a6fdb529 first commit

Itulah sekilas cara melihat log.
