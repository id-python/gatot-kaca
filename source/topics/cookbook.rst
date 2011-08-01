=================
Buku Resep Python
=================

Menukar Nilai Antar Variabel tanpa Variabel Sementara
=====================================================

Untuk menukar nilai antar variabel di dalam python tidak perlu menggunakan variabel sementara, misalnya untuk menukar nilai antar variabel a,b,c

Python::

    a,b,c = b,c,a
	
Hal yang sama jika dilakukan dalam bahasa C::
    
	temp = a
	a = b
	b = c
	c = temp
	
Mengambil Sebuah Nilai dari Dictionary
======================================

Misalnya akan diambil nilai berdasarkan kunci dari dictionary::

    d ={'try':'coba', 'again':'lagi'}

cara yang sering dilakukan adalah mengecek apakah dictionary memiliki kunci yang diminta::

    if d.has_key('try'):
        print d['try']
    else:
        print 'nggak ketemu'
		
namun ada cara yang lebih sederhana::

    print d.get('try', 'nggak ketemu')

lebih sederhana dan mempersedikit kesalahan ketik


Menampilkan index dari suatu iterable (list, dictionary)
========================================================

Jika kita ingin menampilkan index dalam loop, kita bisa menggunakan enumerate, contoh : ::

    >>> a = ["apple", "banana", "orange", "mango", "grape"]
    >>> for index, item in enumerate(a):
    >>>     print index, item
    0 apple
    1 banana
    2 orange
    3 mango
    4 grape


Fungsi untuk Membuat Dictionary
===============================

Dalam membuat aplikasi python, dictionary adalah tipe data yang sering digunakan. Misalnya ingin membuat dictionary untuk translasi bahasa Inggris ke Indonesia seperti ini::

    kamus = {'red' : 'merah', 'green' : 'hijau', 'blue' : 'biru'}
	
kita dapat memubuat fungsi yang memudahkan kita untuk membuat dictionary seperti di atas::

    def makedict(**kwargs):
        return kwargs
		
    kamus = makedict(red='merah', green='hijau', blue='biru')
	
dan hasilnya::

    >>> print kamus
    {'blue': 'biru', 'green': 'hijau', 'red': 'merah'} 
