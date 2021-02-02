Web Development Tools

Ini adalah bentuk mini dari tools dari laradock.io

Features:
- mariadb
- memcached
- mongo
- mysql
- postgresql
- nginx
- php-fpm

Cara pakai:
- Install docker dan docker-compose
- Clone repository ini
- Buat folder data di dalam direktori hasil clone
    $cd webdevtools
    $mkdir data
- Jalankan perintah: 
    $docker-compose up -d nginx postgres workspace
- Untuk masuk ke container workspace, jalankan perintah ini:
    $docker-compose exec --user webdev workspace bash

License: MIT
