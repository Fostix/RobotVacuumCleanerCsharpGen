# IO.Swagger.Api.SendCleanTheRoomApi

All URIs are relative to *http://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**SendClean**](SendCleanTheRoomApi.md#sendclean) | **POST** /sendclean/launch | 

<a name="sendclean"></a>
# **SendClean**
> void SendClean (TaskForRobotOnlyLaunch body)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class SendCleanExample
    {
        public void main()
        {

            var apiInstance = new SendCleanTheRoomApi();
            var body = new TaskForRobotOnlyLaunch(); // TaskForRobotOnlyLaunch | 

            try
            {
                apiInstance.SendClean(body);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling SendCleanTheRoomApi.SendClean: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**TaskForRobotOnlyLaunch**](TaskForRobotOnlyLaunch.md)|  | 

### Return type

void (empty response body)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
