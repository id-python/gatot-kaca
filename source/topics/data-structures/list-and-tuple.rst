==============
List dan Tuple
==============
              
Sekarang waktunya untuk memperkenalkan struktur data dalam Python: *list* dan *tuple*. Yang saya maksudkan: *list* maupun *tuple* merupakan kumpulan dari sekelompok data. Data apa saja? Data yang merupakan anggota *list* dan *tuple* dapat berupa angka atau kata. *List* maupun *tuple* bahkan dapat beranggotakan *list* maupun *tuple* yang lain.

Contoh dari *list*::

    list_angka = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
    list_kata = ["satu", "dua", "tiga", "empat", "lima", "enam", "tujuh", "delapan", "sembilan", "sepuluh"]
    list_angka_kata = [1, "dua", 3, "empat", 5, "enam", 7, "delapan", 9, "sepuluh"]
    print list_angka
    print list_kata
    print list_angka_kata
	
maka akan menghasilkan::

    [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
    ['satu', 'dua', 'tiga', 'empat', 'lima', 'enam', 'tujuh', 'delapan', 'sembilan', 'sepuluh']
    [1, 'dua', 3, 'empat', 5, 'enam', 7, 'delapan', 9, 'sepuluh']
	
kita mendefinisikan 3 buah variabel *list* yang masing-masing berisikan 10 anggota:

* *list_angka* beranggotakan 10 buah angka
* *list_kata* beranggotakan 10 buah kata/teks/string
* *list_angka_kata* beranggotakan 10: 5 buah angka, dan 5 buah kata

Contoh dari *tuple*::

    tuple_angka = (1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
    tuple_kata = ("satu", "dua", "tiga", "empat", "lima", "enam", "tujuh", "delapan", "sembilan", "sepuluh")
    tuple_angka_kata = (1, "dua", 3, "empat", 5, "enam", 7, "delapan", 9, "sepuluh")
    print tuple_angka
    print tuple_kata
    print tuple_angka_kata

yang akan menghasilkan::

    (1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
    ('satu', 'dua', 'tiga', 'empat', 'lima', 'enam', 'tujuh', 'delapan', 'sembilan', 'sepuluh')
    (1, 'dua', 3, 'empat', 5, 'enam', 7, 'delapan', 9, 'sepuluh')

kita telah mendefinisikan 3 buah variabel *tuple* yang masing-masing beranggotakan 10:

* *tuple_angka* beranggotakan 10 buah angka
* *tuple_kata* beranggotakan 10 buah kata/teks/string
* *tuple_angka_kata* beranggotakan 10: 5 buah angka, dan 5 buah kata

Lalu, contoh *list* ataupun *tuple* yang berisikan *list* ataupun *tuple*::

    list_campur = [[1, "dua"], 3, "empat", (5, "enam"), 7, "delapan", 9, "sepuluh"]
    tuple_campur = (1, "dua", (3, "empat"), 5, "enam", [7, "delapan"], 9, "sepuluh")

    print list_campur
    print tuple_campur

yang akan menghasilkan::

    [[1, 'dua'], 3, 'empat', (5, 'enam'), 7, 'delapan', 9, 'sepuluh']
    (1, 'dua', (3, 'empat'), 5, 'enam', [7, 'delapan'], 9, 'sepuluh')
	
Nah, coba hitung berapa jumlah anggota dari *list_campur* dan *tuple_campur*?

**Jawab**::
    
	list_campur memiliki 8 anggota: 1 list, 3 angka, 3 kata, dan 1 tuple. 
	tuple_campur memiliki 8 anggota juga: 3 angka, 3 kata, 1 tuple, dan 1 list

Apakah jawaban kamu benar?

Kegunaan *list* dan *tuple*
===========================

Pertanyaan yang penting: "Lalu apa kegunaan list dan tuple?". Jawabnya: untuk membuat pembuatan progran lebih mudah. Bayangkan misalnya Boss dari contoh ayam dan bebek meminta: "Tolong dong laporkan daftar pembeli kita!", bisa saja kita membuat program seperti ini::

    #contoh5.py
    #Program untuk menampilkan daftar pelanggan

    pelanggan1 = "Bejo"
    pelanggan2 = "Karyo"
    pelanggan3 = "Tarjo"
    pelanggan4 = "Udin"
    pelanggan5 = "Asep"
    pelanggan6 = "Aminah"
    pelanggan7 = "Iyah"
    pelanggan8 = "Joni"
    pelanggan9 = "Siti"
    pelanggan10 = "Citra"

    print "Daftar pembeli:"
    print "1.", pelanggan1
    print "2.", pelanggan2
    print "3.", pelanggan3
    print "4.", pelanggan4
    print "5.", pelanggan5
    print "6.", pelanggan6
    print "7.", pelanggan7
    print "8.", pelanggan8
    print "9.", pelanggan9
    print "10.", pelanggan10

atau alternatifnya bila menggunakan *list*::

    #contoh5a.py
    #Program untuk menampilkan daftar pelanggan menggunnakan list

    pelanggan = ["Bejo", "Karyo", "Tarjo", "Udin", "Asep", "Aminah", "Iyah", "Joni", "Siti", "Citra"]


    print "Daftar pembeli:"

    cacah = 0
    while cacah < 10:
        print cacah+1, pelanggan[cacah]
        cacah = cacah + 1

yang apabila dijalankan akan memberikan hasil yang sama::

    Daftar pembeli:
    1 Bejo
    2 Karyo
    3 Tarjo
    4 Udin
    5 Asep
    6 Aminah
    7 Iyah
    8 Joni
    9 Siti
    10 Citra
	
*contoh5.py* kita perlu mengetikkan 21 baris program (tanpa menghitung komentar dan baris kosong), dibandingkan hanya 6 baris program di *contoh5a.py*. Bayangkan jika pembeli ada 100 orang!

Indeks
======

Nah, mari kita tilik kembali bagian program dari *contoh5a.py*::

    cacah = 0
        while cacah < 10:
            print cacah+1, pelanggan[cacah]
            cacah = cacah + 1
			
kita mendefinisikan sebuah variabel *cacah* yang dalam perulangan *while...* nilainya dinaikkan satu demi satu (cacah = cacah + 1). Variabel *cacah* kemudan digunakan untuk memanggil anggota dari *list* *pelanggan* (pelanggan[cacah]). Di sini kita memanggil anggota list melalui *indeks*. Indeks merupakan bilangan yang menunjukkan urutan letak anggota. Indeks mirip seperti saat kita bersekolah dulu, masing-masing kita mendapat no urut kelas (saat kuliah no urut kelas saya 22....) sehingga saat awal pelajaran dosen memanggil "22! Mico!" maka saya menjawab: "22, hadir!". Namun perlu diingat, jika no urut kelas dimulai dari *1*,, *indeks* untuk *list* maupun *tuple* dimulai dari *0*. Sehingga jika kita memiliki list::

    pelanggan = ["Bejo", "Karyo", "Tarjo", "Udin", "Asep", "Aminah", "Iyah", "Joni", "Siti", "Citra"]
 
maka::

    pelanggan[0] = "Bejo"
    pelanggan[1] = "Karyo"
    pelanggan[2] = "Tarjo"
	
dan seterusnya.

in
==

*in* adalah operator dalam Python untuk mengetes apakah sebuah nilai merupakan anggota dari sebuah *list* atau *tuple*, misalnya::

    pelanggan = ["Bejo", "Karyo", "Tarjo", "Udin", "Asep", "Aminah", "Iyah", "Joni", "Siti", "Citra"]
    print "Udin" in pelanggan
    print "Thomas" in pelanggan
	
akan menghasilkan::

    True
    False
	
atau dengan kata lain: "Udin" adalah anggota pelanggan, sedangkan "Thomas" bukan salah satu anggota pelanggan
 
