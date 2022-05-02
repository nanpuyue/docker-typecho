# typecho

```
/** 定义数据库参数 */
$db = new Typecho_Db('Pdo_Mysql', 'typecho_');
$db->addServer(array (
  'host' => '',
  'user' => '__USER__',
  'password' => '__PASSWORD__',
  'charset' => 'utf8',
  'port' => '',
  'database' => '__DATABASE__',
), Typecho_Db::READ | Typecho_Db::WRITE);
Typecho_Db::set($db);
```


# nginx

```
# pass PHP scripts to FastCGI server
location ~ \.php$ {
    include snippets/fastcgi-php.conf;
    fastcgi_pass unix:/var/run/php/php7.3-fpm.sock;
}
```

