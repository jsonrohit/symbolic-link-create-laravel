# Symbolic-link-create-laravel
### Storage data not show publicly than use this `cmd`
`php artisan storage:link`
if this `cmd` not working.

###  than create manully symbolic link
```php
    $targetFolder = $_SERVER['DOCUMENT_ROOT'].'/storage/app/public';
    $linkFolder = $_SERVER['DOCUMENT_ROOT'].'/public/storage';
    symlink($targetFolder,$linkFolder);
    echo 'Symlink process successfully completed';
```
