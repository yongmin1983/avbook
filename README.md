<p align="center"><img src="https://github.com/guyueyingmu/avbook/blob/master/public/avbook/logo.png?raw=true"></p>

<p align="center">

<img src="https://travis-ci.org/laravel/framework.svg"> 
<img src="https://img.shields.io/packagist/php-v/symfony/symfony.svg"> 
<img src="https://img.shields.io/badge/mysql-%3E%3D5.7-brightgreen.svg"> 
<img src="https://img.shields.io/apm/l/vim-mode.svg">

</p>

[releases](https://github.com/guyueyingmu/avbook/releases/download/v.0.19.7.11/avbook_laragon.0.19.7.11.7z)

password:gyym.avbook.bt.01

#### 使用方法:

> 1.解压到 D:\laragon <br>

    2.打开 D:\laragon\laragon.exe ,点击 `启动所有`<br>
    3.点击 `网站` 或者访问 <http://avbook.test>  enjoy it

> ps:<br>

     Ⅰ. 如果没有解压到 D:\laragon 需自行修改Nginx配置，php.ini配置，并在hosts文件新增一行 ：`127.0.0.1      avbook.test` <br>
     Ⅱ. laragon终端启动爬虫前先 `git pull ` 更新到最新版本。

## License

The AVBook is open-source software licensed under the [MIT license](https://opensource.org/licenses/MIT).

gyym.avbook.bt.01

git clone https://github.com/guyueyingmu/avbook.git

cd avbook;cp .env.example .env #复制 .env.example 为 .env 并设置数据库信息

composer install

php artisan migrate

#替换 avbook/config/urlconfig.php 文件中的域名为最新域名 #从被墙域名获取：avmoo.com ;javbus.com;javlib.com

php artisan avbook:avmoo #启动 avmoo 爬虫

php artisan avbook:javbus --movie=1 --page=10 --magpage=10 #启动 javbus 爬虫

php artisan scandir --path='/moviefiles' #扫描指定目录 /moviefiles 中的文件，正则匹配番号，设置为已拥有状态

php artisan avbook:javlib --genre --movie #javlibrary 爬虫

https://www.oschina.net/p/avbook
