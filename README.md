
## Laravelサーバの作成
1) next_tweet フォルダをVSCodeで開く

2) ターミナルを開いて、Laravelプロジェクトを作成

```
composer create-project laravel/laravel server
```

3) serverプロジェクトを新しいウィンドウで開く

```
code server
```

4) Laravelサーバの起動

```
php artisan serve
```

5) XAMPPのApache、MySQLを起動

6) phpMyAdmin で 「next_tweet」データベースを作成

7) .env のDB設定「next_tweet」

```
DB_DATABASE=next_tweet
```

## ログイン認証（SSR版）

1) Laravel Breezeをダウンロード

```
composer require laravel/breeze --dev
```

2) Laravel Breezeをインストール

```
php artisan breeze:install blade
```

3) ブラウザで確認

http://localhost:8000


## DB作成
1) DBマイグレートする

```
php artisan migrate
```

2) phpMyAdminでテーブル確認する

3) Registerからユーザ登録する

4) Tweetモデルの作成

```
php artisan make:model Tweet -m
```

5) app/Models/Tweet.php の修正


