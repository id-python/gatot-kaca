Python Cookbook
================

Menukar Nilai Antar Variabel tanpa Variabel Sementara
----------------------------------------------------
Untuk menukar nilai antar variabel di dalam python tidak perlu menggunakan variabel sementara, misalnya untuk menukar nilai antar variabel a,b,c

Python::

    a,b,c = b,c,a
	
Hal yang sama jika dilakukan dalam bahasa C::
    
	temp = a
	a = b
	b = c
	c = temp
	
Mengambil Sebuah Nilai dari Dictionary
---------------------------------------
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
    