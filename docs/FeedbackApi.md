# IO.Swagger.Api.FeedbackApi

All URIs are relative to *http://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetFeedback**](FeedbackApi.md#getfeedback) | **GET** /feedback/get | 
[**SendFeedback**](FeedbackApi.md#sendfeedback) | **POST** /feedback | 

<a name="getfeedback"></a>
# **GetFeedback**
> Feedback GetFeedback ()



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class GetFeedbackExample
    {
        public void main()
        {

            var apiInstance = new FeedbackApi();

            try
            {
                Feedback result = apiInstance.GetFeedback();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling FeedbackApi.GetFeedback: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**Feedback**](Feedback.md)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="sendfeedback"></a>
# **SendFeedback**
> void SendFeedback (Feedback body)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class SendFeedbackExample
    {
        public void main()
        {

            var apiInstance = new FeedbackApi();
            var body = new Feedback(); // Feedback | 

            try
            {
                apiInstance.SendFeedback(body);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling FeedbackApi.SendFeedback: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Feedback**](Feedback.md)|  | 

### Return type

void (empty response body)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
