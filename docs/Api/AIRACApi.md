# Swagger\Client\AIRACApi

All URIs are relative to *http://v3.openaviationdata.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**airacAirportGet**](AIRACApi.md#airacAirportGet) | **GET** /airac/airport | Airport
[**airacAirspaceGet**](AIRACApi.md#airacAirspaceGet) | **GET** /airac/airspace | Airspace Data
[**airacFirGet**](AIRACApi.md#airacFirGet) | **GET** /airac/fir | Flight Information Region
[**airacMoraGet**](AIRACApi.md#airacMoraGet) | **GET** /airac/mora | Minimum Off Route Altitude


# **airacAirportGet**
> \Swagger\Client\Model\Airport[] airacAirportGet($icao, $type, $capability)

Airport

The AIRAC Airport Endpoint provides information about airports worldwide and is refreshed with every AIRAC cycle.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\AIRACApi();
$icao = "icao_example"; // string | Airport ICAO code.
$type = "type_example"; // string | Can be CIV (Civilian) or MIL (Military).
$capability = "capability_example"; // string | Can be IFR, VFR, VFA, or VRF.

try {
    $result = $api_instance->airacAirportGet($icao, $type, $capability);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AIRACApi->airacAirportGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **icao** | **string**| Airport ICAO code. | [optional]
 **type** | **string**| Can be CIV (Civilian) or MIL (Military). | [optional]
 **capability** | **string**| Can be IFR, VFR, VFA, or VRF. | [optional]

### Return type

[**\Swagger\Client\Model\Airport[]**](../Model/Airport.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **airacAirspaceGet**
> \Swagger\Client\Model\Airspace[] airacAirspaceGet()

Airspace Data

The AIRAC Airspace Endpoint provides information about airspaces and is refreshed with every AIRAC cycle.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\AIRACApi();

try {
    $result = $api_instance->airacAirspaceGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AIRACApi->airacAirspaceGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\Airspace[]**](../Model/Airspace.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **airacFirGet**
> \Swagger\Client\Model\FIR[] airacFirGet($icao)

Flight Information Region

The FIR Endpoint provides information about Flight Information Regions and is refreshed with every AIRAC cycle.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\AIRACApi();
$icao = "icao_example"; // string | FIR ICAO code.

try {
    $result = $api_instance->airacFirGet($icao);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AIRACApi->airacFirGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **icao** | **string**| FIR ICAO code. | [optional]

### Return type

[**\Swagger\Client\Model\FIR[]**](../Model/FIR.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **airacMoraGet**
> \Swagger\Client\Model\MORA[] airacMoraGet($lat, $lon)

Minimum Off Route Altitude

The MORA Endpoint provides information about Minimum Off Route Altitudes and is refreshed with every AIRAC cycle.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\AIRACApi();
$lat = "lat_example"; // string | Latitude (.25 degree accuracy - must be exact).
$lon = "lon_example"; // string | Longitude (.25 degree accuracy - must be exact).

try {
    $result = $api_instance->airacMoraGet($lat, $lon);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AIRACApi->airacMoraGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lat** | **string**| Latitude (.25 degree accuracy - must be exact). | [optional]
 **lon** | **string**| Longitude (.25 degree accuracy - must be exact). | [optional]

### Return type

[**\Swagger\Client\Model\MORA[]**](../Model/MORA.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

