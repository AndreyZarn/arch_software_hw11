# ScheduleApi

All URIs are relative to *https://localhost:9669*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addSchedule**](ScheduleApi.md#addSchedule) | **POST** /Schedule | Добавление расписания
[**deleteSchedule**](ScheduleApi.md#deleteSchedule) | **DELETE** /Schedule/deleteById/{scheduleId} | Удаление расписания по ID
[**getScheduleById**](ScheduleApi.md#getScheduleById) | **GET** /Schedule/findById/{scheduleId} | Поиск расписания по ID
[**updateSchedule**](ScheduleApi.md#updateSchedule) | **PUT** /Schedule/updateById/{scheduleId} | Обновление расписания уборки

<a name="addSchedule"></a>
# **addSchedule**
> Schedule addSchedule(body)

Добавление расписания

Добавление расписания в базу данных

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.ScheduleApi;


ScheduleApi apiInstance = new ScheduleApi();
Schedule body = new Schedule(); // Schedule | Добавление расписания в базу данных
try {
    Schedule result = apiInstance.addSchedule(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ScheduleApi#addSchedule");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Schedule**](Schedule.md)| Добавление расписания в базу данных |

### Return type

[**Schedule**](Schedule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, application/xml, application/x-www-form-urlencoded
 - **Accept**: application/json, application/xml

<a name="addSchedule"></a>
# **addSchedule**
> Schedule addSchedule(id, dateTime, mode, robotId)

Добавление расписания

Добавление расписания в базу данных

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.ScheduleApi;


ScheduleApi apiInstance = new ScheduleApi();
Long id = 789L; // Long | 
String dateTime = "dateTime_example"; // String | 
Long mode = 789L; // Long | 
Long robotId = 789L; // Long | 
try {
    Schedule result = apiInstance.addSchedule(id, dateTime, mode, robotId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ScheduleApi#addSchedule");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Long**|  |
 **dateTime** | **String**|  |
 **mode** | **Long**|  |
 **robotId** | **Long**|  |

### Return type

[**Schedule**](Schedule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, application/xml, application/x-www-form-urlencoded
 - **Accept**: application/json, application/xml

<a name="deleteSchedule"></a>
# **deleteSchedule**
> deleteSchedule(scheduleId, scheduleId)

Удаление расписания по ID

Удаление расписания из базы данных

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.ScheduleApi;


ScheduleApi apiInstance = new ScheduleApi();
Long scheduleId = 789L; // Long | ID - идентификатор расписпания
String scheduleId = "scheduleId_example"; // String | 
try {
    apiInstance.deleteSchedule(scheduleId, scheduleId);
} catch (ApiException e) {
    System.err.println("Exception when calling ScheduleApi#deleteSchedule");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **scheduleId** | **Long**| ID - идентификатор расписпания |
 **scheduleId** | **String**|  | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="getScheduleById"></a>
# **getScheduleById**
> Schedule getScheduleById(scheduleId)

Поиск расписания по ID

Поиск расписания в базе данных

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.ScheduleApi;


ScheduleApi apiInstance = new ScheduleApi();
Long scheduleId = 789L; // Long | scheduleId - идентификатор пользователя
try {
    Schedule result = apiInstance.getScheduleById(scheduleId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ScheduleApi#getScheduleById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **scheduleId** | **Long**| scheduleId - идентификатор пользователя |

### Return type

[**Schedule**](Schedule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/xml

<a name="updateSchedule"></a>
# **updateSchedule**
> Schedule updateSchedule(scheduleId)

Обновление расписания уборки

Обновление расписания в базе данных

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.ScheduleApi;


ScheduleApi apiInstance = new ScheduleApi();
Long scheduleId = 789L; // Long | scheduleId - идентификатор пользователя
try {
    Schedule result = apiInstance.updateSchedule(scheduleId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ScheduleApi#updateSchedule");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **scheduleId** | **Long**| scheduleId - идентификатор пользователя |

### Return type

[**Schedule**](Schedule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/xml

