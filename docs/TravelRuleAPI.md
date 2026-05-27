# \TravelRuleAPI

All URIs are relative to *https://api.dev.cobo.com/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CancelSatoshiTestChallenge**](TravelRuleAPI.md#CancelSatoshiTestChallenge) | **Post** /travel_rule/satoshi_test/challenge/cancel | Cancel Satoshi Test challenge
[**CreateSatoshiTestChallenge**](TravelRuleAPI.md#CreateSatoshiTestChallenge) | **Post** /travel_rule/satoshi_test/challenge | Create Satoshi Test challenge
[**GetAddressVerification**](TravelRuleAPI.md#GetAddressVerification) | **Get** /travel_rule/address_verifications/{verification_id} | Get address verification
[**GetSatoshiTestChallenge**](TravelRuleAPI.md#GetSatoshiTestChallenge) | **Get** /travel_rule/satoshi_test/challenge/status | Get Satoshi Test challenge
[**GetSignatureChallenge**](TravelRuleAPI.md#GetSignatureChallenge) | **Get** /travel_rule/signature_challenge | Get self-custody signature challenge
[**GetTransactionLimitation**](TravelRuleAPI.md#GetTransactionLimitation) | **Get** /travel_rule/transaction/limitation | Retrieve transaction limitations
[**ListAddressVerifications**](TravelRuleAPI.md#ListAddressVerifications) | **Get** /travel_rule/address_verifications | List address verifications
[**ListSupportedCountries**](TravelRuleAPI.md#ListSupportedCountries) | **Get** /travel_rule/transaction/countries | List supported countries
[**SubmitDepositTravelRuleInfo**](TravelRuleAPI.md#SubmitDepositTravelRuleInfo) | **Post** /travel_rule/transaction/deposit/travel_rule_info | Submit Travel Rule information for deposits
[**SubmitWithdrawTravelRuleInfo**](TravelRuleAPI.md#SubmitWithdrawTravelRuleInfo) | **Post** /travel_rule/transaction/withdraw/travel_rule_info | Submit Travel Rule information for withdrawals



## CancelSatoshiTestChallenge

> SatoshiTestCancelResult CancelSatoshiTestChallenge(ctx).CancelSatoshiTestChallengeRequest(cancelSatoshiTestChallengeRequest).Execute()

Cancel Satoshi Test challenge



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    coboWaas2 "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2"
    "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2/crypto"
)

func main() {
	cancelSatoshiTestChallengeRequest := *coboWaas2.NewCancelSatoshiTestChallengeRequest("a1b2c3d4-e5f6-7890-abcd-ef1234567890")

	configuration := coboWaas2.NewConfiguration()
	// Initialize the API client
	apiClient := coboWaas2.NewAPIClient(configuration)
	ctx := context.Background()

    // Select the development environment. To use the production environment, replace coboWaas2.DevEnv with coboWaas2.ProdEnv
	ctx = context.WithValue(ctx, coboWaas2.ContextEnv, coboWaas2.DevEnv)
    // Replace `<YOUR_PRIVATE_KEY>` with your private key
	ctx = context.WithValue(ctx, coboWaas2.ContextPortalSigner, crypto.Ed25519Signer{
		Secret: "<YOUR_PRIVATE_KEY>",
	})
	resp, r, err := apiClient.TravelRuleAPI.CancelSatoshiTestChallenge(ctx).CancelSatoshiTestChallengeRequest(cancelSatoshiTestChallengeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TravelRuleAPI.CancelSatoshiTestChallenge``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelSatoshiTestChallenge`: SatoshiTestCancelResult
	fmt.Fprintf(os.Stdout, "Response from `TravelRuleAPI.CancelSatoshiTestChallenge`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCancelSatoshiTestChallengeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **cancelSatoshiTestChallengeRequest** | [**CancelSatoshiTestChallengeRequest**](CancelSatoshiTestChallengeRequest.md) |  | 

### Return type

[**SatoshiTestCancelResult**](SatoshiTestCancelResult.md)

### Authorization

[OAuth2](../README.md#OAuth2), [CoboAuth](../README.md#CoboAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateSatoshiTestChallenge

> SatoshiTestChallenge CreateSatoshiTestChallenge(ctx).CreateSatoshiTestChallengeRequest(createSatoshiTestChallengeRequest).Execute()

Create Satoshi Test challenge



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    coboWaas2 "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2"
    "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2/crypto"
)

func main() {
	createSatoshiTestChallengeRequest := *coboWaas2.NewCreateSatoshiTestChallengeRequest(coboWaas2.SatoshiTestChallengeAction("PREPARE"), "ETH", "0x1234567890abcdef1234567890abcdef12345678", "123e4567-e89b-12d3-a456-426614174000", coboWaas2.TravelRuleTransactionType("DEPOSIT"))

	configuration := coboWaas2.NewConfiguration()
	// Initialize the API client
	apiClient := coboWaas2.NewAPIClient(configuration)
	ctx := context.Background()

    // Select the development environment. To use the production environment, replace coboWaas2.DevEnv with coboWaas2.ProdEnv
	ctx = context.WithValue(ctx, coboWaas2.ContextEnv, coboWaas2.DevEnv)
    // Replace `<YOUR_PRIVATE_KEY>` with your private key
	ctx = context.WithValue(ctx, coboWaas2.ContextPortalSigner, crypto.Ed25519Signer{
		Secret: "<YOUR_PRIVATE_KEY>",
	})
	resp, r, err := apiClient.TravelRuleAPI.CreateSatoshiTestChallenge(ctx).CreateSatoshiTestChallengeRequest(createSatoshiTestChallengeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TravelRuleAPI.CreateSatoshiTestChallenge``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateSatoshiTestChallenge`: SatoshiTestChallenge
	fmt.Fprintf(os.Stdout, "Response from `TravelRuleAPI.CreateSatoshiTestChallenge`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateSatoshiTestChallengeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createSatoshiTestChallengeRequest** | [**CreateSatoshiTestChallengeRequest**](CreateSatoshiTestChallengeRequest.md) |  | 

### Return type

[**SatoshiTestChallenge**](SatoshiTestChallenge.md)

### Authorization

[OAuth2](../README.md#OAuth2), [CoboAuth](../README.md#CoboAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetAddressVerification

> AddressVerificationDetail GetAddressVerification(ctx, verificationId).Execute()

Get address verification



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    coboWaas2 "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2"
    "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2/crypto"
)

func main() {
	verificationId := "fb377ea5-a97a-49b4-955d-23f8fdd5177a"

	configuration := coboWaas2.NewConfiguration()
	// Initialize the API client
	apiClient := coboWaas2.NewAPIClient(configuration)
	ctx := context.Background()

    // Select the development environment. To use the production environment, replace coboWaas2.DevEnv with coboWaas2.ProdEnv
	ctx = context.WithValue(ctx, coboWaas2.ContextEnv, coboWaas2.DevEnv)
    // Replace `<YOUR_PRIVATE_KEY>` with your private key
	ctx = context.WithValue(ctx, coboWaas2.ContextPortalSigner, crypto.Ed25519Signer{
		Secret: "<YOUR_PRIVATE_KEY>",
	})
	resp, r, err := apiClient.TravelRuleAPI.GetAddressVerification(ctx, verificationId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TravelRuleAPI.GetAddressVerification``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAddressVerification`: AddressVerificationDetail
	fmt.Fprintf(os.Stdout, "Response from `TravelRuleAPI.GetAddressVerification`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for ServerHost/Env, Signer, etc.
**verificationId** | **string** | The unique identifier of the address verification record. | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAddressVerificationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**AddressVerificationDetail**](AddressVerificationDetail.md)

### Authorization

[OAuth2](../README.md#OAuth2), [CoboAuth](../README.md#CoboAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetSatoshiTestChallenge

> SatoshiTestChallenge GetSatoshiTestChallenge(ctx).ChallengeId(challengeId).Execute()

Get Satoshi Test challenge



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    coboWaas2 "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2"
    "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2/crypto"
)

func main() {
	challengeId := "a1b2c3d4-e5f6-7890-abcd-ef1234567890"

	configuration := coboWaas2.NewConfiguration()
	// Initialize the API client
	apiClient := coboWaas2.NewAPIClient(configuration)
	ctx := context.Background()

    // Select the development environment. To use the production environment, replace coboWaas2.DevEnv with coboWaas2.ProdEnv
	ctx = context.WithValue(ctx, coboWaas2.ContextEnv, coboWaas2.DevEnv)
    // Replace `<YOUR_PRIVATE_KEY>` with your private key
	ctx = context.WithValue(ctx, coboWaas2.ContextPortalSigner, crypto.Ed25519Signer{
		Secret: "<YOUR_PRIVATE_KEY>",
	})
	resp, r, err := apiClient.TravelRuleAPI.GetSatoshiTestChallenge(ctx).ChallengeId(challengeId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TravelRuleAPI.GetSatoshiTestChallenge``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetSatoshiTestChallenge`: SatoshiTestChallenge
	fmt.Fprintf(os.Stdout, "Response from `TravelRuleAPI.GetSatoshiTestChallenge`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetSatoshiTestChallengeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **challengeId** | **string** | The Satoshi Test challenge ID returned by the &#x60;prepare&#x60; or &#x60;submit&#x60; operation. | 

### Return type

[**SatoshiTestChallenge**](SatoshiTestChallenge.md)

### Authorization

[OAuth2](../README.md#OAuth2), [CoboAuth](../README.md#CoboAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetSignatureChallenge

> SignatureChallenge GetSignatureChallenge(ctx).TransactionType(transactionType).TransactionId(transactionId).Execute()

Get self-custody signature challenge



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    coboWaas2 "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2"
    "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2/crypto"
)

func main() {
	transactionType := "DEPOSIT"
	transactionId := "123e4567-e89b-12d3-a456-426614174000"

	configuration := coboWaas2.NewConfiguration()
	// Initialize the API client
	apiClient := coboWaas2.NewAPIClient(configuration)
	ctx := context.Background()

    // Select the development environment. To use the production environment, replace coboWaas2.DevEnv with coboWaas2.ProdEnv
	ctx = context.WithValue(ctx, coboWaas2.ContextEnv, coboWaas2.DevEnv)
    // Replace `<YOUR_PRIVATE_KEY>` with your private key
	ctx = context.WithValue(ctx, coboWaas2.ContextPortalSigner, crypto.Ed25519Signer{
		Secret: "<YOUR_PRIVATE_KEY>",
	})
	resp, r, err := apiClient.TravelRuleAPI.GetSignatureChallenge(ctx).TransactionType(transactionType).TransactionId(transactionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TravelRuleAPI.GetSignatureChallenge``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetSignatureChallenge`: SignatureChallenge
	fmt.Fprintf(os.Stdout, "Response from `TravelRuleAPI.GetSignatureChallenge`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetSignatureChallengeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **transactionType** | **string** | The transaction type. Possible values include:    - &#x60;DEPOSIT&#x60;: A deposit transaction.   - &#x60;WITHDRAW&#x60;: A withdrawal transaction.  | 
 **transactionId** | **string** | The transaction ID. | 

### Return type

[**SignatureChallenge**](SignatureChallenge.md)

### Authorization

[OAuth2](../README.md#OAuth2), [CoboAuth](../README.md#CoboAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTransactionLimitation

> GetTransactionLimitation200Response GetTransactionLimitation(ctx).TransactionType(transactionType).TransactionId(transactionId).Execute()

Retrieve transaction limitations



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    coboWaas2 "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2"
    "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2/crypto"
)

func main() {
	transactionType := "DEPOSIT"
	transactionId := "123e4567-e89b-12d3-a456-426614174000"

	configuration := coboWaas2.NewConfiguration()
	// Initialize the API client
	apiClient := coboWaas2.NewAPIClient(configuration)
	ctx := context.Background()

    // Select the development environment. To use the production environment, replace coboWaas2.DevEnv with coboWaas2.ProdEnv
	ctx = context.WithValue(ctx, coboWaas2.ContextEnv, coboWaas2.DevEnv)
    // Replace `<YOUR_PRIVATE_KEY>` with your private key
	ctx = context.WithValue(ctx, coboWaas2.ContextPortalSigner, crypto.Ed25519Signer{
		Secret: "<YOUR_PRIVATE_KEY>",
	})
	resp, r, err := apiClient.TravelRuleAPI.GetTransactionLimitation(ctx).TransactionType(transactionType).TransactionId(transactionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TravelRuleAPI.GetTransactionLimitation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTransactionLimitation`: GetTransactionLimitation200Response
	fmt.Fprintf(os.Stdout, "Response from `TravelRuleAPI.GetTransactionLimitation`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetTransactionLimitationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **transactionType** | **string** | The transaction type. Possible values include:    - &#x60;DEPOSIT&#x60;: A deposit transaction.   - &#x60;WITHDRAW&#x60;: A withdrawal transaction.  | 
 **transactionId** | **string** | The transaction ID. | 

### Return type

[**GetTransactionLimitation200Response**](GetTransactionLimitation200Response.md)

### Authorization

[OAuth2](../README.md#OAuth2), [CoboAuth](../README.md#CoboAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListAddressVerifications

> ListAddressVerifications200Response ListAddressVerifications(ctx).Status(status).ChainId(chainId).Address(address).Limit(limit).Before(before).After(after).Execute()

List address verifications



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    coboWaas2 "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2"
    "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2/crypto"
)

func main() {
	status := coboWaas2.AddressVerificationStatus("PENDING")
	chainId := "ETH"
	address := "0x1234567890abcdef1234567890abcdef12345678"
	limit := int32(10)
	before := "RqeEoTkgKG5rpzqYzg2Hd3szmPoj2cE7w5jWwShz3C1vyGmk1"
	after := "RqeEoTkgKG5rpzqYzg2Hd3szmPoj2cE7w5jWwShz3C1vyGSAk"

	configuration := coboWaas2.NewConfiguration()
	// Initialize the API client
	apiClient := coboWaas2.NewAPIClient(configuration)
	ctx := context.Background()

    // Select the development environment. To use the production environment, replace coboWaas2.DevEnv with coboWaas2.ProdEnv
	ctx = context.WithValue(ctx, coboWaas2.ContextEnv, coboWaas2.DevEnv)
    // Replace `<YOUR_PRIVATE_KEY>` with your private key
	ctx = context.WithValue(ctx, coboWaas2.ContextPortalSigner, crypto.Ed25519Signer{
		Secret: "<YOUR_PRIVATE_KEY>",
	})
	resp, r, err := apiClient.TravelRuleAPI.ListAddressVerifications(ctx).Status(status).ChainId(chainId).Address(address).Limit(limit).Before(before).After(after).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TravelRuleAPI.ListAddressVerifications``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAddressVerifications`: ListAddressVerifications200Response
	fmt.Fprintf(os.Stdout, "Response from `TravelRuleAPI.ListAddressVerifications`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListAddressVerificationsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | [**AddressVerificationStatus**](AddressVerificationStatus.md) | Filter by verification status. Allowed values: - &#x60;PENDING&#x60;: A Satoshi Test challenge is in progress (countdown active or awaiting confirmation). - &#x60;VERIFIED&#x60;: The address ownership has been confirmed (by signature or by a matched Satoshi Test transfer). - &#x60;FAILED&#x60;: The verification attempt did not succeed (Satoshi Test expired without match, or signature verification rejected).  Omit this parameter to return records of all three statuses.  | 
 **chainId** | **string** | Filter by chain ID (e.g. &#x60;BTC&#x60;, &#x60;ETH&#x60;, &#x60;BASE_ETH&#x60;, &#x60;BSC_BNB&#x60;, &#x60;TRON&#x60;). | 
 **address** | **string** | Filter by counterparty (self-custody) wallet address. | 
 **limit** | **int32** | The maximum number of objects to return. For most operations, the value range is [1, 50]. | [default to 10]
 **before** | **string** | A cursor indicating the position before the current page. This value is generated by Cobo and returned in the response. If you are paginating forward from the beginning, you do not need to provide it on the first request. When paginating backward (to the previous page), you should pass the before value returned from the last response.  | 
 **after** | **string** | A cursor indicating the position after the current page. This value is generated by Cobo and returned in the response. You do not need to provide it on the first request. When paginating forward (to the next page), you should pass the after value returned from the last response.  | 

### Return type

[**ListAddressVerifications200Response**](ListAddressVerifications200Response.md)

### Authorization

[OAuth2](../README.md#OAuth2), [CoboAuth](../README.md#CoboAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListSupportedCountries

> []ListSupportedCountries200ResponseInner ListSupportedCountries(ctx).Execute()

List supported countries



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    coboWaas2 "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2"
    "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2/crypto"
)

func main() {

	configuration := coboWaas2.NewConfiguration()
	// Initialize the API client
	apiClient := coboWaas2.NewAPIClient(configuration)
	ctx := context.Background()

    // Select the development environment. To use the production environment, replace coboWaas2.DevEnv with coboWaas2.ProdEnv
	ctx = context.WithValue(ctx, coboWaas2.ContextEnv, coboWaas2.DevEnv)
    // Replace `<YOUR_PRIVATE_KEY>` with your private key
	ctx = context.WithValue(ctx, coboWaas2.ContextPortalSigner, crypto.Ed25519Signer{
		Secret: "<YOUR_PRIVATE_KEY>",
	})
	resp, r, err := apiClient.TravelRuleAPI.ListSupportedCountries(ctx).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TravelRuleAPI.ListSupportedCountries``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListSupportedCountries`: []ListSupportedCountries200ResponseInner
	fmt.Fprintf(os.Stdout, "Response from `TravelRuleAPI.ListSupportedCountries`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListSupportedCountriesRequest struct via the builder pattern


### Return type

[**[]ListSupportedCountries200ResponseInner**](ListSupportedCountries200ResponseInner.md)

### Authorization

[OAuth2](../README.md#OAuth2), [CoboAuth](../README.md#CoboAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SubmitDepositTravelRuleInfo

> SubmitDepositTravelRuleInfo201Response SubmitDepositTravelRuleInfo(ctx).TravelRuleDepositRequest(travelRuleDepositRequest).Execute()

Submit Travel Rule information for deposits



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    coboWaas2 "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2"
    "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2/crypto"
)

func main() {
	travelRuleDepositRequest := *coboWaas2.NewTravelRuleDepositRequest("f47ac10b-58cc-4372-a567-0e02b2c3d479", coboWaas2.TravelRuleDepositRequest_travel_rule_info{SelfCustodyWallet: coboWaas2.NewSelfCustodyWallet(coboWaas2.DestinationWalletType("EXCHANGES_OR_VASP"), "challenge_token_abc123", "0x1234567890abcdef1234567890abcdef12345678", "0xf0a0ca69dd3afc57235c72aba3ff1f1144ee5409aeec013a9b17cdb58d0185a66a525945bfbd66e87bf0503eb0b83bf90cb973a8cbb730d19dc032e00dfe393a1c")})

	configuration := coboWaas2.NewConfiguration()
	// Initialize the API client
	apiClient := coboWaas2.NewAPIClient(configuration)
	ctx := context.Background()

    // Select the development environment. To use the production environment, replace coboWaas2.DevEnv with coboWaas2.ProdEnv
	ctx = context.WithValue(ctx, coboWaas2.ContextEnv, coboWaas2.DevEnv)
    // Replace `<YOUR_PRIVATE_KEY>` with your private key
	ctx = context.WithValue(ctx, coboWaas2.ContextPortalSigner, crypto.Ed25519Signer{
		Secret: "<YOUR_PRIVATE_KEY>",
	})
	resp, r, err := apiClient.TravelRuleAPI.SubmitDepositTravelRuleInfo(ctx).TravelRuleDepositRequest(travelRuleDepositRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TravelRuleAPI.SubmitDepositTravelRuleInfo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SubmitDepositTravelRuleInfo`: SubmitDepositTravelRuleInfo201Response
	fmt.Fprintf(os.Stdout, "Response from `TravelRuleAPI.SubmitDepositTravelRuleInfo`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSubmitDepositTravelRuleInfoRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **travelRuleDepositRequest** | [**TravelRuleDepositRequest**](TravelRuleDepositRequest.md) |  | 

### Return type

[**SubmitDepositTravelRuleInfo201Response**](SubmitDepositTravelRuleInfo201Response.md)

### Authorization

[OAuth2](../README.md#OAuth2), [CoboAuth](../README.md#CoboAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SubmitWithdrawTravelRuleInfo

> SubmitDepositTravelRuleInfo201Response SubmitWithdrawTravelRuleInfo(ctx).TravelRuleWithdrawRequest(travelRuleWithdrawRequest).Execute()

Submit Travel Rule information for withdrawals



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    coboWaas2 "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2"
    "github.com/CoboGlobal/cobo-waas2-go-sdk/cobo_waas2/crypto"
)

func main() {
	travelRuleWithdrawRequest := *coboWaas2.NewTravelRuleWithdrawRequest("f47ac10b-58cc-4372-a567-0e02b2c3d479", coboWaas2.TravelRuleWithdrawRequest_travel_rule_info{SelfCustodyWallet: coboWaas2.NewSelfCustodyWallet(coboWaas2.DestinationWalletType("EXCHANGES_OR_VASP"), "challenge_token_abc123", "0x1234567890abcdef1234567890abcdef12345678", "0xf0a0ca69dd3afc57235c72aba3ff1f1144ee5409aeec013a9b17cdb58d0185a66a525945bfbd66e87bf0503eb0b83bf90cb973a8cbb730d19dc032e00dfe393a1c")})

	configuration := coboWaas2.NewConfiguration()
	// Initialize the API client
	apiClient := coboWaas2.NewAPIClient(configuration)
	ctx := context.Background()

    // Select the development environment. To use the production environment, replace coboWaas2.DevEnv with coboWaas2.ProdEnv
	ctx = context.WithValue(ctx, coboWaas2.ContextEnv, coboWaas2.DevEnv)
    // Replace `<YOUR_PRIVATE_KEY>` with your private key
	ctx = context.WithValue(ctx, coboWaas2.ContextPortalSigner, crypto.Ed25519Signer{
		Secret: "<YOUR_PRIVATE_KEY>",
	})
	resp, r, err := apiClient.TravelRuleAPI.SubmitWithdrawTravelRuleInfo(ctx).TravelRuleWithdrawRequest(travelRuleWithdrawRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TravelRuleAPI.SubmitWithdrawTravelRuleInfo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SubmitWithdrawTravelRuleInfo`: SubmitDepositTravelRuleInfo201Response
	fmt.Fprintf(os.Stdout, "Response from `TravelRuleAPI.SubmitWithdrawTravelRuleInfo`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSubmitWithdrawTravelRuleInfoRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **travelRuleWithdrawRequest** | [**TravelRuleWithdrawRequest**](TravelRuleWithdrawRequest.md) |  | 

### Return type

[**SubmitDepositTravelRuleInfo201Response**](SubmitDepositTravelRuleInfo201Response.md)

### Authorization

[OAuth2](../README.md#OAuth2), [CoboAuth](../README.md#CoboAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

