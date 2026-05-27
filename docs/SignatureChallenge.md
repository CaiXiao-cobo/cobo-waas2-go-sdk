# SignatureChallenge

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Address** | **string** | The self-custody wallet address that must sign this challenge. This is the counterparty address for the transaction: for deposits it is the sender&#39;s wallet, and for withdrawals it is the recipient&#39;s wallet.  | 
**Challenge** | **string** | The human-readable, time-sensitive message to sign. Contains the wallet address, a unique nonce, and a timestamp.  | 
**ExpiresIn** | **int32** | Number of seconds before the challenge expires. The signature must be submitted within this window. | 

## Methods

### NewSignatureChallenge

`func NewSignatureChallenge(address string, challenge string, expiresIn int32, ) *SignatureChallenge`

NewSignatureChallenge instantiates a new SignatureChallenge object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSignatureChallengeWithDefaults

`func NewSignatureChallengeWithDefaults() *SignatureChallenge`

NewSignatureChallengeWithDefaults instantiates a new SignatureChallenge object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAddress

`func (o *SignatureChallenge) GetAddress() string`

GetAddress returns the Address field if non-nil, zero value otherwise.

### GetAddressOk

`func (o *SignatureChallenge) GetAddressOk() (*string, bool)`

GetAddressOk returns a tuple with the Address field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddress

`func (o *SignatureChallenge) SetAddress(v string)`

SetAddress sets Address field to given value.


### GetChallenge

`func (o *SignatureChallenge) GetChallenge() string`

GetChallenge returns the Challenge field if non-nil, zero value otherwise.

### GetChallengeOk

`func (o *SignatureChallenge) GetChallengeOk() (*string, bool)`

GetChallengeOk returns a tuple with the Challenge field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChallenge

`func (o *SignatureChallenge) SetChallenge(v string)`

SetChallenge sets Challenge field to given value.


### GetExpiresIn

`func (o *SignatureChallenge) GetExpiresIn() int32`

GetExpiresIn returns the ExpiresIn field if non-nil, zero value otherwise.

### GetExpiresInOk

`func (o *SignatureChallenge) GetExpiresInOk() (*int32, bool)`

GetExpiresInOk returns a tuple with the ExpiresIn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresIn

`func (o *SignatureChallenge) SetExpiresIn(v int32)`

SetExpiresIn sets ExpiresIn field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


