# \DefaultApi

All URIs are relative to */api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetDailyHoroscopeApi**](DefaultApi.md#GetDailyHoroscopeApi) | **Get** /get-horoscope/daily | 
[**GetMonthlyHoroscopeApi**](DefaultApi.md#GetMonthlyHoroscopeApi) | **Get** /get-horoscope/monthly | 
[**GetWeeklyHoroscopeApi**](DefaultApi.md#GetWeeklyHoroscopeApi) | **Get** /get-horoscope/weekly | 



## GetDailyHoroscopeApi

> GetDailyHoroscopeApi(ctx).Sign(sign).Day(day).Execute()



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	sign := "sign_example" // string | 
	day := "day_example" // string | Accepted values: Date in format (YYYY-MM-DD) OR \"TODAY\" OR \"TOMORROW\" OR \"YESTERDAY\". (optional) (default to "TODAY")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.DefaultApi.GetDailyHoroscopeApi(context.Background()).Sign(sign).Day(day).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultApi.GetDailyHoroscopeApi``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetDailyHoroscopeApiRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sign** | **string** |  | 
 **day** | **string** | Accepted values: Date in format (YYYY-MM-DD) OR \&quot;TODAY\&quot; OR \&quot;TOMORROW\&quot; OR \&quot;YESTERDAY\&quot;. | [default to &quot;TODAY&quot;]

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetMonthlyHoroscopeApi

> GetMonthlyHoroscopeApi(ctx).Sign(sign).Execute()



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	sign := "sign_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.DefaultApi.GetMonthlyHoroscopeApi(context.Background()).Sign(sign).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultApi.GetMonthlyHoroscopeApi``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetMonthlyHoroscopeApiRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sign** | **string** |  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetWeeklyHoroscopeApi

> GetWeeklyHoroscopeApi(ctx).Sign(sign).Execute()



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	sign := "sign_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.DefaultApi.GetWeeklyHoroscopeApi(context.Background()).Sign(sign).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultApi.GetWeeklyHoroscopeApi``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetWeeklyHoroscopeApiRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sign** | **string** |  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

