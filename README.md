# php
PHP apifunc - php.latency.pl

# functions:
+ ping.php
+ response.php
+ response_curl.php
+ response_true.php 


# example

```php
apifunc([
    'https://php.defjson.com/def_json.php',
    'https://php.latency.pl/ping.php'
], function () {
    global $domain;
    $ping =  ping($domain, 80, 10);
    echo def_json("", [
        "ping" => $ping,
        "domain" => $domain
    ]);
});
```

---
+ [edit](https://github.com/latency-pl/php/edit/main/README.md)

```
https://github.com/latency-pl/php.git
```
