# METAR

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**station** | **string** | Station Identifier | [optional] 
**observation_time** | **string** | Datetime METAR Observed (ISO8601) | [optional] 
**coordinates** | **object** |  | [optional] 
**tmp** | **string** | Air Temperature (Celcius) | [optional] 
**dewpt** | **string** | Dewpoint Temperature (Celcius) | [optional] 
**wind** | [**\Swagger\Client\Model\METARWind**](METARWind.md) |  | [optional] 
**visibility** | **string** | Horizontal visibility (SM) | [optional] 
**altimeter** | **string** | Altimeter (inches of Hg) | [optional] 
**pressure** | **string** | Sea-level pressure (mb) | [optional] 
**wx_string** | **string** | WX String Descriptions | [optional] 
**sky_conditions** | [**\Swagger\Client\Model\SkyConditions[]**](SkyConditions.md) |  | [optional] 
**category** | **string** | Flight category of METAR (can be VFR, MVFR, IFR, LIFR) | [optional] 
**_3hr** | [**\Swagger\Client\Model\METAR3hr**](METAR3hr.md) |  | [optional] 
**_6hr** | [**\Swagger\Client\Model\METAR6hr**](METAR6hr.md) |  | [optional] 
**_24hr** | [**\Swagger\Client\Model\METAR24hr**](METAR24hr.md) |  | [optional] 
**precip_sincelast** | **int** | Liquid precipitation in inches since the last regular METAR | [optional] 
**precip_snow** | **int** | Snow depth on the ground (inches) | [optional] 
**type** | **string** | Metar Type (METAR or SPECI) | [optional] 
**elevation** | **string** | Reported Station Elevation (ft MSL) | [optional] 
**raw** | **string** | RAW Metar | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


