# php artisan serve と apachaの違い
Laravelをローカルで動かす方法が2つあったので調べた。
## php artisan serve
[https://anytimesnotes.com/archives/1750](url)

Laravelサーバーを起動するためのコマンド。
明示的にホスト名やポート番号も指定できる。

php artisan serveはserver.phpを起動するコマンド。
[https://detail.chiebukuro.yahoo.co.jp/qa/question_detail/q12184231152](url)
> `php artisan serve`
> 
> は
> 
> `php -S localhost:8000 server.php`
> 
> をラップしたコマンドで、これはPHP自身が持つ「ビルトインサーバ」というWebサーバ機能を使っています。

## apach
