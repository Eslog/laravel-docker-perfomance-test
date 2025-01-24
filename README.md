# laravel-docker-perfomance-test

## Apache + PHPのモジュール版の環境構築
1. コマンドを叩く
```
cd apache-php-module
docker compose up -d
docker compose exec app bash
composer create-project --prefer-dist "laravel/laravel=11.*" .
chmod -R 777 storage bootstrap/cache
```
2. サイトにアクセス
http://localhost:3000
