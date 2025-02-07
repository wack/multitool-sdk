# MultiTool.UsersApi

All URIs are relative to *http://localhost:8000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createUser**](UsersApi.md#createUser) | **POST** /api/v1/users | 
[**login**](UsersApi.md#login) | **POST** /api/v1/users/login | 



## createUser

> CreateUserSuccess createUser(createUserRequest)



### Example

```javascript
import MultiTool from 'multi_tool';

let apiInstance = new MultiTool.UsersApi();
let createUserRequest = new MultiTool.CreateUserRequest(); // CreateUserRequest | 
apiInstance.createUser(createUserRequest).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createUserRequest** | [**CreateUserRequest**](CreateUserRequest.md)|  | 

### Return type

[**CreateUserSuccess**](CreateUserSuccess.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## login

> LoginSuccess login(loginRequest)



### Example

```javascript
import MultiTool from 'multi_tool';

let apiInstance = new MultiTool.UsersApi();
let loginRequest = new MultiTool.LoginRequest(); // LoginRequest | 
apiInstance.login(loginRequest).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **loginRequest** | [**LoginRequest**](LoginRequest.md)|  | 

### Return type

[**LoginSuccess**](LoginSuccess.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

