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
- Buat file .env dengan mencopy file env-example
    ~~~
    $cp env-example .env
    ~~~
- Buat virtualhost yang akan kita pakai, misal: webapp.test:
    ~~~
    $cp nginx/sites/app.conf.example nginx/sites/webapp.test.conf
    ~~~
    Edit file webapp.test.conf, sesuaikan dengan virtualhost yang ingin kita buat
    ~~~
    $vi nginx/sites/webapp.test.conf
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
