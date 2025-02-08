# MultiTool.WorkspacesApi

All URIs are relative to *http://localhost:8000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createWorkspace**](WorkspacesApi.md#createWorkspace) | **POST** /api/v1/workspaces | 
[**listWorkspaces**](WorkspacesApi.md#listWorkspaces) | **GET** /api/v1/workspaces | 
[**readWorkspace**](WorkspacesApi.md#readWorkspace) | **GET** /api/v1/workspaces/{id} | 
[**updateWorkspace**](WorkspacesApi.md#updateWorkspace) | **PATCH** /api/v1/workspaces/{id} | 



## createWorkspace

> CreateWorkspaceSuccess createWorkspace(createWorkspaceRequest)



### Example

```javascript
import MultiTool from 'multi_tool';
let defaultClient = MultiTool.ApiClient.instance;
// Configure Bearer access token for authorization: bearer_auth
let bearer_auth = defaultClient.authentications['bearer_auth'];
bearer_auth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MultiTool.WorkspacesApi();
let createWorkspaceRequest = new MultiTool.CreateWorkspaceRequest(); // CreateWorkspaceRequest | 
apiInstance.createWorkspace(createWorkspaceRequest).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createWorkspaceRequest** | [**CreateWorkspaceRequest**](CreateWorkspaceRequest.md)|  | 

### Return type

[**CreateWorkspaceSuccess**](CreateWorkspaceSuccess.md)

### Authorization

[bearer_auth](../README.md#bearer_auth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## listWorkspaces

> ListWorkspaceSuccess listWorkspaces(opts)



### Example

```javascript
import MultiTool from 'multi_tool';
let defaultClient = MultiTool.ApiClient.instance;
// Configure Bearer access token for authorization: bearer_auth
let bearer_auth = defaultClient.authentications['bearer_auth'];
bearer_auth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MultiTool.WorkspacesApi();
let opts = {
  'displayName': "displayName_example" // String | Only return workspaces with this name.
};
apiInstance.listWorkspaces(opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **displayName** | **String**| Only return workspaces with this name. | [optional] 

### Return type

[**ListWorkspaceSuccess**](ListWorkspaceSuccess.md)

### Authorization

[bearer_auth](../README.md#bearer_auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## readWorkspace

> WorkspaceDetails readWorkspace(id)



### Example

```javascript
import MultiTool from 'multi_tool';
let defaultClient = MultiTool.ApiClient.instance;
// Configure Bearer access token for authorization: bearer_auth
let bearer_auth = defaultClient.authentications['bearer_auth'];
bearer_auth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MultiTool.WorkspacesApi();
let id = "id_example"; // String | The workspace's id
apiInstance.readWorkspace(id).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| The workspace&#39;s id | 

### Return type

[**WorkspaceDetails**](WorkspaceDetails.md)

### Authorization

[bearer_auth](../README.md#bearer_auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateWorkspace

> WorkspaceDetails updateWorkspace(updateWorkspaceRequest, id)



### Example

```javascript
import MultiTool from 'multi_tool';
let defaultClient = MultiTool.ApiClient.instance;
// Configure Bearer access token for authorization: bearer_auth
let bearer_auth = defaultClient.authentications['bearer_auth'];
bearer_auth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new MultiTool.WorkspacesApi();
let updateWorkspaceRequest = new MultiTool.UpdateWorkspaceRequest(); // UpdateWorkspaceRequest | 
let id = "id_example"; // String | The workspace's id
apiInstance.updateWorkspace(updateWorkspaceRequest, id).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **updateWorkspaceRequest** | [**UpdateWorkspaceRequest**](UpdateWorkspaceRequest.md)|  | 
 **id** | **String**| The workspace&#39;s id | 

### Return type

[**WorkspaceDetails**](WorkspaceDetails.md)

### Authorization

[bearer_auth](../README.md#bearer_auth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

