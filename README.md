# php-rate-limit
Simple Rate Limit in PHP

## HOW TO USE

Ex: 5 request in 2 seconds

```php
$i = 1;
while ($i <= 7) {
    Ratelimiter::check(5, 2);
    echo "foo {$i} - ".date('i:s').PHP_EOL;
    $i++;
}
echo 'FINISH';
```
