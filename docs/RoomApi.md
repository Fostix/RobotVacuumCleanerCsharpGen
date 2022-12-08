# IO.Swagger.Api.RoomApi

All URIs are relative to *http://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateRoom**](RoomApi.md#createroom) | **POST** /room | 
[**DeleteRoomById**](RoomApi.md#deleteroombyid) | **DELETE** /room/{roomId} | 
[**GetRoom**](RoomApi.md#getroom) | **GET** /room/All | 
[**GetRoomById**](RoomApi.md#getroombyid) | **GET** /room{roomId} | 
[**UpdateRoom**](RoomApi.md#updateroom) | **PUT** /room/{roomId} | 

<a name="createroom"></a>
# **CreateRoom**
> void CreateRoom (Room body)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CreateRoomExample
    {
        public void main()
        {

            var apiInstance = new RoomApi();
            var body = new Room(); // Room | 

            try
            {
                apiInstance.CreateRoom(body);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RoomApi.CreateRoom: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Room**](Room.md)|  | 

### Return type

void (empty response body)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="deleteroombyid"></a>
# **DeleteRoomById**
> void DeleteRoomById (string roomId)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class DeleteRoomByIdExample
    {
        public void main()
        {

            var apiInstance = new RoomApi();
            var roomId = roomId_example;  // string | 

            try
            {
                apiInstance.DeleteRoomById(roomId);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RoomApi.DeleteRoomById: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **roomId** | **string**|  | 

### Return type

void (empty response body)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="getroom"></a>
# **GetRoom**
> Room GetRoom ()



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class GetRoomExample
    {
        public void main()
        {

            var apiInstance = new RoomApi();

            try
            {
                Room result = apiInstance.GetRoom();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RoomApi.GetRoom: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**Room**](Room.md)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="getroombyid"></a>
# **GetRoomById**
> Room GetRoomById (int? roomId)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class GetRoomByIdExample
    {
        public void main()
        {

            var apiInstance = new RoomApi();
            var roomId = 56;  // int? | 

            try
            {
                Room result = apiInstance.GetRoomById(roomId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RoomApi.GetRoomById: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **roomId** | **int?**|  | 

### Return type

[**Room**](Room.md)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="updateroom"></a>
# **UpdateRoom**
> void UpdateRoom (Room body, string roomId)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class UpdateRoomExample
    {
        public void main()
        {

            var apiInstance = new RoomApi();
            var body = new Room(); // Room | 
            var roomId = roomId_example;  // string | 

            try
            {
                apiInstance.UpdateRoom(body, roomId);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RoomApi.UpdateRoom: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Room**](Room.md)|  | 
 **roomId** | **string**|  | 

### Return type

void (empty response body)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
