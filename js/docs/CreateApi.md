# MultiTool.CreateApi

All URIs are relative to *http://localhost:8000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create**](CreateApi.md#create) | **POST** /api/v1/users | 



## create

> CreateUserSuccess create(createUserRequest)



### Example

```javascript
import MultiTool from 'multi_tool';

let apiInstance = new MultiTool.CreateApi();
let createUserRequest = new MultiTool.CreateUserRequest(); // CreateUserRequest | 
apiInstance.create(createUserRequest).then((data) => {
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

