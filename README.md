# wilsonMCV_framework
MVC framework to begin any php build

If you change the root name Be sure to change the .htaccess file in the public folder to reflect your own project. See below (RewriteBase).

```
<IfModule mod_rewrite.c>
  Options -Multiviews
  RewriteEngine On
  RewriteBase /**ROOT_DIRECTORY_NAME**/public
  RewriteCond %{REQUEST_FILENAME} !-d
  RewriteCond %{REQUEST_FILENAME} !-f
  RewriteRule  ^(.+)$ index.php?url=$1 [QSA,L]
</IfModule>
```

