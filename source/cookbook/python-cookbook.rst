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
	
    