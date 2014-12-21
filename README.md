RESTful cURL PHP Wrapper
========================

A simple composer based cURL wrapper providing RESTful HTTP requests


**Usage**

Add the following requirement to your composer file and do a composer install/update:

```
  "require": {
        ...
        "daa/restful-curl-php-wrapper": "1.*"
  },
```

Instantiate a new client in your code:

```
use Curl\Sdk\HttpClient;

$client = new HttpClient;
```

Make your call:

```
try {
    $response = $client->get($url);
    $response = $client->post($url, $params);
    $response = $client->put($url, $params);
    $response = $client->delete($url);
} catch(\Exception $e) {

}
```

