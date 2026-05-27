# AddressVerification

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**VerificationId** | **string** | The unique identifier of this verification record. | 
**Address** | **string** | The counterparty (self-custody) wallet address being verified. | 
**ChainId** | **string** | The chain on which this address is verified. | 
**Status** | [**AddressVerificationStatus**](AddressVerificationStatus.md) |  | 
**VerificationMethod** | [**AddressVerificationMethod**](AddressVerificationMethod.md) |  | 
**VerifiedAt** | Pointer to **NullableInt64** | Timestamp (milliseconds) when verification completed. &#x60;null&#x60; while &#x60;status&#x3D;PENDING&#x60; or &#x60;FAILED&#x60;. | [optional] 

## Methods

### NewAddressVerification

`func NewAddressVerification(verificationId string, address string, chainId string, status AddressVerificationStatus, verificationMethod AddressVerificationMethod, ) *AddressVerification`

NewAddressVerification instantiates a new AddressVerification object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAddressVerificationWithDefaults

`func NewAddressVerificationWithDefaults() *AddressVerification`

NewAddressVerificationWithDefaults instantiates a new AddressVerification object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVerificationId

`func (o *AddressVerification) GetVerificationId() string`

GetVerificationId returns the VerificationId field if non-nil, zero value otherwise.

### GetVerificationIdOk

`func (o *AddressVerification) GetVerificationIdOk() (*string, bool)`

GetVerificationIdOk returns a tuple with the VerificationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVerificationId

`func (o *AddressVerification) SetVerificationId(v string)`

SetVerificationId sets VerificationId field to given value.


### GetAddress

`func (o *AddressVerification) GetAddress() string`

GetAddress returns the Address field if non-nil, zero value otherwise.

### GetAddressOk

`func (o *AddressVerification) GetAddressOk() (*string, bool)`

GetAddressOk returns a tuple with the Address field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddress

`func (o *AddressVerification) SetAddress(v string)`

SetAddress sets Address field to given value.


### GetChainId

`func (o *AddressVerification) GetChainId() string`

GetChainId returns the ChainId field if non-nil, zero value otherwise.

### GetChainIdOk

`func (o *AddressVerification) GetChainIdOk() (*string, bool)`

GetChainIdOk returns a tuple with the ChainId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChainId

`func (o *AddressVerification) SetChainId(v string)`

SetChainId sets ChainId field to given value.


### GetStatus

`func (o *AddressVerification) GetStatus() AddressVerificationStatus`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *AddressVerification) GetStatusOk() (*AddressVerificationStatus, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *AddressVerification) SetStatus(v AddressVerificationStatus)`

SetStatus sets Status field to given value.


### GetVerificationMethod

`func (o *AddressVerification) GetVerificationMethod() AddressVerificationMethod`

GetVerificationMethod returns the VerificationMethod field if non-nil, zero value otherwise.

### GetVerificationMethodOk

`func (o *AddressVerification) GetVerificationMethodOk() (*AddressVerificationMethod, bool)`

GetVerificationMethodOk returns a tuple with the VerificationMethod field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVerificationMethod

`func (o *AddressVerification) SetVerificationMethod(v AddressVerificationMethod)`

SetVerificationMethod sets VerificationMethod field to given value.


### GetVerifiedAt

`func (o *AddressVerification) GetVerifiedAt() int64`

GetVerifiedAt returns the VerifiedAt field if non-nil, zero value otherwise.

### GetVerifiedAtOk

`func (o *AddressVerification) GetVerifiedAtOk() (*int64, bool)`

GetVerifiedAtOk returns a tuple with the VerifiedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVerifiedAt

`func (o *AddressVerification) SetVerifiedAt(v int64)`

SetVerifiedAt sets VerifiedAt field to given value.

### HasVerifiedAt

`func (o *AddressVerification) HasVerifiedAt() bool`

HasVerifiedAt returns a boolean if a field has been set.

### SetVerifiedAtNil

`func (o *AddressVerification) SetVerifiedAtNil(b bool)`

 SetVerifiedAtNil sets the value for VerifiedAt to be an explicit nil

### UnsetVerifiedAt
`func (o *AddressVerification) UnsetVerifiedAt()`

UnsetVerifiedAt ensures that no value is present for VerifiedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


