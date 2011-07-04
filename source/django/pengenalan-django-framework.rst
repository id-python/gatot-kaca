Pengenalan Django Framework
===========================

Apa itu Django Framework?  
-------------------------
Django adalah Python web framework yang mendukung pembuatan web dengan sangat cepat. Mengadopsi sistem MTV, yaitu Model, Template dan View.

Model adalah layer yang digunakan untuk berinteraksi dengan database, Template adalah layer presentasi untuk HTML, XML dan lainnya, sedangkan View adalah layer yang berisikan logika yang mengolah data dari model dan mengirimkannya ke dalam Template.

Nama Django sendiri diambil dari seorang gitaris bernama Django Reinhardt.

Apa sih kelebihan Django Framework?
Berikut adalah beberapa kelebihan yang dimiliki oleh Django :

*   Object-relational mapper  
    Definisikan data model dalam Python, dan gunakan API untuk mengakses data tersebut.
*   Automatic admin interface  
    Django menyediakan admin interface secara otomatis, sehingga anda tidak perlu repot – repot untuk membuatnya.
*   Elegant URL design  
    Pembuatan URL yang lebih mudah dan fleksibel.
*   Template system  
    Sistem template Django merupakan salah satu yang bagian yang paling powerful.
*   Cache system  
    Gunakan memcache atau sistem cache dengan mudah.
*   Internationalization  
    Django telah didesain untuk mempermudah anda dalam membuat web multi bahasa.


Instalasi Django
----------------
Sebelum memulai instalasi Django, pastikan Python terinstal dalam sistem operasi anda.

Download Django source code
Ekstrak file tersebut, contoh (Linux)
::

    tar -xvf Django-1.1.1.tar.gz

Masuk ke dalam folder hasil ekstrak sebelumnya. Lalu lakukan instalasi Django
::

    cd Django-1.1.1
    sudo python setup.py install

Selamat. Django telah terinstal dalam sistem anda.

Hello world dalam Django
------------------------
Pada terminal, buatlah proyek baru misal dengan nama hello
::

    django-admin startproject hello

Buka views.py, lalu ketikan kode berikut
::

    from django.http import HttpResponse
 
    def index(request):
        return HttpResponse("Hello, world.")


Buka urls.py, lalu berikan url seperti berikut : ::

    from django.conf.urls.defaults import *
 
    urlpatterns = patterns('',
        url(r'^$', 'views.index'),
    )

Jalankan Django development server dengan perintah
::

    ./manage.py runserver

Buka browser anda, dan akses alamat berikut http://localhost:8000

