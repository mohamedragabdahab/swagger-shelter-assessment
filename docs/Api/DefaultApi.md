# Swagger\Client\DefaultApi

All URIs are relative to *https://virtserver.swaggerhub.com/mohamedragabdahab/Animal-Salvation-Army/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addAnimal**](DefaultApi.md#addAnimal) | **POST** /animal | Add a new animal to shelter
[**addShelter**](DefaultApi.md#addShelter) | **POST** /shelter | Add a new shelter
[**addWorker**](DefaultApi.md#addWorker) | **POST** /worker | Add a new worker to shelter
[**deleteAnimal**](DefaultApi.md#deleteAnimal) | **DELETE** /animal/{animalId} | Delete animal from the system
[**deleteShelter**](DefaultApi.md#deleteShelter) | **DELETE** /shelter/{shelterId} | Delete shelter from the system
[**deleteWorker**](DefaultApi.md#deleteWorker) | **DELETE** /worker/{workerId} | Delete worker from the system
[**listShelterAnimals**](DefaultApi.md#listShelterAnimals) | **GET** /shelter/{shelterId}/animals | List worker of a shelter
[**listShelterWorkers**](DefaultApi.md#listShelterWorkers) | **GET** /shelter/{shelterId}/workers | List worker of a shelter


# **addAnimal**
> addAnimal($body)

Add a new animal to shelter

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Swagger\Client\Model\Animal(); // \Swagger\Client\Model\Animal | Animal object that needs to be added to the store

try {
    $apiInstance->addAnimal($body);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->addAnimal: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\Animal**](../Model/Animal.md)| Animal object that needs to be added to the store |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **addShelter**
> addShelter($body)

Add a new shelter

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Swagger\Client\Model\Shelter(); // \Swagger\Client\Model\Shelter | Shelter object that needs to be added to the store

try {
    $apiInstance->addShelter($body);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->addShelter: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\Shelter**](../Model/Shelter.md)| Shelter object that needs to be added to the store |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **addWorker**
> addWorker($body)

Add a new worker to shelter

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Swagger\Client\Model\Worker(); // \Swagger\Client\Model\Worker | Worker object that needs to be added to the store

try {
    $apiInstance->addWorker($body);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->addWorker: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\Worker**](../Model/Worker.md)| Worker object that needs to be added to the store |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteAnimal**
> deleteAnimal($animal_id)

Delete animal from the system

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$animal_id = 789; // int | Animal ID that needs to be deleted from the store

try {
    $apiInstance->deleteAnimal($animal_id);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->deleteAnimal: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **animal_id** | **int**| Animal ID that needs to be deleted from the store |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteShelter**
> deleteShelter($shelter_id)

Delete shelter from the system

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$shelter_id = 789; // int | Shelter ID that needs to be deleted from the store

try {
    $apiInstance->deleteShelter($shelter_id);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->deleteShelter: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shelter_id** | **int**| Shelter ID that needs to be deleted from the store |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteWorker**
> deleteWorker($worker_id)

Delete worker from the system

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$worker_id = 789; // int | Worker ID that needs to be deleted from the store

try {
    $apiInstance->deleteWorker($worker_id);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->deleteWorker: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **worker_id** | **int**| Worker ID that needs to be deleted from the store |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listShelterAnimals**
> \Swagger\Client\Model\Animal listShelterAnimals($shelter_id)

List worker of a shelter

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$shelter_id = 789; // int | Shelter ID that needs to be deleted from the store

try {
    $result = $apiInstance->listShelterAnimals($shelter_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->listShelterAnimals: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shelter_id** | **int**| Shelter ID that needs to be deleted from the store |

### Return type

[**\Swagger\Client\Model\Animal**](../Model/Animal.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **listShelterWorkers**
> \Swagger\Client\Model\Worker listShelterWorkers($shelter_id)

List worker of a shelter

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$shelter_id = 789; // int | Shelter ID that needs to be deleted from the store

try {
    $result = $apiInstance->listShelterWorkers($shelter_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->listShelterWorkers: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shelter_id** | **int**| Shelter ID that needs to be deleted from the store |

### Return type

[**\Swagger\Client\Model\Worker**](../Model/Worker.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

