
Konfigurasi dan Inisialisasi
============================

Sebelum menggunakan git , sebaiknya kamu mengonfigurasi dasar git seperti nama dan email kamu . Untuk itu silakan buka terminal linux kesayanga kamu, jika kamu menggunakan windows gunakan git shell .
::

	$ git config --global user.name "Your Name"
	$ git config --global user.email "your@name.com"

Tanpa menggunakan terminal kita juga bisa langusung mengedit file gitconfig yang ada di direktori home kamu. Sehingga jika kita lihat isinya sebagai berikut .
::
	$ vi ~/.gitconfig

::

	[user]
        	name = Your Name
        	email = your@name.com

Ada konfigurasi yang biasa saya tambahkan yaitu
::

	$ git config --global color.ui true

konfigurasi itu berfungsi bisa memberi warna khusus pada saat kita nanti menggunakan perintah yang ada di git.

Sehingga konfigurasi .gitconfig sekarang menjadi
::

	[user]
        	name = Fanani M. Ihsan
	        email = contact@fanani.net
	[color]
        	ui = true


Masih banyak git global conig yang lain . Dengan menggunakan konfigurasi diatas saya kira sudah cukup dengan kebutuhan yang akan kita gunakan.
