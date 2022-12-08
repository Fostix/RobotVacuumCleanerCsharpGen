# IO.Swagger.Api.UserApi

All URIs are relative to *http://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddNewUser**](UserApi.md#addnewuser) | **POST** /registration | create user
[**GetUser**](UserApi.md#getuser) | **GET** /getUser | 
[**UpdateUser**](UserApi.md#updateuser) | **PUT** /updateUser | 

<a name="addnewuser"></a>
# **AddNewUser**
> void AddNewUser (User body)

create user

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class AddNewUserExample
    {
        public void main()
        {

            var apiInstance = new UserApi();
            var body = new User(); // User | 

            try
            {
                // create user
                apiInstance.AddNewUser(body);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling UserApi.AddNewUser: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**User**](User.md)|  | 

### Return type

void (empty response body)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="getuser"></a>
# **GetUser**
> User GetUser ()



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class GetUserExample
    {
        public void main()
        {

            var apiInstance = new UserApi();

            try
            {
                User result = apiInstance.GetUser();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling UserApi.GetUser: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**User**](User.md)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="updateuser"></a>
# **UpdateUser**
> void UpdateUser (User body)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class UpdateUserExample
    {
        public void main()
        {

            var apiInstance = new UserApi();
            var body = new User(); // User | 

            try
            {
                apiInstance.UpdateUser(body);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling UserApi.UpdateUser: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**User**](User.md)|  | 

### Return type

void (empty response body)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
