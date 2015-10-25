# 佈告欄

## 如何使用

1.請先將此專案 clone 下來

```
$ git clone git@github.com:Peter654q/bulletin.git
```

2.進入專案目錄

```
$ cd bulletin
```

3.將 .env.example 複製到 .env

```
$ cp .env.example .env
```

4.執行 composer install 來安裝需要的套件

```
$ composer install
```

5.產生 laravel 用來加密的 key

```
$ php artisan key:generate
```

6.執行以下指令

```
$ php artisan clear-compiled
$ php artisan optimize
```

7.修改 .env 的設定，以符合你的環境

## 使用 Homestead

若你希望為這個專案單獨準備一個 Homestead 虛擬機，而不使用全域的 Homestead，那你可以下：

```
$ php vendor/bin/homestead make
```

他會產生 Homestead.yaml 在此專案的目錄下，根據你的需求修改過後即可使用

```
$ vagrant up
```

來開啟虛擬機

詳細請看 http://laravel.com/docs/5.1/homestead#per-project-installation
