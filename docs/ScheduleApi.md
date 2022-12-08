# IO.Swagger.Api.ScheduleApi

All URIs are relative to *http://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateTaskInSchedule**](ScheduleApi.md#createtaskinschedule) | **POST** /schedule/create | create schedule for robot
[**CreateTaskInSchedule1**](ScheduleApi.md#createtaskinschedule1) | **DELETE** /schedule/{taskId} | delete task in schedule
[**GetScheduleAllRobots**](ScheduleApi.md#getscheduleallrobots) | **GET** /schedule/All | 
[**GetScheduleByIdRobots**](ScheduleApi.md#getschedulebyidrobots) | **GET** /schedule/{IdRobots} | 
[**UpdateTaskInSchedule**](ScheduleApi.md#updatetaskinschedule) | **PUT** /schedule/{scheduleId} | 

<a name="createtaskinschedule"></a>
# **CreateTaskInSchedule**
> void CreateTaskInSchedule (TaskForRobot body)

create schedule for robot

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CreateTaskInScheduleExample
    {
        public void main()
        {

            var apiInstance = new ScheduleApi();
            var body = new TaskForRobot(); // TaskForRobot | 

            try
            {
                // create schedule for robot
                apiInstance.CreateTaskInSchedule(body);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ScheduleApi.CreateTaskInSchedule: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**TaskForRobot**](TaskForRobot.md)|  | 

### Return type

void (empty response body)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="createtaskinschedule1"></a>
# **CreateTaskInSchedule1**
> void CreateTaskInSchedule1 (string taskId, TaskForRobot body = null)

delete task in schedule

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CreateTaskInSchedule1Example
    {
        public void main()
        {

            var apiInstance = new ScheduleApi();
            var taskId = taskId_example;  // string | 
            var body = new TaskForRobot(); // TaskForRobot |  (optional) 

            try
            {
                // delete task in schedule
                apiInstance.CreateTaskInSchedule1(taskId, body);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ScheduleApi.CreateTaskInSchedule1: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **taskId** | **string**|  | 
 **body** | [**TaskForRobot**](TaskForRobot.md)|  | [optional] 

### Return type

void (empty response body)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="getscheduleallrobots"></a>
# **GetScheduleAllRobots**
> TaskForRobot GetScheduleAllRobots ()



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class GetScheduleAllRobotsExample
    {
        public void main()
        {

            var apiInstance = new ScheduleApi();

            try
            {
                TaskForRobot result = apiInstance.GetScheduleAllRobots();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ScheduleApi.GetScheduleAllRobots: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**TaskForRobot**](TaskForRobot.md)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="getschedulebyidrobots"></a>
# **GetScheduleByIdRobots**
> TaskForRobot GetScheduleByIdRobots (int? idRobot)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class GetScheduleByIdRobotsExample
    {
        public void main()
        {

            var apiInstance = new ScheduleApi();
            var idRobot = 56;  // int? | 

            try
            {
                TaskForRobot result = apiInstance.GetScheduleByIdRobots(idRobot);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ScheduleApi.GetScheduleByIdRobots: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **idRobot** | **int?**|  | 

### Return type

[**TaskForRobot**](TaskForRobot.md)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="updatetaskinschedule"></a>
# **UpdateTaskInSchedule**
> void UpdateTaskInSchedule (TaskForRobot body, string scheduleId)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class UpdateTaskInScheduleExample
    {
        public void main()
        {

            var apiInstance = new ScheduleApi();
            var body = new TaskForRobot(); // TaskForRobot | 
            var scheduleId = scheduleId_example;  // string | 

            try
            {
                apiInstance.UpdateTaskInSchedule(body, scheduleId);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ScheduleApi.UpdateTaskInSchedule: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**TaskForRobot**](TaskForRobot.md)|  | 
 **scheduleId** | **string**|  | 

### Return type

void (empty response body)

### Authorization

[BearerJWT](../README.md#BearerJWT)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
