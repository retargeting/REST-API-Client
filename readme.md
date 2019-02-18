# Retargeting REST API Client

```bash
composer require retargeting/rest-api-client
```

```php
<?php

include "vendor/autoload.php";

use Retargeting\Client;

// use your REST API KEY from Retargeting Admin Panel
$client = new Client("REST_API_KEY");

// set response format to JSON
$client->setResponseFormat("json");

// not decode the string
$client->setDecoding(false);

// check discount code
$response = $client->discount->check("DISCOUNT_CODE");

var_dump($response);

```
