# Swagger\Client\DefaultApi

All URIs are relative to *http://v3.openaviationdata.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**aircraftGet**](DefaultApi.md#aircraftGet) | **GET** /aircraft | Aircraft Data
[**helloGet**](DefaultApi.md#helloGet) | **GET** /hello | Hello World Test
[**notamGet**](DefaultApi.md#notamGet) | **GET** /notam | Notice to Airmen
[**sigmetCurrentGet**](DefaultApi.md#sigmetCurrentGet) | **GET** /sigmet/current | Current SIGMET Data
[**sigmetGeojsonGet**](DefaultApi.md#sigmetGeojsonGet) | **GET** /sigmet/geojson | Current SIGMET Data in GeoJSON Format


# **aircraftGet**
> \Swagger\Client\Model\Aircraft[] aircraftGet()

Aircraft Data

Basic aircraft and performance data as registered with ICAO.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();

try {
    $result = $api_instance->aircraftGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->aircraftGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\Aircraft[]**](../Model/Aircraft.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **helloGet**
> \Swagger\Client\Model\InlineResponse200 helloGet()

Hello World Test

The SIGMET Endpoint provides information about current SIGMETs in real-time.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();

try {
    $result = $api_instance->helloGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->helloGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\InlineResponse200**](../Model/InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **notamGet**
> \Swagger\Client\Model\NOTAM[] notamGet($station)

Notice to Airmen

The NOTAM Endpoint provides information about Notices to Airmen and is available in real-time.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$station = "station_example"; // string | Station ICAO (Can be airport, FIR, or ATC facility)

try {
    $result = $api_instance->notamGet($station);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->notamGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **station** | **string**| Station ICAO (Can be airport, FIR, or ATC facility) |

### Return type

[**\Swagger\Client\Model\NOTAM[]**](../Model/NOTAM.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sigmetCurrentGet**
> \Swagger\Client\Model\SIGMET[] sigmetCurrentGet()

Current SIGMET Data

The SIGMET Endpoint provides information about current SIGMETs in real-time.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();

try {
    $result = $api_instance->sigmetCurrentGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sigmetCurrentGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\SIGMET[]**](../Model/SIGMET.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sigmetGeojsonGet**
> sigmetGeojsonGet()

Current SIGMET Data in GeoJSON Format

The SIGMET Endpoint provides information about current SIGMETs in GeoJSON format.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();

try {
    $api_instance->sigmetGeojsonGet();
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sigmetGeojsonGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

