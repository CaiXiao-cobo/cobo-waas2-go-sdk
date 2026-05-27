# CreateSatoshiTestChallengeRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Action** | [**SatoshiTestChallengeAction**](SatoshiTestChallengeAction.md) |  | 
**ChainId** | **string** | The chain ID of the counterparty address. See the operation description for supported chains. | 
**FromAddress** | **string** | The counterparty (self-custody) wallet address that will transfer the micro-deposit. | 
**TransactionId** | **string** | The Cobo transaction ID that this Satoshi Test is verifying for. | 
**TransactionType** | [**TravelRuleTransactionType**](TravelRuleTransactionType.md) |  | 
**ChallengeId** | Pointer to **string** | The &#x60;challenge_id&#x60; returned by a previous &#x60;PREPARE&#x60; call. - When &#x60;action&#x3D;SUBMIT&#x60;: if provided, activates that specific challenge by id (recommended when you cached the id client-side after &#x60;PREPARE&#x60;). If omitted, the server activates the latest matching challenge identified by &#x60;(chain_id, from_address)&#x60;. - When &#x60;action&#x3D;PREPARE&#x60;: **must be omitted**. A new challenge is always generated; passing a &#x60;challenge_id&#x60; here will cause the request to be rejected.  | [optional] 

## Methods

### NewCreateSatoshiTestChallengeRequest

`func NewCreateSatoshiTestChallengeRequest(action SatoshiTestChallengeAction, chainId string, fromAddress string, transactionId string, transactionType TravelRuleTransactionType, ) *CreateSatoshiTestChallengeRequest`

NewCreateSatoshiTestChallengeRequest instantiates a new CreateSatoshiTestChallengeRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateSatoshiTestChallengeRequestWithDefaults

`func NewCreateSatoshiTestChallengeRequestWithDefaults() *CreateSatoshiTestChallengeRequest`

NewCreateSatoshiTestChallengeRequestWithDefaults instantiates a new CreateSatoshiTestChallengeRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAction

`func (o *CreateSatoshiTestChallengeRequest) GetAction() SatoshiTestChallengeAction`

GetAction returns the Action field if non-nil, zero value otherwise.

### GetActionOk

`func (o *CreateSatoshiTestChallengeRequest) GetActionOk() (*SatoshiTestChallengeAction, bool)`

GetActionOk returns a tuple with the Action field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAction

`func (o *CreateSatoshiTestChallengeRequest) SetAction(v SatoshiTestChallengeAction)`

SetAction sets Action field to given value.


### GetChainId

`func (o *CreateSatoshiTestChallengeRequest) GetChainId() string`

GetChainId returns the ChainId field if non-nil, zero value otherwise.

### GetChainIdOk

`func (o *CreateSatoshiTestChallengeRequest) GetChainIdOk() (*string, bool)`

GetChainIdOk returns a tuple with the ChainId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChainId

`func (o *CreateSatoshiTestChallengeRequest) SetChainId(v string)`

SetChainId sets ChainId field to given value.


### GetFromAddress

`func (o *CreateSatoshiTestChallengeRequest) GetFromAddress() string`

GetFromAddress returns the FromAddress field if non-nil, zero value otherwise.

### GetFromAddressOk

`func (o *CreateSatoshiTestChallengeRequest) GetFromAddressOk() (*string, bool)`

GetFromAddressOk returns a tuple with the FromAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromAddress

`func (o *CreateSatoshiTestChallengeRequest) SetFromAddress(v string)`

SetFromAddress sets FromAddress field to given value.


### GetTransactionId

`func (o *CreateSatoshiTestChallengeRequest) GetTransactionId() string`

GetTransactionId returns the TransactionId field if non-nil, zero value otherwise.

### GetTransactionIdOk

`func (o *CreateSatoshiTestChallengeRequest) GetTransactionIdOk() (*string, bool)`

GetTransactionIdOk returns a tuple with the TransactionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransactionId

`func (o *CreateSatoshiTestChallengeRequest) SetTransactionId(v string)`

SetTransactionId sets TransactionId field to given value.


### GetTransactionType

`func (o *CreateSatoshiTestChallengeRequest) GetTransactionType() TravelRuleTransactionType`

GetTransactionType returns the TransactionType field if non-nil, zero value otherwise.

### GetTransactionTypeOk

`func (o *CreateSatoshiTestChallengeRequest) GetTransactionTypeOk() (*TravelRuleTransactionType, bool)`

GetTransactionTypeOk returns a tuple with the TransactionType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransactionType

`func (o *CreateSatoshiTestChallengeRequest) SetTransactionType(v TravelRuleTransactionType)`

SetTransactionType sets TransactionType field to given value.


### GetChallengeId

`func (o *CreateSatoshiTestChallengeRequest) GetChallengeId() string`

GetChallengeId returns the ChallengeId field if non-nil, zero value otherwise.

### GetChallengeIdOk

`func (o *CreateSatoshiTestChallengeRequest) GetChallengeIdOk() (*string, bool)`

GetChallengeIdOk returns a tuple with the ChallengeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChallengeId

`func (o *CreateSatoshiTestChallengeRequest) SetChallengeId(v string)`

SetChallengeId sets ChallengeId field to given value.

### HasChallengeId

`func (o *CreateSatoshiTestChallengeRequest) HasChallengeId() bool`

HasChallengeId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


