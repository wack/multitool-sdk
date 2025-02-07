# MultiTool.ApplicationsApi

All URIs are relative to *http://localhost:8000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createApplication**](ApplicationsApi.md#createApplication) | **POST** /api/v1/workspaces/{workspace_id}/applications | 
[**getApplication**](ApplicationsApi.md#getApplication) | **GET** /api/v1/workspaces/{workspace_id}/applications/{application_id} | 
[**listApplications**](ApplicationsApi.md#listApplications) | **GET** /api/v1/workspaces/{workspace_id}/applications | 



## createApplication

> CreateApplicationSuccess createApplication(createApplicationRequest, workspaceId)



### Example

```javascript
import MultiTool from 'multi_tool';
let defaultClient = MultiTool.ApiClient.instance;
// Configure Bearer access token for authorization: bearer_auth
let bearer_auth = defaultClient.authentications['bearer_auth'];
bearer_auth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MultiTool.ApplicationsApi();
let createApplicationRequest = new MultiTool.CreateApplicationRequest(); // CreateApplicationRequest | 
let workspaceId = "workspaceId_example"; // String | The workspace's id
apiInstance.createApplication(createApplicationRequest, workspaceId).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createApplicationRequest** | [**CreateApplicationRequest**](CreateApplicationRequest.md)|  | 
 **workspaceId** | **String**| The workspace&#39;s id | 

### Return type

[**CreateApplicationSuccess**](CreateApplicationSuccess.md)

### Authorization

[bearer_auth](../README.md#bearer_auth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## getApplication

> ApplicationDetails getApplication(workspaceId, applicationId)



### Example

```javascript
import MultiTool from 'multi_tool';
let defaultClient = MultiTool.ApiClient.instance;
// Configure Bearer access token for authorization: bearer_auth
let bearer_auth = defaultClient.authentications['bearer_auth'];
bearer_auth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MultiTool.ApplicationsApi();
let workspaceId = "workspaceId_example"; // String | The workspace's id
let applicationId = "applicationId_example"; // String | The application's id
apiInstance.getApplication(workspaceId, applicationId).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspaceId** | **String**| The workspace&#39;s id | 
 **applicationId** | **String**| The application&#39;s id | 

### Return type

[**ApplicationDetails**](ApplicationDetails.md)

### Authorization

[bearer_auth](../README.md#bearer_auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listApplications

> ListApplicationsSuccess listApplications(workspaceId)



### Example

```javascript
import MultiTool from 'multi_tool';
let defaultClient = MultiTool.ApiClient.instance;
// Configure Bearer access token for authorization: bearer_auth
let bearer_auth = defaultClient.authentications['bearer_auth'];
bearer_auth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MultiTool.ApplicationsApi();
let workspaceId = "workspaceId_example"; // String | The workspace's id
apiInstance.listApplications(workspaceId).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workspaceId** | **String**| The workspace&#39;s id | 

### Return type

[**ListApplicationsSuccess**](ListApplicationsSuccess.md)

### Authorization

[bearer_auth](../README.md#bearer_auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

