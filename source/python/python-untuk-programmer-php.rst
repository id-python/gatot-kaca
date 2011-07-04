Python Untuk Programmer PHP
===========================

Pada kesempatan kali, marilah kita belajar sekilas tentang bahasa pemrograman Python.

Perulangan
----------
PHP (for loop)

.. code-block:: php
    
    <?php
    for (i=0;i<10;i++) {
        print i;
    }
    ?>

Python (for loop)::

    for i in range(0, 10):
        print(i)

PHP (foreach loop)

.. code-block:: php

    <?php
    $fruits = ["manggo", "apple", "banana", "grape"];
    foreach ($fruits as $fruit) {
        print $fruit;
    }
    ?>

Python (for loop)::

    fruits = ["manggo", "apple", "banana", "grape"];
    for fruit in  fruits:
        print(fruit)


Seleksi
-------

PHP (if … else … )

.. code-block:: php

    <?php
    if ($value == 3) {
        print "ok";
    } else {
        print "error";
    }
    ?>

Python (if … else ….)::

    if value == 3:
        print("ok")
    else:
        print("error")

    
Fungsi
------

.. code-block:: php

    <?php
    function multiply($a, $b) {
        return $a * $b;
    }
    ?>


Python (function)::

    def multiply(a, b):
        return a * b


Kelas
-----

PHP (class)

.. code-block:: php

    <?php
    class Mobil {
        function __construct() {
        }
    }
    ?>



Python (class)::

    class Mobil():
        def __init__(self):
             pass


Ini hanyalah kursus kilat bagi programmer PHP yang ingin sedikit mengetahui tentang Python, dan bagaimana melakukan hal-hal sederhana dengan Python.