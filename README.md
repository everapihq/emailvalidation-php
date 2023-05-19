<p align="center">
<img src="https://app.numlookupapi.com/img/logo/emailvalidation.png" width="300"/>
</p>

# emailvalidation-php - Email Validation & Verification API

[![Latest Version on Packagist](https://img.shields.io/packagist/v/everapi/emailvalidation-php.svg?style=flat-square)](https://packagist.org/packages/everapi/emailvalidation-php)
[![Total Downloads](https://img.shields.io/packagist/dt/everapi/emailvalidation-php.svg?style=flat-square)](https://packagist.org/packages/everapi/emailvalidation-php)

This package is a PHP wrapper for [emailvalidation.io](https://emailvalidation.io) that aims to make the usage of the API as easy as possible in your project.

## Installation

You can install the package via composer:

```bash
composer require everapi/emailvalidation-php
```

## Usage

Initialize the API with your API Key (get one for free at [emailvalidation.io](https://emailvalidation.io)):

```php
$emailvalidation = new \Emailvalidation\EmailvalidationClient('YOUR-API-KEY');
```

Afterwards you can use the endpoints of the API like this:

```php
echo $emailvalidation->status();
```


```php
var_dump($emailvalidation->validate('john@doe.com', [
    'catch_all' => 1
]));
```


Learn more about endpoints, parameters and response data structure in the [docs](https://emailvalidation.io/docs).

[docs]: https://emailvalidation.io/docs
[numlookupapi.com]: https://emailvalidation.io

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
