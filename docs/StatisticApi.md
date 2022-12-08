# IO.Swagger.Api.StatisticApi

All URIs are relative to *http://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetStatistic**](StatisticApi.md#getstatistic) | **GET** /statistic | 

<a name="getstatistic"></a>
# **GetStatistic**
> StatisticWork GetStatistic ()



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class GetStatisticExample
    {
        public void main()
        {

            var apiInstance = new StatisticApi();

            try
            {
                StatisticWork result = apiInstance.GetStatistic();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling StatisticApi.GetStatistic: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**StatisticWork**](StatisticWork.md)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
