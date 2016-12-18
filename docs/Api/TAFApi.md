# Swagger\Client\TAFApi

All URIs are relative to *http://v3.openaviationdata.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**weatherTafRadiusGet**](TAFApi.md#weatherTafRadiusGet) | **GET** /weather/taf/radius | TAF by Station in Radius from Centerpoint
[**weatherTafRectangleGet**](TAFApi.md#weatherTafRectangleGet) | **GET** /weather/taf/rectangle | TAF by Station in Rectangular Zone
[**weatherTafStationGet**](TAFApi.md#weatherTafStationGet) | **GET** /weather/taf/station | TAF by Station


# **weatherTafRadiusGet**
> \Swagger\Client\Model\TAF[] weatherTafRadiusGet($lat, $lon, $radius)

TAF by Station in Radius from Centerpoint

The TAF Endpoint provides the lastest TAF for any stations within the radius of a centerpoint and is available in real-time.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\TAFApi();
$lat = "lat_example"; // string | Latitude of centerpoint (Decimal Degrees)
$lon = "lon_example"; // string | Longitude of centerpoint (Decimal Degrees)
$radius = "radius_example"; // string | Radius to search within (Statute Miles)

try {
    $result = $api_instance->weatherTafRadiusGet($lat, $lon, $radius);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TAFApi->weatherTafRadiusGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lat** | **string**| Latitude of centerpoint (Decimal Degrees) |
 **lon** | **string**| Longitude of centerpoint (Decimal Degrees) |
 **radius** | **string**| Radius to search within (Statute Miles) |

### Return type

[**\Swagger\Client\Model\TAF[]**](../Model/TAF.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **weatherTafRectangleGet**
> \Swagger\Client\Model\TAF[] weatherTafRectangleGet($minlat, $maxlat, $minlon, $maxlon)

TAF by Station in Rectangular Zone

The TAF Endpoint provides the lastest TAF for any stations within the rectangular zone and is available in real-time.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\TAFApi();
$minlat = "minlat_example"; // string | Minimum latitude to make rectangular (Decimal Degrees)
$maxlat = "maxlat_example"; // string | Maxiumum latitude to make rectangular (Decimal Degrees)
$minlon = "minlon_example"; // string | Minimum longitude to make rectangular (Decimal Degrees)
$maxlon = "maxlon_example"; // string | Maxiumum longitude to make rectangular (Decimal Degrees)

try {
    $result = $api_instance->weatherTafRectangleGet($minlat, $maxlat, $minlon, $maxlon);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TAFApi->weatherTafRectangleGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **minlat** | **string**| Minimum latitude to make rectangular (Decimal Degrees) |
 **maxlat** | **string**| Maxiumum latitude to make rectangular (Decimal Degrees) |
 **minlon** | **string**| Minimum longitude to make rectangular (Decimal Degrees) |
 **maxlon** | **string**| Maxiumum longitude to make rectangular (Decimal Degrees) |

### Return type

[**\Swagger\Client\Model\TAF[]**](../Model/TAF.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **weatherTafStationGet**
> \Swagger\Client\Model\TAF[] weatherTafStationGet($icao)

TAF by Station

The TAF Endpoint provides the lastest TAF for a given station and is available in real-time.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\TAFApi();
$icao = "icao_example"; // string | Station Identifier (Weather Station or Airport)

try {
    $result = $api_instance->weatherTafStationGet($icao);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TAFApi->weatherTafStationGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **icao** | **string**| Station Identifier (Weather Station or Airport) |

### Return type

[**\Swagger\Client\Model\TAF[]**](../Model/TAF.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

