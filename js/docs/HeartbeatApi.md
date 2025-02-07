# MultiTool.HeartbeatApi

All URIs are relative to *http://localhost:8000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**heartbeatController**](HeartbeatApi.md#heartbeatController) | **GET** /api/v1/heartbeat | 



## heartbeatController

> HeartbeatController200Response heartbeatController()



### Example

```javascript
import MultiTool from 'multi_tool';

let apiInstance = new MultiTool.HeartbeatApi();
apiInstance.heartbeatController().then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters

This endpoint does not need any parameter.

### Return type

[**HeartbeatController200Response**](HeartbeatController200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

