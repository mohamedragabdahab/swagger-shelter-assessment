# ServiceShelterSwaggerClient
This is a sample Shelter server [http://swagger.io](http://swagger.io) or on  [irc.freenode.net, #swagger](http://swagger.io/irc/).

This PHP package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 1.0.1
- Package version: 1.0.1
- Build package: io.swagger.codegen.languages.PhpClientCodegen

## Requirements

PHP 5.5 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "git",
      "url": "https://github.com/mohamedragabdahab/service-shelter-swagger-client.git"
    }
  ],
  "require": {
    "mohamedragabdahab/service-shelter-swagger-client": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/ServiceShelterSwaggerClient/vendor/autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Mohamed\SearchShelter\SwaggerClient\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Mohamed\SearchShelter\SwaggerClient\Model\Animal(); // \Mohamed\SearchShelter\SwaggerClient\Model\Animal | Animal object that needs to be added to the store

try {
    $apiInstance->addAnimal($body);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->addAnimal: ', $e->getMessage(), PHP_EOL;
}

?>
```

## Documentation for API Endpoints

All URIs are relative to *https://virtserver.swaggerhub.com/mohamedragabdahab/Animal-Salvation-Army/1.0.0*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*DefaultApi* | [**addAnimal**](docs/Api/DefaultApi.md#addanimal) | **POST** /animal | Add a new animal to shelter
*DefaultApi* | [**addShelter**](docs/Api/DefaultApi.md#addshelter) | **POST** /shelter | Add a new shelter
*DefaultApi* | [**addWorker**](docs/Api/DefaultApi.md#addworker) | **POST** /worker | Add a new worker to shelter
*DefaultApi* | [**deleteAnimal**](docs/Api/DefaultApi.md#deleteanimal) | **DELETE** /animal/{animalId} | Delete animal from the system
*DefaultApi* | [**deleteShelter**](docs/Api/DefaultApi.md#deleteshelter) | **DELETE** /shelter/{shelterId} | Delete shelter from the system
*DefaultApi* | [**deleteWorker**](docs/Api/DefaultApi.md#deleteworker) | **DELETE** /worker/{workerId} | Delete worker from the system
*DefaultApi* | [**listShelterAnimals**](docs/Api/DefaultApi.md#listshelteranimals) | **GET** /shelter/{shelterId}/animals | List worker of a shelter
*DefaultApi* | [**listShelterWorkers**](docs/Api/DefaultApi.md#listshelterworkers) | **GET** /shelter/{shelterId}/workers | List worker of a shelter


## Documentation For Models

 - [Animal](docs/Model/Animal.md)
 - [Customer](docs/Model/Customer.md)
 - [Shelter](docs/Model/Shelter.md)
 - [Worker](docs/Model/Worker.md)


## Documentation For Authorization

 All endpoints do not require authorization.


## Author

apiteam@swagger.io


