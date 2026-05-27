# AddressVerificationDetail

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**VerificationId** | **string** | The unique identifier of this verification record. | 
**Address** | **string** | The counterparty (self-custody) wallet address being verified. | 
**ChainId** | **string** | The chain on which this address is verified. | 
**Status** | [**AddressVerificationStatus**](AddressVerificationStatus.md) |  | 
**VerificationMethod** | [**AddressVerificationMethod**](AddressVerificationMethod.md) |  | 
**VerifiedAt** | Pointer to **NullableInt64** | Timestamp (milliseconds) when verification completed. &#x60;null&#x60; while &#x60;status&#x3D;PENDING&#x60; or &#x60;FAILED&#x60;. | [optional] 
**SatoshiTestDetail** | Pointer to [**NullableAddressVerificationDetailSatoshiTestDetail**](AddressVerificationDetailSatoshiTestDetail.md) |  | [optional] 
**SignatureDetail** | Pointer to [**NullableAddressVerificationDetailSignatureDetail**](AddressVerificationDetailSignatureDetail.md) |  | [optional] 

## Methods

### NewAddressVerificationDetail

`func NewAddressVerificationDetail(verificationId string, address string, chainId string, status AddressVerificationStatus, verificationMethod AddressVerificationMethod, ) *AddressVerificationDetail`

NewAddressVerificationDetail instantiates a new AddressVerificationDetail object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAddressVerificationDetailWithDefaults

`func NewAddressVerificationDetailWithDefaults() *AddressVerificationDetail`

NewAddressVerificationDetailWithDefaults instantiates a new AddressVerificationDetail object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVerificationId

`func (o *AddressVerificationDetail) GetVerificationId() string`

GetVerificationId returns the VerificationId field if non-nil, zero value otherwise.

### GetVerificationIdOk

`func (o *AddressVerificationDetail) GetVerificationIdOk() (*string, bool)`

GetVerificationIdOk returns a tuple with the VerificationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVerificationId

`func (o *AddressVerificationDetail) SetVerificationId(v string)`

SetVerificationId sets VerificationId field to given value.


### GetAddress

`func (o *AddressVerificationDetail) GetAddress() string`

GetAddress returns the Address field if non-nil, zero value otherwise.

### GetAddressOk

`func (o *AddressVerificationDetail) GetAddressOk() (*string, bool)`

GetAddressOk returns a tuple with the Address field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddress

`func (o *AddressVerificationDetail) SetAddress(v string)`

SetAddress sets Address field to given value.


### GetChainId

`func (o *AddressVerificationDetail) GetChainId() string`

GetChainId returns the ChainId field if non-nil, zero value otherwise.

### GetChainIdOk

`func (o *AddressVerificationDetail) GetChainIdOk() (*string, bool)`

GetChainIdOk returns a tuple with the ChainId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChainId

`func (o *AddressVerificationDetail) SetChainId(v string)`

SetChainId sets ChainId field to given value.


### GetStatus

`func (o *AddressVerificationDetail) GetStatus() AddressVerificationStatus`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *AddressVerificationDetail) GetStatusOk() (*AddressVerificationStatus, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *AddressVerificationDetail) SetStatus(v AddressVerificationStatus)`

SetStatus sets Status field to given value.


### GetVerificationMethod

`func (o *AddressVerificationDetail) GetVerificationMethod() AddressVerificationMethod`

GetVerificationMethod returns the VerificationMethod field if non-nil, zero value otherwise.

### GetVerificationMethodOk

`func (o *AddressVerificationDetail) GetVerificationMethodOk() (*AddressVerificationMethod, bool)`

GetVerificationMethodOk returns a tuple with the VerificationMethod field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVerificationMethod

`func (o *AddressVerificationDetail) SetVerificationMethod(v AddressVerificationMethod)`

SetVerificationMethod sets VerificationMethod field to given value.


### GetVerifiedAt

`func (o *AddressVerificationDetail) GetVerifiedAt() int64`

GetVerifiedAt returns the VerifiedAt field if non-nil, zero value otherwise.

### GetVerifiedAtOk

`func (o *AddressVerificationDetail) GetVerifiedAtOk() (*int64, bool)`

GetVerifiedAtOk returns a tuple with the VerifiedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVerifiedAt

`func (o *AddressVerificationDetail) SetVerifiedAt(v int64)`

SetVerifiedAt sets VerifiedAt field to given value.

### HasVerifiedAt

`func (o *AddressVerificationDetail) HasVerifiedAt() bool`

HasVerifiedAt returns a boolean if a field has been set.

### SetVerifiedAtNil

`func (o *AddressVerificationDetail) SetVerifiedAtNil(b bool)`

 SetVerifiedAtNil sets the value for VerifiedAt to be an explicit nil

### UnsetVerifiedAt
`func (o *AddressVerificationDetail) UnsetVerifiedAt()`

UnsetVerifiedAt ensures that no value is present for VerifiedAt, not even an explicit nil
### GetSatoshiTestDetail

`func (o *AddressVerificationDetail) GetSatoshiTestDetail() AddressVerificationDetailSatoshiTestDetail`

GetSatoshiTestDetail returns the SatoshiTestDetail field if non-nil, zero value otherwise.

### GetSatoshiTestDetailOk

`func (o *AddressVerificationDetail) GetSatoshiTestDetailOk() (*AddressVerificationDetailSatoshiTestDetail, bool)`

GetSatoshiTestDetailOk returns a tuple with the SatoshiTestDetail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSatoshiTestDetail

`func (o *AddressVerificationDetail) SetSatoshiTestDetail(v AddressVerificationDetailSatoshiTestDetail)`

SetSatoshiTestDetail sets SatoshiTestDetail field to given value.

### HasSatoshiTestDetail

`func (o *AddressVerificationDetail) HasSatoshiTestDetail() bool`

HasSatoshiTestDetail returns a boolean if a field has been set.

### SetSatoshiTestDetailNil

`func (o *AddressVerificationDetail) SetSatoshiTestDetailNil(b bool)`

 SetSatoshiTestDetailNil sets the value for SatoshiTestDetail to be an explicit nil

### UnsetSatoshiTestDetail
`func (o *AddressVerificationDetail) UnsetSatoshiTestDetail()`

UnsetSatoshiTestDetail ensures that no value is present for SatoshiTestDetail, not even an explicit nil
### GetSignatureDetail

`func (o *AddressVerificationDetail) GetSignatureDetail() AddressVerificationDetailSignatureDetail`

GetSignatureDetail returns the SignatureDetail field if non-nil, zero value otherwise.

### GetSignatureDetailOk

`func (o *AddressVerificationDetail) GetSignatureDetailOk() (*AddressVerificationDetailSignatureDetail, bool)`

GetSignatureDetailOk returns a tuple with the SignatureDetail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSignatureDetail

`func (o *AddressVerificationDetail) SetSignatureDetail(v AddressVerificationDetailSignatureDetail)`

SetSignatureDetail sets SignatureDetail field to given value.

### HasSignatureDetail

`func (o *AddressVerificationDetail) HasSignatureDetail() bool`

HasSignatureDetail returns a boolean if a field has been set.

### SetSignatureDetailNil

`func (o *AddressVerificationDetail) SetSignatureDetailNil(b bool)`

 SetSignatureDetailNil sets the value for SignatureDetail to be an explicit nil

### UnsetSignatureDetail
`func (o *AddressVerificationDetail) UnsetSignatureDetail()`

UnsetSignatureDetail ensures that no value is present for SignatureDetail, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


