# TAFForecasts

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**valid** | **object** |  | [optional] 
**indicator** | **string** | Forecast change indicator (can be TEMPO, BECMG, FM, PROB) | [optional] 
**becoming** | **string** | Datetime becoming (ISO8601) | [optional] 
**probability** | **int** | Probability in becoming (Percentage) | [optional] 
**wind** | [**\Swagger\Client\Model\TAFForecastsWind**](TAFForecastsWind.md) |  | [optional] 
**visibility** | **string** | Horizontal visibility (SM) | [optional] 
**altimeter** | **string** | Altimeter (inches of Hg) | [optional] 
**wx_string** | **string** | WX String Descriptions | [optional] 
**no_decoded** | **string** | Indicates what is not decoded | [optional] 
**sky** | [**\Swagger\Client\Model\SkyConditions[]**](SkyConditions.md) |  | [optional] 
**turbulence** | [**\Swagger\Client\Model\Turbulence[]**](Turbulence.md) |  | [optional] 
**icing** | [**\Swagger\Client\Model\Icing[]**](Icing.md) |  | [optional] 
**tmp** | [**\Swagger\Client\Model\TAFForecastsTmp**](TAFForecastsTmp.md) |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


