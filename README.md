<p align="center">
    <h1 align="center">Web Development Tools</h1>
</p>

Ini adalah bentuk mini dari tools <a href="https://laradock.io" target="_blank">laradock.io</a>

Features:
- mariadb
- memcached
- mongo
- mysql
- postgresql
- nginx
- php-fpm

Cara pakai:
------------
- Install docker dan docker-compose
- Clone repository ini
    ~~~
    $git clone https://github.com/sangbima/webdevtools.git
    ~~~
- Buat folder data di dalam direktori hasil clone
    ~~~
    $cd webdevtools
    $mkdir data
    ~~~
- Jalankan perintah:
    ~~~
    $docker-compose up -d nginx postgres workspace
    ~~~
- Untuk masuk ke container workspace, jalankan perintah ini:
    ~~~
    $docker-compose exec --user webdev workspace bash
    ~~~

License: MIT
