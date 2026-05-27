# ListBulkSends200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | Pointer to [**[]PaymentBulkSend**](PaymentBulkSend.md) |  | [optional] 
**Pagination** | Pointer to [**Pagination**](Pagination.md) |  | [optional] 

## Methods

### NewListBulkSends200Response

`func NewListBulkSends200Response() *ListBulkSends200Response`

NewListBulkSends200Response instantiates a new ListBulkSends200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListBulkSends200ResponseWithDefaults

`func NewListBulkSends200ResponseWithDefaults() *ListBulkSends200Response`

NewListBulkSends200ResponseWithDefaults instantiates a new ListBulkSends200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *ListBulkSends200Response) GetData() []PaymentBulkSend`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ListBulkSends200Response) GetDataOk() (*[]PaymentBulkSend, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ListBulkSends200Response) SetData(v []PaymentBulkSend)`

SetData sets Data field to given value.

### HasData

`func (o *ListBulkSends200Response) HasData() bool`

HasData returns a boolean if a field has been set.

### GetPagination

`func (o *ListBulkSends200Response) GetPagination() Pagination`

GetPagination returns the Pagination field if non-nil, zero value otherwise.

### GetPaginationOk

`func (o *ListBulkSends200Response) GetPaginationOk() (*Pagination, bool)`

GetPaginationOk returns a tuple with the Pagination field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPagination

`func (o *ListBulkSends200Response) SetPagination(v Pagination)`

SetPagination sets Pagination field to given value.

### HasPagination

`func (o *ListBulkSends200Response) HasPagination() bool`

HasPagination returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


