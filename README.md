# Backup Pro REST Client

A simple REST cient to interact with Backup Pro installations

## Installation
Add `backup-pro/rest-client` as a requirement to `composer.json`:

```bash
$ composer require backup-pro/rest-client
```

## Simple Example


```php
<?php
$client = new Client();
$backups = $client->setApiKey($api_key)
                 ->setApiSecret($api_secret)
                 ->setSiteUrl($api_endpoint_url)
                 ->get('/backups');

```

## Authentication

Backup Pro uses HMAC-SHA authentication which is a simple key / secret paradigm to create hashed signatures. You can get/set your api key and secret from your individual Backup Pro installations. 

