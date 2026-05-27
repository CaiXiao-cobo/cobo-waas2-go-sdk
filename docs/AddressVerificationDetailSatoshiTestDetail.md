# AddressVerificationDetailSatoshiTestDetail

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ChallengeId** | **string** | The unique identifier of the Satoshi Test challenge. | 
**FromAddress** | **string** | The counterparty (self-custody) wallet address that must transfer the micro-deposit. | 
**ToAddress** | **string** | The Cobo-generated verification address that will receive the micro-deposit. | 
**Amount** | **string** | The exact amount (in the token&#39;s smallest unit) that must be transferred. The amount is unique per challenge and is used together with &#x60;to_address&#x60; to identify a matching on-chain transfer.  | 
**TokenId** | **string** | The ID of the token used for the micro-deposit (typically the chain&#39;s native asset). | 
**ChainId** | **string** | The chain on which the micro-deposit is expected. | 
**Status** | [**SatoshiTestChallengeStatus**](SatoshiTestChallengeStatus.md) |  | 
**RemainingSeconds** | **int32** | Remaining time (in seconds) before the challenge expires. &#x60;0&#x60; when the challenge is not yet submitted or has already completed/expired.  | 
**MatchedTxid** | Pointer to **NullableString** | The on-chain transaction hash of the matching transfer, once matched. | [optional] 
**StartedAt** | Pointer to **NullableInt64** | Timestamp (milliseconds) when the challenge was submitted and the countdown started. | [optional] 
**ExpiresAt** | Pointer to **NullableInt64** | Timestamp (milliseconds) when the challenge will expire if not matched. | [optional] 

## Methods

### NewAddressVerificationDetailSatoshiTestDetail

`func NewAddressVerificationDetailSatoshiTestDetail(challengeId string, fromAddress string, toAddress string, amount string, tokenId string, chainId string, status SatoshiTestChallengeStatus, remainingSeconds int32, ) *AddressVerificationDetailSatoshiTestDetail`

NewAddressVerificationDetailSatoshiTestDetail instantiates a new AddressVerificationDetailSatoshiTestDetail object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAddressVerificationDetailSatoshiTestDetailWithDefaults

`func NewAddressVerificationDetailSatoshiTestDetailWithDefaults() *AddressVerificationDetailSatoshiTestDetail`

NewAddressVerificationDetailSatoshiTestDetailWithDefaults instantiates a new AddressVerificationDetailSatoshiTestDetail object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetChallengeId

`func (o *AddressVerificationDetailSatoshiTestDetail) GetChallengeId() string`

GetChallengeId returns the ChallengeId field if non-nil, zero value otherwise.

### GetChallengeIdOk

`func (o *AddressVerificationDetailSatoshiTestDetail) GetChallengeIdOk() (*string, bool)`

GetChallengeIdOk returns a tuple with the ChallengeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChallengeId

`func (o *AddressVerificationDetailSatoshiTestDetail) SetChallengeId(v string)`

SetChallengeId sets ChallengeId field to given value.


### GetFromAddress

`func (o *AddressVerificationDetailSatoshiTestDetail) GetFromAddress() string`

GetFromAddress returns the FromAddress field if non-nil, zero value otherwise.

### GetFromAddressOk

`func (o *AddressVerificationDetailSatoshiTestDetail) GetFromAddressOk() (*string, bool)`

GetFromAddressOk returns a tuple with the FromAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromAddress

`func (o *AddressVerificationDetailSatoshiTestDetail) SetFromAddress(v string)`

SetFromAddress sets FromAddress field to given value.


### GetToAddress

`func (o *AddressVerificationDetailSatoshiTestDetail) GetToAddress() string`

GetToAddress returns the ToAddress field if non-nil, zero value otherwise.

### GetToAddressOk

`func (o *AddressVerificationDetailSatoshiTestDetail) GetToAddressOk() (*string, bool)`

GetToAddressOk returns a tuple with the ToAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToAddress

`func (o *AddressVerificationDetailSatoshiTestDetail) SetToAddress(v string)`

SetToAddress sets ToAddress field to given value.


### GetAmount

`func (o *AddressVerificationDetailSatoshiTestDetail) GetAmount() string`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *AddressVerificationDetailSatoshiTestDetail) GetAmountOk() (*string, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *AddressVerificationDetailSatoshiTestDetail) SetAmount(v string)`

SetAmount sets Amount field to given value.


### GetTokenId

`func (o *AddressVerificationDetailSatoshiTestDetail) GetTokenId() string`

GetTokenId returns the TokenId field if non-nil, zero value otherwise.

### GetTokenIdOk

`func (o *AddressVerificationDetailSatoshiTestDetail) GetTokenIdOk() (*string, bool)`

GetTokenIdOk returns a tuple with the TokenId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokenId

`func (o *AddressVerificationDetailSatoshiTestDetail) SetTokenId(v string)`

SetTokenId sets TokenId field to given value.


### GetChainId

`func (o *AddressVerificationDetailSatoshiTestDetail) GetChainId() string`

GetChainId returns the ChainId field if non-nil, zero value otherwise.

### GetChainIdOk

`func (o *AddressVerificationDetailSatoshiTestDetail) GetChainIdOk() (*string, bool)`

GetChainIdOk returns a tuple with the ChainId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChainId

`func (o *AddressVerificationDetailSatoshiTestDetail) SetChainId(v string)`

SetChainId sets ChainId field to given value.


### GetStatus

`func (o *AddressVerificationDetailSatoshiTestDetail) GetStatus() SatoshiTestChallengeStatus`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *AddressVerificationDetailSatoshiTestDetail) GetStatusOk() (*SatoshiTestChallengeStatus, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *AddressVerificationDetailSatoshiTestDetail) SetStatus(v SatoshiTestChallengeStatus)`

SetStatus sets Status field to given value.


### GetRemainingSeconds

`func (o *AddressVerificationDetailSatoshiTestDetail) GetRemainingSeconds() int32`

GetRemainingSeconds returns the RemainingSeconds field if non-nil, zero value otherwise.

### GetRemainingSecondsOk

`func (o *AddressVerificationDetailSatoshiTestDetail) GetRemainingSecondsOk() (*int32, bool)`

GetRemainingSecondsOk returns a tuple with the RemainingSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemainingSeconds

`func (o *AddressVerificationDetailSatoshiTestDetail) SetRemainingSeconds(v int32)`

SetRemainingSeconds sets RemainingSeconds field to given value.


### GetMatchedTxid

`func (o *AddressVerificationDetailSatoshiTestDetail) GetMatchedTxid() string`

GetMatchedTxid returns the MatchedTxid field if non-nil, zero value otherwise.

### GetMatchedTxidOk

`func (o *AddressVerificationDetailSatoshiTestDetail) GetMatchedTxidOk() (*string, bool)`

GetMatchedTxidOk returns a tuple with the MatchedTxid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatchedTxid

`func (o *AddressVerificationDetailSatoshiTestDetail) SetMatchedTxid(v string)`

SetMatchedTxid sets MatchedTxid field to given value.

### HasMatchedTxid

`func (o *AddressVerificationDetailSatoshiTestDetail) HasMatchedTxid() bool`

HasMatchedTxid returns a boolean if a field has been set.

### SetMatchedTxidNil

`func (o *AddressVerificationDetailSatoshiTestDetail) SetMatchedTxidNil(b bool)`

 SetMatchedTxidNil sets the value for MatchedTxid to be an explicit nil

### UnsetMatchedTxid
`func (o *AddressVerificationDetailSatoshiTestDetail) UnsetMatchedTxid()`

UnsetMatchedTxid ensures that no value is present for MatchedTxid, not even an explicit nil
### GetStartedAt

`func (o *AddressVerificationDetailSatoshiTestDetail) GetStartedAt() int64`

GetStartedAt returns the StartedAt field if non-nil, zero value otherwise.

### GetStartedAtOk

`func (o *AddressVerificationDetailSatoshiTestDetail) GetStartedAtOk() (*int64, bool)`

GetStartedAtOk returns a tuple with the StartedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartedAt

`func (o *AddressVerificationDetailSatoshiTestDetail) SetStartedAt(v int64)`

SetStartedAt sets StartedAt field to given value.

### HasStartedAt

`func (o *AddressVerificationDetailSatoshiTestDetail) HasStartedAt() bool`

HasStartedAt returns a boolean if a field has been set.

### SetStartedAtNil

`func (o *AddressVerificationDetailSatoshiTestDetail) SetStartedAtNil(b bool)`

 SetStartedAtNil sets the value for StartedAt to be an explicit nil

### UnsetStartedAt
`func (o *AddressVerificationDetailSatoshiTestDetail) UnsetStartedAt()`

UnsetStartedAt ensures that no value is present for StartedAt, not even an explicit nil
### GetExpiresAt

`func (o *AddressVerificationDetailSatoshiTestDetail) GetExpiresAt() int64`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *AddressVerificationDetailSatoshiTestDetail) GetExpiresAtOk() (*int64, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *AddressVerificationDetailSatoshiTestDetail) SetExpiresAt(v int64)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *AddressVerificationDetailSatoshiTestDetail) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### SetExpiresAtNil

`func (o *AddressVerificationDetailSatoshiTestDetail) SetExpiresAtNil(b bool)`

 SetExpiresAtNil sets the value for ExpiresAt to be an explicit nil

### UnsetExpiresAt
`func (o *AddressVerificationDetailSatoshiTestDetail) UnsetExpiresAt()`

UnsetExpiresAt ensures that no value is present for ExpiresAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


