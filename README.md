# Laravel 8 以 Markdown 格式撰寫文件

引入 binarytorch 的 larecipe 套件來擴增使用 Markdown 格式撰寫的文件並且看起來不會像是由許多標籤或是格式指令所構成，強調的是它的可讀性。Markdown 是一種輕量級標記式語言， 它有純文字標記的特性，讓編寫的可讀性提高，這是在以前很多電子郵件中就已經有的寫法，而目前也有很多網站都使用來撰寫說明文件。

## 使用方式
- 把整個專案複製一份到你的電腦裡，這裡指的「內容」不是只有檔案，而是指所有整個專案的歷史紀錄、分支、標籤等內容都會複製一份下來。
```sh
$ git clone
```
- 將 __.env.example__ 檔案重新命名成 __.env__，如果應用程式金鑰沒有被設定的話，你的使用者 sessions 和其他加密的資料都是不安全的！
- 當你的專案中已經有 composer.lock，可以直接執行指令以讓 Composer 安裝 composer.lock 中指定的套件及版本。
```sh
$ composer install
```
- 產生 Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan key:generate
```
- 在瀏覽器中輸入已定義的路由 URL 來訪問，例如：http://127.0.0.1:8000。
- 你可以經由 `/docs` 來進行文件產生。

----

## 畫面截圖
![](https://i.imgur.com/Hfihryn.png)
> 可以呈現精美的文件
