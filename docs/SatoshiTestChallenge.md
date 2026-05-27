# SatoshiTestChallenge

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

### NewSatoshiTestChallenge

`func NewSatoshiTestChallenge(challengeId string, fromAddress string, toAddress string, amount string, tokenId string, chainId string, status SatoshiTestChallengeStatus, remainingSeconds int32, ) *SatoshiTestChallenge`

NewSatoshiTestChallenge instantiates a new SatoshiTestChallenge object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSatoshiTestChallengeWithDefaults

`func NewSatoshiTestChallengeWithDefaults() *SatoshiTestChallenge`

NewSatoshiTestChallengeWithDefaults instantiates a new SatoshiTestChallenge object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetChallengeId

`func (o *SatoshiTestChallenge) GetChallengeId() string`

GetChallengeId returns the ChallengeId field if non-nil, zero value otherwise.

### GetChallengeIdOk

`func (o *SatoshiTestChallenge) GetChallengeIdOk() (*string, bool)`

GetChallengeIdOk returns a tuple with the ChallengeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChallengeId

`func (o *SatoshiTestChallenge) SetChallengeId(v string)`

SetChallengeId sets ChallengeId field to given value.


### GetFromAddress

`func (o *SatoshiTestChallenge) GetFromAddress() string`

GetFromAddress returns the FromAddress field if non-nil, zero value otherwise.

### GetFromAddressOk

`func (o *SatoshiTestChallenge) GetFromAddressOk() (*string, bool)`

GetFromAddressOk returns a tuple with the FromAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromAddress

`func (o *SatoshiTestChallenge) SetFromAddress(v string)`

SetFromAddress sets FromAddress field to given value.


### GetToAddress

`func (o *SatoshiTestChallenge) GetToAddress() string`

GetToAddress returns the ToAddress field if non-nil, zero value otherwise.

### GetToAddressOk

`func (o *SatoshiTestChallenge) GetToAddressOk() (*string, bool)`

GetToAddressOk returns a tuple with the ToAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToAddress

`func (o *SatoshiTestChallenge) SetToAddress(v string)`

SetToAddress sets ToAddress field to given value.


### GetAmount

`func (o *SatoshiTestChallenge) GetAmount() string`

GetAmount returns the Amount field if non-nil, zero value otherwise.

### GetAmountOk

`func (o *SatoshiTestChallenge) GetAmountOk() (*string, bool)`

GetAmountOk returns a tuple with the Amount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmount

`func (o *SatoshiTestChallenge) SetAmount(v string)`

SetAmount sets Amount field to given value.


### GetTokenId

`func (o *SatoshiTestChallenge) GetTokenId() string`

GetTokenId returns the TokenId field if non-nil, zero value otherwise.

### GetTokenIdOk

`func (o *SatoshiTestChallenge) GetTokenIdOk() (*string, bool)`

GetTokenIdOk returns a tuple with the TokenId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokenId

`func (o *SatoshiTestChallenge) SetTokenId(v string)`

SetTokenId sets TokenId field to given value.


### GetChainId

`func (o *SatoshiTestChallenge) GetChainId() string`

GetChainId returns the ChainId field if non-nil, zero value otherwise.

### GetChainIdOk

`func (o *SatoshiTestChallenge) GetChainIdOk() (*string, bool)`

GetChainIdOk returns a tuple with the ChainId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChainId

`func (o *SatoshiTestChallenge) SetChainId(v string)`

SetChainId sets ChainId field to given value.


### GetStatus

`func (o *SatoshiTestChallenge) GetStatus() SatoshiTestChallengeStatus`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *SatoshiTestChallenge) GetStatusOk() (*SatoshiTestChallengeStatus, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *SatoshiTestChallenge) SetStatus(v SatoshiTestChallengeStatus)`

SetStatus sets Status field to given value.


### GetRemainingSeconds

`func (o *SatoshiTestChallenge) GetRemainingSeconds() int32`

GetRemainingSeconds returns the RemainingSeconds field if non-nil, zero value otherwise.

### GetRemainingSecondsOk

`func (o *SatoshiTestChallenge) GetRemainingSecondsOk() (*int32, bool)`

GetRemainingSecondsOk returns a tuple with the RemainingSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemainingSeconds

`func (o *SatoshiTestChallenge) SetRemainingSeconds(v int32)`

SetRemainingSeconds sets RemainingSeconds field to given value.


### GetMatchedTxid

`func (o *SatoshiTestChallenge) GetMatchedTxid() string`

GetMatchedTxid returns the MatchedTxid field if non-nil, zero value otherwise.

### GetMatchedTxidOk

`func (o *SatoshiTestChallenge) GetMatchedTxidOk() (*string, bool)`

GetMatchedTxidOk returns a tuple with the MatchedTxid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatchedTxid

`func (o *SatoshiTestChallenge) SetMatchedTxid(v string)`

SetMatchedTxid sets MatchedTxid field to given value.

### HasMatchedTxid

`func (o *SatoshiTestChallenge) HasMatchedTxid() bool`

HasMatchedTxid returns a boolean if a field has been set.

### SetMatchedTxidNil

`func (o *SatoshiTestChallenge) SetMatchedTxidNil(b bool)`

 SetMatchedTxidNil sets the value for MatchedTxid to be an explicit nil

### UnsetMatchedTxid
`func (o *SatoshiTestChallenge) UnsetMatchedTxid()`

UnsetMatchedTxid ensures that no value is present for MatchedTxid, not even an explicit nil
### GetStartedAt

`func (o *SatoshiTestChallenge) GetStartedAt() int64`

GetStartedAt returns the StartedAt field if non-nil, zero value otherwise.

### GetStartedAtOk

`func (o *SatoshiTestChallenge) GetStartedAtOk() (*int64, bool)`

GetStartedAtOk returns a tuple with the StartedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartedAt

`func (o *SatoshiTestChallenge) SetStartedAt(v int64)`

SetStartedAt sets StartedAt field to given value.

### HasStartedAt

`func (o *SatoshiTestChallenge) HasStartedAt() bool`

HasStartedAt returns a boolean if a field has been set.

### SetStartedAtNil

`func (o *SatoshiTestChallenge) SetStartedAtNil(b bool)`

 SetStartedAtNil sets the value for StartedAt to be an explicit nil

### UnsetStartedAt
`func (o *SatoshiTestChallenge) UnsetStartedAt()`

UnsetStartedAt ensures that no value is present for StartedAt, not even an explicit nil
### GetExpiresAt

`func (o *SatoshiTestChallenge) GetExpiresAt() int64`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *SatoshiTestChallenge) GetExpiresAtOk() (*int64, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *SatoshiTestChallenge) SetExpiresAt(v int64)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *SatoshiTestChallenge) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### SetExpiresAtNil

`func (o *SatoshiTestChallenge) SetExpiresAtNil(b bool)`

 SetExpiresAtNil sets the value for ExpiresAt to be an explicit nil

### UnsetExpiresAt
`func (o *SatoshiTestChallenge) UnsetExpiresAt()`

UnsetExpiresAt ensures that no value is present for ExpiresAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


