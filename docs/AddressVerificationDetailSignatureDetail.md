# AddressVerificationDetailSignatureDetail

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Address** | **string** | The self-custody wallet address that signed the challenge. | 
**Challenge** | Pointer to **NullableString** | The challenge string that was signed. | [optional] 
**Signature** | Pointer to **NullableString** | The wallet signature submitted by the client. | [optional] 
**VerifiedAt** | Pointer to **NullableInt64** | Timestamp (milliseconds) when the signature was verified. | [optional] 

## Methods

### NewAddressVerificationDetailSignatureDetail

`func NewAddressVerificationDetailSignatureDetail(address string, ) *AddressVerificationDetailSignatureDetail`

NewAddressVerificationDetailSignatureDetail instantiates a new AddressVerificationDetailSignatureDetail object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAddressVerificationDetailSignatureDetailWithDefaults

`func NewAddressVerificationDetailSignatureDetailWithDefaults() *AddressVerificationDetailSignatureDetail`

NewAddressVerificationDetailSignatureDetailWithDefaults instantiates a new AddressVerificationDetailSignatureDetail object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAddress

`func (o *AddressVerificationDetailSignatureDetail) GetAddress() string`

GetAddress returns the Address field if non-nil, zero value otherwise.

### GetAddressOk

`func (o *AddressVerificationDetailSignatureDetail) GetAddressOk() (*string, bool)`

GetAddressOk returns a tuple with the Address field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddress

`func (o *AddressVerificationDetailSignatureDetail) SetAddress(v string)`

SetAddress sets Address field to given value.


### GetChallenge

`func (o *AddressVerificationDetailSignatureDetail) GetChallenge() string`

GetChallenge returns the Challenge field if non-nil, zero value otherwise.

### GetChallengeOk

`func (o *AddressVerificationDetailSignatureDetail) GetChallengeOk() (*string, bool)`

GetChallengeOk returns a tuple with the Challenge field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChallenge

`func (o *AddressVerificationDetailSignatureDetail) SetChallenge(v string)`

SetChallenge sets Challenge field to given value.

### HasChallenge

`func (o *AddressVerificationDetailSignatureDetail) HasChallenge() bool`

HasChallenge returns a boolean if a field has been set.

### SetChallengeNil

`func (o *AddressVerificationDetailSignatureDetail) SetChallengeNil(b bool)`

 SetChallengeNil sets the value for Challenge to be an explicit nil

### UnsetChallenge
`func (o *AddressVerificationDetailSignatureDetail) UnsetChallenge()`

UnsetChallenge ensures that no value is present for Challenge, not even an explicit nil
### GetSignature

`func (o *AddressVerificationDetailSignatureDetail) GetSignature() string`

GetSignature returns the Signature field if non-nil, zero value otherwise.

### GetSignatureOk

`func (o *AddressVerificationDetailSignatureDetail) GetSignatureOk() (*string, bool)`

GetSignatureOk returns a tuple with the Signature field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSignature

`func (o *AddressVerificationDetailSignatureDetail) SetSignature(v string)`

SetSignature sets Signature field to given value.

### HasSignature

`func (o *AddressVerificationDetailSignatureDetail) HasSignature() bool`

HasSignature returns a boolean if a field has been set.

### SetSignatureNil

`func (o *AddressVerificationDetailSignatureDetail) SetSignatureNil(b bool)`

 SetSignatureNil sets the value for Signature to be an explicit nil

### UnsetSignature
`func (o *AddressVerificationDetailSignatureDetail) UnsetSignature()`

UnsetSignature ensures that no value is present for Signature, not even an explicit nil
### GetVerifiedAt

`func (o *AddressVerificationDetailSignatureDetail) GetVerifiedAt() int64`

GetVerifiedAt returns the VerifiedAt field if non-nil, zero value otherwise.

### GetVerifiedAtOk

`func (o *AddressVerificationDetailSignatureDetail) GetVerifiedAtOk() (*int64, bool)`

GetVerifiedAtOk returns a tuple with the VerifiedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVerifiedAt

`func (o *AddressVerificationDetailSignatureDetail) SetVerifiedAt(v int64)`

SetVerifiedAt sets VerifiedAt field to given value.

### HasVerifiedAt

`func (o *AddressVerificationDetailSignatureDetail) HasVerifiedAt() bool`

HasVerifiedAt returns a boolean if a field has been set.

### SetVerifiedAtNil

`func (o *AddressVerificationDetailSignatureDetail) SetVerifiedAtNil(b bool)`

 SetVerifiedAtNil sets the value for VerifiedAt to be an explicit nil

### UnsetVerifiedAt
`func (o *AddressVerificationDetailSignatureDetail) UnsetVerifiedAt()`

UnsetVerifiedAt ensures that no value is present for VerifiedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


