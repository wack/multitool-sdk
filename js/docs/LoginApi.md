# MultiTool.LoginApi

All URIs are relative to *http://localhost:8000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**login**](LoginApi.md#login) | **POST** /api/v1/users/login | 



## login

> LoginSuccess login(loginRequest)



### Example

```javascript
import MultiTool from 'multi_tool';

let apiInstance = new MultiTool.LoginApi();
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

