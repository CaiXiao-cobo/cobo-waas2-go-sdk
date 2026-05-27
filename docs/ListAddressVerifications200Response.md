# ListAddressVerifications200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]AddressVerification**](AddressVerification.md) | The page of address verification records. | 
**Pagination** | [**Pagination**](Pagination.md) |  | 

## Methods

### NewListAddressVerifications200Response

`func NewListAddressVerifications200Response(data []AddressVerification, pagination Pagination, ) *ListAddressVerifications200Response`

NewListAddressVerifications200Response instantiates a new ListAddressVerifications200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListAddressVerifications200ResponseWithDefaults

`func NewListAddressVerifications200ResponseWithDefaults() *ListAddressVerifications200Response`

NewListAddressVerifications200ResponseWithDefaults instantiates a new ListAddressVerifications200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *ListAddressVerifications200Response) GetData() []AddressVerification`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ListAddressVerifications200Response) GetDataOk() (*[]AddressVerification, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ListAddressVerifications200Response) SetData(v []AddressVerification)`

SetData sets Data field to given value.


### GetPagination

`func (o *ListAddressVerifications200Response) GetPagination() Pagination`

GetPagination returns the Pagination field if non-nil, zero value otherwise.

### GetPaginationOk

`func (o *ListAddressVerifications200Response) GetPaginationOk() (*Pagination, bool)`

GetPaginationOk returns a tuple with the Pagination field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPagination

`func (o *ListAddressVerifications200Response) SetPagination(v Pagination)`

SetPagination sets Pagination field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


