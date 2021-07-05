# Swagger\Client\FilesApi

All URIs are relative to *https://bws.baokim.vn/cdn*

Method | HTTP request | Description
------------- | ------------- | -------------
[**filesUpload**](FilesApi.md#filesupload) | **POST** /files/upload | Upload files to public/protected folder

# **filesUpload**
> \Swagger\Client\Model\InlineResponse200 filesUpload($folder, $access_mode, $files)

Upload files to public/protected folder

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\FilesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$folder = "folder_example"; // string | 
$access_mode = "access_mode_example"; // string | 
$files = "/path/to/file"; // \SplFileObject | 

try {
    $result = $apiInstance->filesUpload($folder, $access_mode, $files);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling FilesApi->filesUpload: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **folder** | **string**|  | [optional]
 **access_mode** | **string**|  | [optional]
 **files** | [**\SplFileObject**](../Model/.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse200**](../Model/InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

