php_xdebug.dll is for php version 8.2

copy php_xdebug.dll into C:\xampp\php\ext

add this lines to php.ini (C:\xampp\php\php.ini)

[XDebug]
xdebug.mode=debug
xdebug.start_with_request=yes
zend_extension = "C:\xampp\php\ext\php_xdebug.dll"

copy .vscode into root of working project to get launch configurations for debugging in vscode

first go php artisan serve, and than npm run dev, and than run Listen for Xdebug configuration