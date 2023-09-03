# GroupApi

All URIs are relative to *https://localhost:9669*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addGroup**](GroupApi.md#addGroup) | **POST** /Group | Добавить группу
[**deleteGroup**](GroupApi.md#deleteGroup) | **DELETE** /Group/deleteById/{groupId} | Удаление группы по ID
[**getGroupById**](GroupApi.md#getGroupById) | **GET** /Group/findById/{groupId} | Поиск группы по ID
[**updateGroup**](GroupApi.md#updateGroup) | **PUT** /Group/updateById/{groupId} | Обновление группы пользователей

<a name="addGroup"></a>
# **addGroup**
> Group addGroup(body)

Добавить группу

Добавить группу в базу

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.GroupApi;


GroupApi apiInstance = new GroupApi();
Group body = new Group(); // Group | Создание новой группы в базе
try {
    Group result = apiInstance.addGroup(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GroupApi#addGroup");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Group**](Group.md)| Создание новой группы в базе |

### Return type

[**Group**](Group.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, application/xml, application/x-www-form-urlencoded
 - **Accept**: application/json, application/xml

<a name="addGroup"></a>
# **addGroup**
> Group addGroup(id, userId)

Добавить группу

Добавить группу в базу

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.GroupApi;


GroupApi apiInstance = new GroupApi();
Long id = 789L; // Long | 
Long userId = 789L; // Long | 
try {
    Group result = apiInstance.addGroup(id, userId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GroupApi#addGroup");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Long**|  |
 **userId** | **Long**|  |

### Return type

[**Group**](Group.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, application/xml, application/x-www-form-urlencoded
 - **Accept**: application/json, application/xml

<a name="deleteGroup"></a>
# **deleteGroup**
> deleteGroup(groupId, groupId)

Удаление группы по ID

Удаление группы в базе данных

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.GroupApi;


GroupApi apiInstance = new GroupApi();
Long groupId = 789L; // Long | ID - идентификатор группы
String groupId = "groupId_example"; // String | 
try {
    apiInstance.deleteGroup(groupId, groupId);
} catch (ApiException e) {
    System.err.println("Exception when calling GroupApi#deleteGroup");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **groupId** | **Long**| ID - идентификатор группы |
 **groupId** | **String**|  | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="getGroupById"></a>
# **getGroupById**
> Group getGroupById(groupId)

Поиск группы по ID

Поиск группы в базе данных

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.GroupApi;


GroupApi apiInstance = new GroupApi();
Long groupId = 789L; // Long | Поиск группы
try {
    Group result = apiInstance.getGroupById(groupId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GroupApi#getGroupById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **groupId** | **Long**| Поиск группы |

### Return type

[**Group**](Group.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/xml

<a name="updateGroup"></a>
# **updateGroup**
> Group updateGroup(groupId)

Обновление группы пользователей

Обновить группу пользователей

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.GroupApi;


GroupApi apiInstance = new GroupApi();
Long groupId = 789L; // Long | Поиск группы
try {
    Group result = apiInstance.updateGroup(groupId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GroupApi#updateGroup");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **groupId** | **Long**| Поиск группы |

### Return type

[**Group**](Group.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/xml

