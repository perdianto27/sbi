Cara Clone Menjalankan Project Laravel

- Buka project laravel yang akan kita clone dari github.
- Download saja langsung file ZIP-nya, atau bisa anda clone langsung pada komputer anda melalui syntax github seperti ini,

“git clone https://github.com/perdianto27/laraadmin.git”

- Jika sudah di download silahkan unzip atau unrar dan tempatkan pada url yang dapat diakses nantinya, sehingga file project laravel yang sudah di download atau di clone.
- Pada saat anda buka url project laravel tersebut akan muncul error. Untuk memperbaikinya lakukan langkah ini :

“Composer dumpautoload”
“Composer update –no-scripts”

- Jika sudah "OK" buka kembali url project laravelnya, jika muncul error.
- Mensetting database-nya.
- Jika project laravel menggunakan env, Maka pengaturan database diletakkan pada file .env, jika tidak ada file .env maka copy saja file .env.example, ubah namanya menjadi .env
- Isi database dengan nama database, username dengan username akses database, dan password dengan password akses database anda pada phpmyadmin.
- Jika project laravel tidak menggunakan env, maka langsung ubah saja file database.php pada path config.
- Isi database dengan nama database, username dengan username akses database, dan password dengan password akses database anda pada phpmyadmin.
- Kemudian buka url project pada terminal dan lakukan migrate

"php artisan migrate" 
- Jika muncul error, berarti setting database anda masih salah,
-Buka kembali url project anda pada browser, jika muncul error seperti ini,

"No supported encrypter found. The cipher and / or key length are invalid."

- Berarti key laravel anda salah untuk memperbaikinya tinggal di

"php artisan key:generate"

- Buka kembali url project anda pada browser, maka akan tampak tampilan project anda.



# Laravel PHP Framework

[![Build Status](https://travis-ci.org/laravel/framework.svg)](https://travis-ci.org/laravel/framework)
[![Total Downloads](https://poser.pugx.org/laravel/framework/d/total.svg)](https://packagist.org/packages/laravel/framework)
[![Latest Stable Version](https://poser.pugx.org/laravel/framework/v/stable.svg)](https://packagist.org/packages/laravel/framework)
[![Latest Unstable Version](https://poser.pugx.org/laravel/framework/v/unstable.svg)](https://packagist.org/packages/laravel/framework)
[![License](https://poser.pugx.org/laravel/framework/license.svg)](https://packagist.org/packages/laravel/framework)

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable, creative experience to be truly fulfilling. Laravel attempts to take the pain out of development by easing common tasks used in the majority of web projects, such as authentication, routing, sessions, queueing, and caching.

Laravel is accessible, yet powerful, providing tools needed for large, robust applications. A superb inversion of control container, expressive migration system, and tightly integrated unit testing support give you the tools you need to build any application with which you are tasked.

## Official Documentation

Documentation for the framework can be found on the [Laravel website](http://laravel.com/docs).

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](http://laravel.com/docs/contributions).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell at taylor@laravel.com. All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT).
