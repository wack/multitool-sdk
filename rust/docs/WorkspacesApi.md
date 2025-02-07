# \WorkspacesApi

All URIs are relative to *http://localhost:8000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_workspace**](WorkspacesApi.md#create_workspace) | **POST** /api/v1/workspaces | 
[**list_workspaces**](WorkspacesApi.md#list_workspaces) | **GET** /api/v1/workspaces | 
[**read_workspace**](WorkspacesApi.md#read_workspace) | **GET** /api/v1/workspaces/{id} | 
[**update_workspace**](WorkspacesApi.md#update_workspace) | **PATCH** /api/v1/workspaces/{id} | 



## create_workspace

> models::CreateWorkspaceSuccess create_workspace(create_workspace_request)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_workspace_request** | [**CreateWorkspaceRequest**](CreateWorkspaceRequest.md) |  | [required] |

### Return type

[**models::CreateWorkspaceSuccess**](CreateWorkspaceSuccess.md)

### Authorization

[bearer_auth](../README.md#bearer_auth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## list_workspaces

> models::WorkspaceListSuccess list_workspaces()


### Parameters

This endpoint does not need any parameter.

### Return type

[**models::WorkspaceListSuccess**](WorkspaceListSuccess.md)

### Authorization

[bearer_auth](../README.md#bearer_auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## read_workspace

> models::WorkspaceDetails read_workspace(id)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** | The workspace's id | [required] |

### Return type

[**models::WorkspaceDetails**](WorkspaceDetails.md)

### Authorization

[bearer_auth](../README.md#bearer_auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_workspace

> models::WorkspaceDetails update_workspace(id, update_workspace_request)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **uuid::Uuid** | The workspace's id | [required] |
**update_workspace_request** | [**UpdateWorkspaceRequest**](UpdateWorkspaceRequest.md) |  | [required] |

### Return type

[**models::WorkspaceDetails**](WorkspaceDetails.md)

### Authorization

[bearer_auth](../README.md#bearer_auth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

