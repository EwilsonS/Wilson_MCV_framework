# wilsonMCV_framework
MVC framework to begin any php build

Be sure to change the .htaccess file to reflect your own project
`
<IfModule mod_rewrite.c>
  Options -Multiviews
  RewriteEngine On
  RewriteBase /<strong>ROOT_DIRECTORY_NAME</strong>/public
  RewriteCond %{REQUEST_FILENAME} !-d
  RewriteCond %{REQUEST_FILENAME} !-f
  RewriteRule  ^(.+)$ index.php?url=$1 [QSA,L]
</IfModule>
`
