# Swagger\Client\ROUTINGApi

All URIs are relative to *http://v3.openaviationdata.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**routingOceanicGet**](ROUTINGApi.md#routingOceanicGet) | **GET** /routing/oceanic | Oceanic Tracks


# **routingOceanicGet**
> \Swagger\Client\Model\OceanicTracks[] routingOceanicGet($subset)

Oceanic Tracks

The Oceanic Track Endpoint provides information about current, upcoming, and recently expired oceanic tracks and is available in real-time.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\ROUTINGApi();
$subset = "subset_example"; // string | Filter to specific subset (can be 'ausot', 'pacot', 'nat') - Defaults to all

try {
    $result = $api_instance->routingOceanicGet($subset);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ROUTINGApi->routingOceanicGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subset** | **string**| Filter to specific subset (can be &#39;ausot&#39;, &#39;pacot&#39;, &#39;nat&#39;) - Defaults to all | [optional]

### Return type

[**\Swagger\Client\Model\OceanicTracks[]**](../Model/OceanicTracks.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

