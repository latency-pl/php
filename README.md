# php
PHP apifunc - php.latency.pl

# functions:
+ ping.php
+ response.php
+ response_curl.php
+ response_true.php 


# example

Request

    localhost/index.php?domain=softreck.com

index.php

```php
apifunc([
    'https://php.defjson.com/def_json.php',
    'https://php.latency.pl/ping.php'
], function () {
    echo def_json("", [
        "ping" => ping($_GET['domain'], 80, 10),
        "domain" => $_GET['domain']
    ]);
});
```

Response
```json
{
    "message":	"5 ms",
    "domain":	"softreck.com"
}    
```

---
+ [edit](https://github.com/latency-pl/php/edit/main/README.md)

```
https://github.com/latency-pl/php.git
```
