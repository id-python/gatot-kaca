Ini adalah proyek penulisan artikel/tutorial sebagai sarana pengembangan programmer Python Indonesia.

Update terbaru akan selalu ditampilkan dalam website project ini dan source akan selalu tersedia. Tetapi jika anda ingin memiliki lokal copy, berikut ini adalah instruksinya :

* Pastikan anda memiliki sphinx dalam system anda, jika belum anda bisa meng-installnya melalui pip maupun easy_install ::

    sudo pip install sphinx

* Clone repository menggunakan git ::
    
    git clone git@github.com:id-python/gatot-kaca.git


* Masuk dalam directory tersebut dan anda bisa menghasilkan html dengan perintah :
  ::    
    
    make html

  atau untuk generate epub untuk dibaca di smartphone/tablet : ::
    
    make epub


Note
----

Untuk para kontributor, agar repositori yang anda fork selalu up to date dengan repositori utama lakukan hal berikut : ::

    git remote add upstream git://github.com/id-python/gatot-kaca.git
    git fetch upstream
    git merge upstream/master

Untuk melanjutkan, tidak perlu melakukan remote add kembali cukup dengan : ::

    git fetch upstream
    git merge upstream/master
