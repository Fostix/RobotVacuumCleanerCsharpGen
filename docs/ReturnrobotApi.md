# IO.Swagger.Api.ReturnrobotApi

All URIs are relative to *http://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GoBase**](ReturnrobotApi.md#gobase) | **POST** /gobase | 

<a name="gobase"></a>
# **GoBase**
> void GoBase (int? robotId)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class GoBaseExample
    {
        public void main()
        {

            var apiInstance = new ReturnrobotApi();
            var robotId = 56;  // int? | 

            try
            {
                apiInstance.GoBase(robotId);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ReturnrobotApi.GoBase: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **robotId** | **int?**|  | 

### Return type

void (empty response body)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
