# 

**`API Version:`** `2.25.1`

sMsMode API-REST Documentation



## Base URL

The base URL for this API is `http://rest.smsmode.com/`









# <a name="api_reference"></a>API Reference

* [report-controller](#report_controller)
* [invoice-controller](#invoice_controller)
* [authentication-controller](#authentication_controller)
* [contact-controller](#contact_controller)
* [customer-controller](#customer_controller)
* [group-controller](#group_controller)
* [campaign-controller](#campaign_controller)
* [transfer-controller](#transfer_controller)
* [email-api-configuration-controller](#email_api_configuration_controller)
* [message-controller](#message_controller)
* [register-controler](#register_controler)
* [credit-consumption-controller](#credit_consumption_controller)
* [pricing-controller](#pricing_controller)
* [message-model-controller](#message_model_controller)
* [societe-info-controller](#societe_info_controller)

## <a name="report_controller"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "report-controller") report-controller


### <a name="list_using_get_8"></a>![Endpoint: ](https://apidocs.io/img/method.png "listUsingGET_8") listUsingGET_8


**`GET`** `/reports`

> *Tags:*  ``` Skips Authentication ``` 

> list




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `131` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="list_page_using_get_8"></a>![Endpoint: ](https://apidocs.io/img/method.png "listPageUsingGET_8") listPageUsingGET_8


**`GET`** `/reports/pages/{page}`

> *Tags:*  ``` Skips Authentication ``` 

> listPage




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| page | number |  ``` Required ```  | page | `131` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `131` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="get_using_get_8"></a>![Endpoint: ](https://apidocs.io/img/method.png "getUsingGET_8") getUsingGET_8


**`GET`** `/reports/{messageRef}`

> *Tags:*  ``` Skips Authentication ``` 

> get




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| messageRef | string |  ``` Required ```  | messageRef | `"messageRef"` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `131` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="get_page_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "getPageUsingGET") getPageUsingGET


**`GET`** `/reports/{messageRef}/pages/{page}`

> *Tags:*  ``` Skips Authentication ``` 

> getPage




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| messageRef | string |  ``` Required ```  | messageRef | `"messageRef"` | 
| page | number |  ``` Required ```  | page | `131` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `131` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="find_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "findUsingGET") findUsingGET


**`GET`** `/reports/{messageRef}/{destinataire}`

> *Tags:*  ``` Skips Authentication ``` 

> find




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| messageRef | string |  ``` Required ```  | messageRef | `"messageRef"` | 
| destinataire | string |  ``` Required ```  | destinataire | `"destinataire"` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


[Back to API Reference](#api_reference)

## <a name="invoice_controller"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "invoice-controller") invoice-controller


### <a name="list_using_get_5"></a>![Endpoint: ](https://apidocs.io/img/method.png "listUsingGET_5") listUsingGET_5


**`GET`** `/invoices`

> *Tags:*  ``` Skips Authentication ``` 

> View a list of invoices




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `131` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="list_page_using_get_5"></a>![Endpoint: ](https://apidocs.io/img/method.png "listPageUsingGET_5") listPageUsingGET_5


**`GET`** `/invoices/pages/{page}`

> *Tags:*  ``` Skips Authentication ``` 

> listPage




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| page | number |  ``` Required ```  | page | `131` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `131` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="get_pdf_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "getPdfUsingGET") getPdfUsingGET


**`GET`** `/invoices/pdf/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> Generate an invoice in a pdf file




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | number |  ``` Required ```  | id | `131` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| base64 | boolean |  ``` Required ```  | base64 | `true` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="get_using_get_5"></a>![Endpoint: ](https://apidocs.io/img/method.png "getUsingGET_5") getUsingGET_5


**`GET`** `/invoices/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> Show an invoice




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | number |  ``` Required ```  | id | `131` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[InvoiceResource](#invoice_resource)**) 

```
{
  "amount": 131.000044143759,
  "completionDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "credit": 131.000044143759,
  "currency": "currency",
  "invoiceId": 131,
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "messageCredit": 131.000044143759,
  "reference": "reference",
  "transactionStatus": "transactionStatus",
  "transactionType": "transactionType",
  "vatIncluded": true
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


[Back to API Reference](#api_reference)

## <a name="authentication_controller"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "authentication-controller") authentication-controller


### <a name="get_token_using_post"></a>![Endpoint: ](https://apidocs.io/img/method.png "getTokenUsingPOST") getTokenUsingPOST


**`POST`** `/authentication`

> *Tags:*  ``` Skips Authentication ``` 

> Generate the OAuth Token




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [AuthenticationResource](#authentication_resource) |  ``` Required ```  | request | 

 *Example Body* 
``` 
{
  "login": "login",
  "password": "password"
}
``` 

#### Responses
**201** 

> OK


 *Example Body* (**[TokenResource](#token_resource)**) 

```
{
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "token": "token"
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


[Back to API Reference](#api_reference)

## <a name="contact_controller"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "contact-controller") contact-controller


### <a name="list_using_get_1"></a>![Endpoint: ](https://apidocs.io/img/method.png "listUsingGET_1") listUsingGET_1


**`GET`** `/contacts`

> *Tags:*  ``` Skips Authentication ``` 

> View a list of contacts




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `131` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="add_using_post"></a>![Endpoint: ](https://apidocs.io/img/method.png "addUsingPOST") addUsingPOST


**`POST`** `/contacts`

> *Tags:*  ``` Skips Authentication ``` 

> Add a contact




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ContactResource](#contact_resource) |  ``` Required ```  | resource | 

 *Example Body* 
``` 
{
  "address": {
    "address1": "address1",
    "address2": "address2",
    "city": "city",
    "country": "country",
    "links": [
      {
        "href": "href",
        "rel": "rel",
        "templated": true
      }
    ],
    "zipCode": "zipCode"
  },
  "birthDate": "yyyy-MM-dd",
  "company": "company",
  "contactId": 131,
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "email": "email",
  "emailInvalid": true,
  "emailOptout": true,
  "fax": "fax",
  "firstName": "firstName",
  "groups": [
    {
      "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
      "description": "description",
      "groupId": 222,
      "links": [
        {
          "href": "href",
          "rel": "rel",
          "templated": true
        }
      ],
      "name": "name",
      "updateDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
      "valid": true
    }
  ],
  "lastName": "lastName",
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "mobile": "mobile",
  "mobileInvalid": true,
  "mobileOptout": true,
  "modificationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "other": "other",
  "phone": "phone",
  "title": "title",
  "valid": true,
  "vatNumber": "vatNumber"
}
``` 

#### Responses
**201** 

> OK


 *Example Body* (**[ContactResource](#contact_resource)**) 

```
{
  "address": {
    "address1": "address1",
    "address2": "address2",
    "city": "city",
    "country": "country",
    "links": [
      {
        "href": "href",
        "rel": "rel",
        "templated": true
      }
    ],
    "zipCode": "zipCode"
  },
  "birthDate": "yyyy-MM-dd",
  "company": "company",
  "contactId": 222,
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "email": "email",
  "emailInvalid": true,
  "emailOptout": true,
  "fax": "fax",
  "firstName": "firstName",
  "groups": [
    {
      "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
      "description": "description",
      "groupId": 222,
      "links": [
        {
          "href": "href",
          "rel": "rel",
          "templated": true
        }
      ],
      "name": "name",
      "updateDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
      "valid": true
    }
  ],
  "lastName": "lastName",
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "mobile": "mobile",
  "mobileInvalid": true,
  "mobileOptout": true,
  "modificationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "other": "other",
  "phone": "phone",
  "title": "title",
  "valid": true,
  "vatNumber": "vatNumber"
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="delete_book_using_delete"></a>![Endpoint: ](https://apidocs.io/img/method.png "deleteBookUsingDELETE") deleteBookUsingDELETE


**`DELETE`** `/contacts/book`

> *Tags:*  ``` Skips Authentication ``` 

> Remove all contacts and groups of the account




#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**204** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden


### <a name="get_customer_info_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "getCustomerInfoUsingGET") getCustomerInfoUsingGET


**`GET`** `/contacts/customer`

> *Tags:*  ``` Skips Authentication ``` 

> Show contact info of customer




#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[ContactResource](#contact_resource)**) 

```
{
  "address": {
    "address1": "address1",
    "address2": "address2",
    "city": "city",
    "country": "country",
    "links": [
      {
        "href": "href",
        "rel": "rel",
        "templated": true
      }
    ],
    "zipCode": "zipCode"
  },
  "birthDate": "yyyy-MM-dd",
  "company": "company",
  "contactId": 222,
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "email": "email",
  "emailInvalid": true,
  "emailOptout": true,
  "fax": "fax",
  "firstName": "firstName",
  "groups": [
    {
      "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
      "description": "description",
      "groupId": 222,
      "links": [
        {
          "href": "href",
          "rel": "rel",
          "templated": true
        }
      ],
      "name": "name",
      "updateDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
      "valid": true
    }
  ],
  "lastName": "lastName",
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "mobile": "mobile",
  "mobileInvalid": true,
  "mobileOptout": true,
  "modificationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "other": "other",
  "phone": "phone",
  "title": "title",
  "valid": true,
  "vatNumber": "vatNumber"
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="edit_customer_using_put"></a>![Endpoint: ](https://apidocs.io/img/method.png "editCustomerUsingPUT") editCustomerUsingPUT


**`PUT`** `/contacts/customer`

> *Tags:*  ``` Skips Authentication ``` 

> Edit contact info of customer




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ContactResource](#contact_resource) |  ``` Required ```  | resource | 

 *Example Body* 
``` 
{
  "address": {
    "address1": "address1",
    "address2": "address2",
    "city": "city",
    "country": "country",
    "links": [
      {
        "href": "href",
        "rel": "rel",
        "templated": true
      }
    ],
    "zipCode": "zipCode"
  },
  "birthDate": "yyyy-MM-dd",
  "company": "company",
  "contactId": 222,
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "email": "email",
  "emailInvalid": true,
  "emailOptout": true,
  "fax": "fax",
  "firstName": "firstName",
  "groups": [
    {
      "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
      "description": "description",
      "groupId": 222,
      "links": [
        {
          "href": "href",
          "rel": "rel",
          "templated": true
        }
      ],
      "name": "name",
      "updateDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
      "valid": true
    }
  ],
  "lastName": "lastName",
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "mobile": "mobile",
  "mobileInvalid": true,
  "mobileOptout": true,
  "modificationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "other": "other",
  "phone": "phone",
  "title": "title",
  "valid": true,
  "vatNumber": "vatNumber"
}
``` 

#### Responses
**201** 

> OK


 *Example Body* (**[ContactResource](#contact_resource)**) 

```
{
  "address": {
    "address1": "address1",
    "address2": "address2",
    "city": "city",
    "country": "country",
    "links": [
      {
        "href": "href",
        "rel": "rel",
        "templated": true
      }
    ],
    "zipCode": "zipCode"
  },
  "birthDate": "yyyy-MM-dd",
  "company": "company",
  "contactId": 222,
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "email": "email",
  "emailInvalid": true,
  "emailOptout": true,
  "fax": "fax",
  "firstName": "firstName",
  "groups": [
    {
      "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
      "description": "description",
      "groupId": 222,
      "links": [
        {
          "href": "href",
          "rel": "rel",
          "templated": true
        }
      ],
      "name": "name",
      "updateDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
      "valid": true
    }
  ],
  "lastName": "lastName",
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "mobile": "mobile",
  "mobileInvalid": true,
  "mobileOptout": true,
  "modificationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "other": "other",
  "phone": "phone",
  "title": "title",
  "valid": true,
  "vatNumber": "vatNumber"
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="delete_list_using_post"></a>![Endpoint: ](https://apidocs.io/img/method.png "deleteListUsingPOST") deleteListUsingPOST


**`POST`** `/contacts/delete`

> *Tags:*  ``` Skips Authentication ``` 

> Delete a list of contacts




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| number |  ``` Required ```  ``` Collection ```  | idList | 

 *Example Body* 
``` 
[
  222
]
``` 

#### Responses
**201** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="export_contacts_using_post"></a>![Endpoint: ](https://apidocs.io/img/method.png "exportContactsUsingPOST") exportContactsUsingPOST


**`POST`** `/contacts/export`

> *Tags:*  ``` Skips Authentication ``` 

> Export contacts in csv format




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| string |  ``` Required ```  ``` Collection ```  | fields | 

 *Example Body* 
``` 
[
  "fields"
]
``` 

#### Responses
**201** 

> OK


 *Example Body* (**[DeferredResult«ResponseEntity«object»»](#deferred_result«response_entity«object»»)**) 

```
{
  "result": {},
  "setOrExpired": true
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="upload_blocking_using_post"></a>![Endpoint: ](https://apidocs.io/img/method.png "uploadBlockingUsingPOST") uploadBlockingUsingPOST


**`POST`** `/contacts/import`

> *Tags:*  ``` Skips Authentication ``` 

> Import contacts via xls or csv files




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| model | string |  ``` Required ```  | model | `"model"` | 

#### Request Headers
>Content-Type=multipart/form-data;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Multipart Form Data

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| file | file |  ``` Required ```  | file |  | 

*Example Body*
```
 file = path/to/file 
```

#### Responses
**201** 

> OK


 *Example Body* (**[DeferredResult«ResponseEntity«object»»](#deferred_result«response_entity«object»»)**) 

```
{
  "result": {},
  "setOrExpired": true
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="list_page_using_get_1"></a>![Endpoint: ](https://apidocs.io/img/method.png "listPageUsingGET_1") listPageUsingGET_1


**`GET`** `/contacts/pages/{page}`

> *Tags:*  ``` Skips Authentication ``` 

> listPage




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| page | number |  ``` Required ```  | page | `222` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `222` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[Resources«ContactResource»](#resources«contact_resource»)**) 

```
{
  "content": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ]
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="search_using_get_1"></a>![Endpoint: ](https://apidocs.io/img/method.png "searchUsingGET_1") searchUsingGET_1


**`GET`** `/contacts/search/{name}`

> *Tags:*  ``` Skips Authentication ``` 

> search




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| name | string |  ``` Required ```  | name | `"name"` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `222` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="get_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "getUsingGET") getUsingGET


**`GET`** `/contacts/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> Show a contact




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | number |  ``` Required ```  | id | `222` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[ContactResource](#contact_resource)**) 

```
{
  "address": {
    "address1": "address1",
    "address2": "address2",
    "city": "city",
    "country": "country",
    "links": [
      {
        "href": "href",
        "rel": "rel",
        "templated": true
      }
    ],
    "zipCode": "zipCode"
  },
  "birthDate": "yyyy-MM-dd",
  "company": "company",
  "contactId": 222,
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "email": "email",
  "emailInvalid": true,
  "emailOptout": true,
  "fax": "fax",
  "firstName": "firstName",
  "groups": [
    {
      "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
      "description": "description",
      "groupId": 222,
      "links": [
        {
          "href": "href",
          "rel": "rel",
          "templated": true
        }
      ],
      "name": "name",
      "updateDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
      "valid": true
    }
  ],
  "lastName": "lastName",
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "mobile": "mobile",
  "mobileInvalid": true,
  "mobileOptout": true,
  "modificationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "other": "other",
  "phone": "phone",
  "title": "title",
  "valid": true,
  "vatNumber": "vatNumber"
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="update_using_put"></a>![Endpoint: ](https://apidocs.io/img/method.png "updateUsingPUT") updateUsingPUT


**`PUT`** `/contacts/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> Update a contact




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | number |  ``` Required ```  | id | `222` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ContactResource](#contact_resource) |  ``` Required ```  | resource | 

 *Example Body* 
``` 
{
  "address": {
    "address1": "address1",
    "address2": "address2",
    "city": "city",
    "country": "country",
    "links": [
      {
        "href": "href",
        "rel": "rel",
        "templated": true
      }
    ],
    "zipCode": "zipCode"
  },
  "birthDate": "yyyy-MM-dd",
  "company": "company",
  "contactId": 222,
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "email": "email",
  "emailInvalid": true,
  "emailOptout": true,
  "fax": "fax",
  "firstName": "firstName",
  "groups": [
    {
      "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
      "description": "description",
      "groupId": 222,
      "links": [
        {
          "href": "href",
          "rel": "rel",
          "templated": true
        }
      ],
      "name": "name",
      "updateDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
      "valid": true
    }
  ],
  "lastName": "lastName",
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "mobile": "mobile",
  "mobileInvalid": true,
  "mobileOptout": true,
  "modificationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "other": "other",
  "phone": "phone",
  "title": "title",
  "valid": true,
  "vatNumber": "vatNumber"
}
``` 

#### Responses
**201** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="delete_using_delete_1"></a>![Endpoint: ](https://apidocs.io/img/method.png "deleteUsingDELETE_1") deleteUsingDELETE_1


**`DELETE`** `/contacts/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> Delete a contact




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | number |  ``` Required ```  | id | `222` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**204** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden


### <a name="add_group_using_post"></a>![Endpoint: ](https://apidocs.io/img/method.png "addGroupUsingPOST") addGroupUsingPOST


**`POST`** `/contacts/{id}/group/{groupId}`

> *Tags:*  ``` Skips Authentication ``` 

> Add a contact in a group




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | number |  ``` Required ```  | id | `222` | 
| groupId | number |  ``` Required ```  | groupId | `222` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**201** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="groups_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "groupsUsingGET") groupsUsingGET


**`GET`** `/contacts/{id}/groups/pages/{page}`

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups for a contact




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | number |  ``` Required ```  | id | `222` | 
| page | number |  ``` Required ```  | page | `222` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `222` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="delete_group_using_delete"></a>![Endpoint: ](https://apidocs.io/img/method.png "deleteGroupUsingDELETE") deleteGroupUsingDELETE


**`DELETE`** `/contacts/{id}/groups/{groupId}`

> *Tags:*  ``` Skips Authentication ``` 

> Remove a contact from a group




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | number |  ``` Required ```  | id | `222` | 
| groupId | number |  ``` Required ```  | groupId | `222` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**204** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden


[Back to API Reference](#api_reference)

## <a name="customer_controller"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "customer-controller") customer-controller


### <a name="get_using_get_2"></a>![Endpoint: ](https://apidocs.io/img/method.png "getUsingGET_2") getUsingGET_2


**`GET`** `/account`

> *Tags:*  ``` Skips Authentication ``` 

> Show your account




#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[CustomerResource](#customer_resource)**) 

```
{
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "credit": 180.772152808854,
  "creditThreshold": 180,
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "name": "name"
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="get_from_fields_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "getFromFieldsUsingGET") getFromFieldsUsingGET


**`GET`** `/account/senders`

> *Tags:*  ``` Skips Authentication ``` 

> Get your personnalized sender IDs




#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="delete_sender_using_put"></a>![Endpoint: ](https://apidocs.io/img/method.png "deleteSenderUsingPUT") deleteSenderUsingPUT


**`PUT`** `/account/senders`

> *Tags:*  ``` Skips Authentication ``` 

> Remove sender ID




#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| string |  ``` Required ```  | senderID | 

 *Example Body* 
``` 
"senderID"
``` 

#### Responses
**201** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="add_sender_using_post"></a>![Endpoint: ](https://apidocs.io/img/method.png "addSenderUsingPOST") addSenderUsingPOST


**`POST`** `/account/senders`

> *Tags:*  ``` Skips Authentication ``` 

> Add personnalized sender ID




#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| string |  ``` Required ```  | senderID | 

 *Example Body* 
``` 
"senderID"
``` 

#### Responses
**201** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="list_using_get_3"></a>![Endpoint: ](https://apidocs.io/img/method.png "listUsingGET_3") listUsingGET_3


**`GET`** `/account/subaccounts`

> *Tags:*  ``` Skips Authentication ``` 

> View a list of your subaccounts




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="list_page_using_get_3"></a>![Endpoint: ](https://apidocs.io/img/method.png "listPageUsingGET_3") listPageUsingGET_3


**`GET`** `/account/subaccounts/pages/{page}`

> *Tags:*  ``` Skips Authentication ``` 

> View a list of your subaccounts by page




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| page | number |  ``` Required ```  | page | `180` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


[Back to API Reference](#api_reference)

## <a name="group_controller"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "group-controller") group-controller


### <a name="list_using_get_4"></a>![Endpoint: ](https://apidocs.io/img/method.png "listUsingGET_4") listUsingGET_4


**`GET`** `/groups`

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="add_using_post_2"></a>![Endpoint: ](https://apidocs.io/img/method.png "addUsingPOST_2") addUsingPOST_2


**`POST`** `/groups`

> *Tags:*  ``` Skips Authentication ``` 

> Add a group




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [GroupResource](#group_resource) |  ``` Required ```  | resource | 

 *Example Body* 
``` 
{
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "description": "description",
  "groupId": 180,
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "name": "name",
  "updateDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "valid": true
}
``` 

#### Responses
**201** 

> OK


 *Example Body* (**[GroupResource](#group_resource)**) 

```
{
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "description": "description",
  "groupId": 180,
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "name": "name",
  "updateDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "valid": true
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="delete_list_using_post_1"></a>![Endpoint: ](https://apidocs.io/img/method.png "deleteListUsingPOST_1") deleteListUsingPOST_1


**`POST`** `/groups/delete`

> *Tags:*  ``` Skips Authentication ``` 

> Delete a list of groups




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| number |  ``` Required ```  ``` Collection ```  | idList | 

 *Example Body* 
``` 
[
  180
]
``` 

#### Responses
**201** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="list_page_using_get_4"></a>![Endpoint: ](https://apidocs.io/img/method.png "listPageUsingGET_4") listPageUsingGET_4


**`GET`** `/groups/pages/{page}`

> *Tags:*  ``` Skips Authentication ``` 

> listPage




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| page | number |  ``` Required ```  | page | `180` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="search_using_get_2"></a>![Endpoint: ](https://apidocs.io/img/method.png "searchUsingGET_2") searchUsingGET_2


**`GET`** `/groups/search/{name}`

> *Tags:*  ``` Skips Authentication ``` 

> search




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| name | string |  ``` Required ```  | name | `"name"` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="get_using_get_4"></a>![Endpoint: ](https://apidocs.io/img/method.png "getUsingGET_4") getUsingGET_4


**`GET`** `/groups/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> Show a group




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | number |  ``` Required ```  | id | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[GroupResource](#group_resource)**) 

```
{
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "description": "description",
  "groupId": 180,
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "name": "name",
  "updateDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "valid": true
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="update_using_put_2"></a>![Endpoint: ](https://apidocs.io/img/method.png "updateUsingPUT_2") updateUsingPUT_2


**`PUT`** `/groups/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> Update a group




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | number |  ``` Required ```  | id | `180` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [GroupResource](#group_resource) |  ``` Required ```  | resource | 

 *Example Body* 
``` 
{
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "description": "description",
  "groupId": 180,
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "name": "name",
  "updateDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "valid": true
}
``` 

#### Responses
**201** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="delete_using_delete_3"></a>![Endpoint: ](https://apidocs.io/img/method.png "deleteUsingDELETE_3") deleteUsingDELETE_3


**`DELETE`** `/groups/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> Delete a group




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | number |  ``` Required ```  | id | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**204** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden


### <a name="contacts_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "contactsUsingGET") contactsUsingGET


**`GET`** `/groups/{id}/contacts/pages/{page}`

> *Tags:*  ``` Skips Authentication ``` 

> Show a list of contacts for a group




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | number |  ``` Required ```  | id | `180` | 
| page | number |  ``` Required ```  | page | `180` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[GroupResource](#group_resource)**) 

```
{
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "description": "description",
  "groupId": 180,
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "name": "name",
  "updateDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "valid": true
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


[Back to API Reference](#api_reference)

## <a name="campaign_controller"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "campaign-controller") campaign-controller


### <a name="list_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "listUsingGET") listUsingGET


**`GET`** `/campaigns`

> *Tags:*  ``` Skips Authentication ``` 

> list




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="send_to_list_using_post"></a>![Endpoint: ](https://apidocs.io/img/method.png "sendToListUsingPOST") sendToListUsingPOST


**`POST`** `/campaigns`

> *Tags:*  ``` Skips Authentication ``` 

> sendToList




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CampaignInputResource](#campaign_input_resource) |  ``` Required ```  | resource | 

 *Example Body* 
``` 
{
  "campaignName": "campaignName",
  "contactIdLst": [
    180
  ],
  "fromField": "fromField",
  "groupIdLst": [
    180
  ],
  "numeroLst": [
    "numeroLst"
  ],
  "sendDate": "2017-11-03T13:01:11.8891147Z",
  "text": "text"
}
``` 

#### Responses
**201** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="list_page_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "listPageUsingGET") listPageUsingGET


**`GET`** `/campaigns/pages/{page}`

> *Tags:*  ``` Skips Authentication ``` 

> listPage




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| page | number |  ``` Required ```  | page | `180` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="search_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "searchUsingGET") searchUsingGET


**`GET`** `/campaigns/search/{name}`

> *Tags:*  ``` Skips Authentication ``` 

> search




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| name | string |  ``` Required ```  | name | `"name"` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="delete_using_delete"></a>![Endpoint: ](https://apidocs.io/img/method.png "deleteUsingDELETE") deleteUsingDELETE


**`DELETE`** `/campaigns/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> delete




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | string |  ``` Required ```  | TODO: Add a parameter description | `"id"` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| messsageId | string |  ``` Required ```  | messsageId | `"messsageId"` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**204** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden


[Back to API Reference](#api_reference)

## <a name="transfer_controller"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "transfer-controller") transfer-controller


### <a name="list_using_get_9"></a>![Endpoint: ](https://apidocs.io/img/method.png "listUsingGET_9") listUsingGET_9


**`GET`** `/transfers`

> *Tags:*  ``` Skips Authentication ``` 

> View a list of transferts




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="list_page_using_get_9"></a>![Endpoint: ](https://apidocs.io/img/method.png "listPageUsingGET_9") listPageUsingGET_9


**`GET`** `/transfers/pages/{page}`

> *Tags:*  ``` Skips Authentication ``` 

> listPage




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| page | number |  ``` Required ```  | page | `180` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="get_using_get_9"></a>![Endpoint: ](https://apidocs.io/img/method.png "getUsingGET_9") getUsingGET_9


**`GET`** `/transfers/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> Show a transfet




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | number |  ``` Required ```  | id | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[TransferResource](#transfer_resource)**) 

```
{
  "amount": 180.772152808854,
  "creationDate": "2017-11-03T13:01:11.8891147Z",
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "messageCredit": 180.772152808854,
  "reference": "reference",
  "transactionAmount": 180.772152808854,
  "transactionStatus": "transactionStatus",
  "transactionType": "transactionType",
  "transferId": 180
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


[Back to API Reference](#api_reference)

## <a name="email_api_configuration_controller"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "email-api-configuration-controller") email-api-configuration-controller


### <a name="get_using_get_3"></a>![Endpoint: ](https://apidocs.io/img/method.png "getUsingGET_3") getUsingGET_3


**`GET`** `/configuration/email`

> *Tags:*  ``` Skips Authentication ``` 

> Show your configuration




#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[EmailAPIConfigurationResource](#email_api_configuration_resource)**) 

```
{
  "emailDomainList": {},
  "emailList": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "secureIpAddressList": {},
  "sender": "sender",
  "useEmailSubject": true,
  "useUnicode": true
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="update_using_put_1"></a>![Endpoint: ](https://apidocs.io/img/method.png "updateUsingPUT_1") updateUsingPUT_1


**`PUT`** `/configuration/email`

> *Tags:*  ``` Skips Authentication ``` 

> Update your configuration




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [EmailAPIConfigurationResource](#email_api_configuration_resource) |  ``` Required ```  | resource | 

 *Example Body* 
``` 
{
  "emailDomainList": {},
  "emailList": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "secureIpAddressList": {},
  "sender": "sender",
  "useEmailSubject": true,
  "useUnicode": true
}
``` 

#### Responses
**201** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="add_using_post_1"></a>![Endpoint: ](https://apidocs.io/img/method.png "addUsingPOST_1") addUsingPOST_1


**`POST`** `/configuration/email`

> *Tags:*  ``` Skips Authentication ``` 

> Create your configuration




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [EmailAPIConfigurationResource](#email_api_configuration_resource) |  ``` Required ```  | resource | 

 *Example Body* 
``` 
{
  "emailDomainList": {},
  "emailList": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "secureIpAddressList": {},
  "sender": "sender",
  "useEmailSubject": true,
  "useUnicode": true
}
``` 

#### Responses
**201** 

> OK


 *Example Body* (**[EmailAPIConfigurationResource](#email_api_configuration_resource)**) 

```
{
  "emailDomainList": {},
  "emailList": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "secureIpAddressList": {},
  "sender": "sender",
  "useEmailSubject": true,
  "useUnicode": true
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="delete_using_delete_2"></a>![Endpoint: ](https://apidocs.io/img/method.png "deleteUsingDELETE_2") deleteUsingDELETE_2


**`DELETE`** `/configuration/email`

> *Tags:*  ``` Skips Authentication ``` 

> Delete your configuration




#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**204** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden


[Back to API Reference](#api_reference)

## <a name="message_controller"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "message-controller") message-controller


### <a name="list_using_get_6"></a>![Endpoint: ](https://apidocs.io/img/method.png "listUsingGET_6") listUsingGET_6


**`GET`** `/sms`

> *Tags:*  ``` Skips Authentication ``` 

> list




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="list_page_using_get_6"></a>![Endpoint: ](https://apidocs.io/img/method.png "listPageUsingGET_6") listPageUsingGET_6


**`GET`** `/sms/pages/{page}`

> *Tags:*  ``` Skips Authentication ``` 

> listPage




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| page | number |  ``` Required ```  | page | `180` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[PagedResources«MessageResource»](#paged_resources«message_resource»)**) 

```
{
  "content": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "page": {
    "number": 180,
    "size": 180,
    "totalElements": 180,
    "totalPages": 180
  }
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="list_responses_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "listResponsesUsingGET") listResponsesUsingGET


**`GET`** `/sms/responses`

> *Tags:*  ``` Skips Authentication ``` 

> listResponses




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[Resources«MessageResource»](#resources«message_resource»)**) 

```
{
  "content": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ]
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="list_responses_page_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "listResponsesPageUsingGET") listResponsesPageUsingGET


**`GET`** `/sms/responses/pages/{page}`

> *Tags:*  ``` Skips Authentication ``` 

> listResponsesPage




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| page | number |  ``` Required ```  | page | `180` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[PagedResources«MessageResource»](#paged_resources«message_resource»)**) 

```
{
  "content": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "page": {
    "number": 180,
    "size": 180,
    "totalElements": 180,
    "totalPages": 180
  }
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="list_scheduled_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "listScheduledUsingGET") listScheduledUsingGET


**`GET`** `/sms/scheduled`

> *Tags:*  ``` Skips Authentication ``` 

> listScheduled




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[Resources«MessageResource»](#resources«message_resource»)**) 

```
{
  "content": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ]
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="list_scheduled_page_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "listScheduledPageUsingGET") listScheduledPageUsingGET


**`GET`** `/sms/scheduled/pages/{page}`

> *Tags:*  ``` Skips Authentication ``` 

> listScheduledPage




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| page | number |  ``` Required ```  | page | `180` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[PagedResources«MessageResource»](#paged_resources«message_resource»)**) 

```
{
  "content": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "page": {
    "number": 180,
    "size": 180,
    "totalElements": 180,
    "totalPages": 180
  }
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="search_using_get_3"></a>![Endpoint: ](https://apidocs.io/img/method.png "searchUsingGET_3") searchUsingGET_3


**`GET`** `/sms/search/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> search




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | string |  ``` Required ```  | id | `"id"` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `180` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="send_to_list_using_post_1"></a>![Endpoint: ](https://apidocs.io/img/method.png "sendToListUsingPOST_1") sendToListUsingPOST_1


**`POST`** `/sms/send`

> *Tags:*  ``` Skips Authentication ``` 

> sendToList




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [MessageInputMixedResource](#message_input_mixed_resource) |  ``` Required ```  | resource | 

 *Example Body* 
``` 
{
  "contactIdLst": [
    180
  ],
  "fromField": "fromField",
  "groupIdLst": [
    180
  ],
  "numeroLst": [
    "numeroLst"
  ],
  "sendDate": "2017-11-03T13:01:11.8891147Z",
  "text": "text"
}
``` 

#### Responses
**201** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="send_to_contact_list_using_post"></a>![Endpoint: ](https://apidocs.io/img/method.png "sendToContactListUsingPOST") sendToContactListUsingPOST


**`POST`** `/sms/send/contacts`

> *Tags:*  ``` Skips Authentication ``` 

> sendToContactList




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [MessageInputContactResource](#message_input_contact_resource) |  ``` Required ```  | resource | 

 *Example Body* 
``` 
{
  "contactIdLst": [
    180
  ],
  "fromField": "fromField",
  "sendDate": "2017-11-03T13:01:11.8891147Z",
  "text": "text"
}
``` 

#### Responses
**201** 

> OK



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="send_to_group_list_using_post"></a>![Endpoint: ](https://apidocs.io/img/method.png "sendToGroupListUsingPOST") sendToGroupListUsingPOST


**`POST`** `/sms/send/groups`

> *Tags:*  ``` Skips Authentication ``` 

> sendToGroupList




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [MessageInputGroupResource](#message_input_group_resource) |  ``` Required ```  | resource | 

 *Example Body* 
``` 
{
  "fromField": "fromField",
  "groupIdLst": [
    180
  ],
  "sendDate": "2017-11-03T13:01:11.8891147Z",
  "text": "text"
}
``` 

#### Responses
**201** 

> OK



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="send_to_number_list_using_post"></a>![Endpoint: ](https://apidocs.io/img/method.png "sendToNumberListUsingPOST") sendToNumberListUsingPOST


**`POST`** `/sms/send/list`

> *Tags:*  ``` Skips Authentication ``` 

> sendToNumberList




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [MessageInputResource](#message_input_resource) |  ``` Required ```  | resource | 

 *Example Body* 
``` 
{
  "fromField": "fromField",
  "numeroLst": [
    "numeroLst"
  ],
  "sendDate": "2017-11-03T13:01:11.9047393Z",
  "text": "text"
}
``` 

#### Responses
**201** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="delete_using_delete_4"></a>![Endpoint: ](https://apidocs.io/img/method.png "deleteUsingDELETE_4") deleteUsingDELETE_4


**`DELETE`** `/sms/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> delete




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | string |  ``` Required ```  | TODO: Add a parameter description | `"id"` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| messsageId | string |  ``` Required ```  | messsageId | `"messsageId"` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**204** 

> OK



**401** 

> Unauthorized

**403** 

> Forbidden


[Back to API Reference](#api_reference)

## <a name="register_controler"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "register-controler") register-controler


### <a name="register_using_post"></a>![Endpoint: ](https://apidocs.io/img/method.png "registerUsingPOST") registerUsingPOST


**`POST`** `/register`

> *Tags:*  ``` Skips Authentication ``` 

> register




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [RegisterResource](#register_resource) |  ``` Required ```  | resource | 

 *Example Body* 
``` 
{
  "email": "email",
  "login": "login",
  "password": "password"
}
``` 

#### Responses
**201** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="refresh_using_post"></a>![Endpoint: ](https://apidocs.io/img/method.png "refreshUsingPOST") refreshUsingPOST


**`POST`** `/register/refresh`

> *Tags:*  ``` Skips Authentication ``` 

> refresh




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [SimpleEmailResource](#simple_email_resource) |  ``` Required ```  | resource | 

 *Example Body* 
``` 
{
  "email": "email"
}
``` 

#### Responses
**201** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="activate_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "activateUsingGET") activateUsingGET


**`GET`** `/register/{token}/client/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> activate




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| token | string |  ``` Required ```  | token | `"token"` | 
| id | number |  ``` Required ```  | id | `17` | 

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


[Back to API Reference](#api_reference)

## <a name="credit_consumption_controller"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "credit-consumption-controller") credit-consumption-controller


### <a name="list_using_get_2"></a>![Endpoint: ](https://apidocs.io/img/method.png "listUsingGET_2") listUsingGET_2


**`GET`** `/consumption`

> *Tags:*  ``` Skips Authentication ``` 

> Get the consumption of the last months




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `17` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="list_page_using_get_2"></a>![Endpoint: ](https://apidocs.io/img/method.png "listPageUsingGET_2") listPageUsingGET_2


**`GET`** `/consumption/pages/{page}`

> *Tags:*  ``` Skips Authentication ``` 

> Get pageable consumption of the last months




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| page | number |  ``` Required ```  | page | `17` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `17` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="get_using_get_1"></a>![Endpoint: ](https://apidocs.io/img/method.png "getUsingGET_1") getUsingGET_1


**`GET`** `/consumption/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> Get specific consumption by id 




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | number |  ``` Required ```  | id | `17` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


[Back to API Reference](#api_reference)

## <a name="pricing_controller"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "pricing-controller") pricing-controller


### <a name="get_using_get_7"></a>![Endpoint: ](https://apidocs.io/img/method.png "getUsingGET_7") getUsingGET_7


**`GET`** `/pricing`

> *Tags:*  ``` Skips Authentication ``` 

> get




#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[PricingResource](#pricing_resource)**) 

```
{
  "pricing": [
    {
      "count": 17,
      "priceHT": 17.2674347005167,
      "priceTTC": 17.2674347005167,
      "unitPriceHT": 17.2674347005167,
      "unitPriceTTC": 17.2674347005167
    }
  ],
  "vatRate": 17.2674347005167
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


[Back to API Reference](#api_reference)

## <a name="message_model_controller"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "message-model-controller") message-model-controller


### <a name="list_using_get_7"></a>![Endpoint: ](https://apidocs.io/img/method.png "listUsingGET_7") listUsingGET_7


**`GET`** `/models`

> *Tags:*  ``` Skips Authentication ``` 

> list




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| size | number |  ``` Optional ```  | size | `17` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[Resources«MessageModelResource»](#resources«message_model_resource»)**) 

```
{
  "content": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": false
    }
  ]
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="add_using_post_3"></a>![Endpoint: ](https://apidocs.io/img/method.png "addUsingPOST_3") addUsingPOST_3


**`POST`** `/models`

> *Tags:*  ``` Skips Authentication ``` 

> add




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [MessageModelInputResource](#message_model_input_resource) |  ``` Required ```  | resource | 

 *Example Body* 
``` 
{
  "fromField": "fromField",
  "text": "text",
  "titre": "titre"
}
``` 

#### Responses
**201** 

> OK


 *Example Body* (**[MessageModelResource](#message_model_resource)**) 

```
{
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "fromField": "fromField",
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": false
    }
  ],
  "modelId": "modelId",
  "text": "text",
  "titre": "titre"
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="delete_multiple_using_post"></a>![Endpoint: ](https://apidocs.io/img/method.png "deleteMultipleUsingPOST") deleteMultipleUsingPOST


**`POST`** `/models/delete`

> *Tags:*  ``` Skips Authentication ``` 

> deleteMultiple




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| string |  ``` Required ```  ``` Collection ```  | ids | 

 *Example Body* 
``` 
[
  "ids"
]
``` 

#### Responses
**201** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="list_page_using_get_7"></a>![Endpoint: ](https://apidocs.io/img/method.png "listPageUsingGET_7") listPageUsingGET_7


**`GET`** `/models/pages/{page}`

> *Tags:*  ``` Skips Authentication ``` 

> listPage




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| page | number |  ``` Required ```  | page | `17` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| limit | number |  ``` Optional ```  | limit | `17` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[PagedResources«MessageModelResource»](#paged_resources«message_model_resource»)**) 

```
{
  "content": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": false
    }
  ],
  "page": {
    "number": 17,
    "size": 17,
    "totalElements": 17,
    "totalPages": 17
  }
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="get_using_get_6"></a>![Endpoint: ](https://apidocs.io/img/method.png "getUsingGET_6") getUsingGET_6


**`GET`** `/models/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> get




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | string |  ``` Required ```  | id | `"id"` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**200** 

> OK


 *Example Body* (**[MessageModelResource](#message_model_resource)**) 

```
{
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "fromField": "fromField",
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": false
    }
  ],
  "modelId": "modelId",
  "text": "text",
  "titre": "titre"
}
```


**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="update_using_put_3"></a>![Endpoint: ](https://apidocs.io/img/method.png "updateUsingPUT_3") updateUsingPUT_3


**`PUT`** `/models/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> update




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | string |  ``` Required ```  | id | `"id"` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;
>X-Auth-Token="X-Auth-Token";

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [MessageModelInputResource](#message_model_input_resource) |  ``` Required ```  | resource | 

 *Example Body* 
``` 
{
  "fromField": "fromField",
  "text": "text",
  "titre": "titre"
}
``` 

#### Responses
**201** 

> OK



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="delete_using_delete_5"></a>![Endpoint: ](https://apidocs.io/img/method.png "deleteUsingDELETE_5") deleteUsingDELETE_5


**`DELETE`** `/models/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> delete




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | string |  ``` Required ```  | id | `"id"` | 

#### Request Headers
>X-Auth-Token="X-Auth-Token";

#### Responses
**204** 

> OK



**401** 

> Unauthorized

**403** 

> Forbidden


[Back to API Reference](#api_reference)

## <a name="societe_info_controller"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "societe-info-controller") societe-info-controller


### <a name="research_company_using_post"></a>![Endpoint: ](https://apidocs.io/img/method.png "researchCompanyUsingPOST") researchCompanyUsingPOST


**`POST`** `/company`

> *Tags:*  ``` Skips Authentication ``` 

> researchCompany




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [SocieteInfoResearchResource](#societe_info_research_resource) |  ``` Required ```  | research | 

 *Example Body* 
``` 
{
  "city": "city",
  "name": "name",
  "page": 17,
  "totalPages": 17
}
``` 

#### Responses
**201** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


### <a name="get_details_using_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "getDetailsUsingGET") getDetailsUsingGET


**`GET`** `/company/detail/{id}`

> *Tags:*  ``` Skips Authentication ``` 

> getDetails




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| id | string |  ``` Required ```  | id | `"id"` | 

#### Responses
**200** 

> OK


 *Example Body* (**dynamic**) 



**401** 

> Unauthorized

**403** 

> Forbidden

**404** 

> Not Found


[Back to API Reference](#api_reference)

# <a name="models"></a> Models

### List of Models

* [PagedResources«MessageResource»](#paged_resources«message_resource»)
* [MessageResource](#message_resource)
* [CustomerResource](#customer_resource)
* [Resources«ContactResource»](#resources«contact_resource»)
* [MessageInputContactResource](#message_input_contact_resource)
* [SimpleEmailResource](#simple_email_resource)
* [EmailAPIConfigurationResource](#email_api_configuration_resource)
* [MessageInputResource](#message_input_resource)
* [DeferredResult«ResponseEntity«object»»](#deferred_result«response_entity«object»»)
* [Resources«MessageModelResource»](#resources«message_model_resource»)
* [PricingResource](#pricing_resource)
* [CreditPacksResource](#credit_packs_resource)
* [MessageInputMixedResource](#message_input_mixed_resource)
* [PagedResources«MessageModelResource»](#paged_resources«message_model_resource»)
* [Resources«MessageResource»](#resources«message_resource»)
* [AddressResource](#address_resource)
* [GroupResource](#group_resource)
* [RegisterResource](#register_resource)
* [MessageModelInputResource](#message_model_input_resource)
* [MessageModelResource](#message_model_resource)
* [ContactResource](#contact_resource)
* [PageMetadata](#page_metadata)
* [AuthenticationResource](#authentication_resource)
* [SocieteInfoResearchResource](#societe_info_research_resource)
* [MessageInputGroupResource](#message_input_group_resource)
* [Link](#link)
* [TokenResource](#token_resource)
* [TransferResource](#transfer_resource)
* [InvoiceResource](#invoice_resource)
* [CampaignInputResource](#campaign_input_resource)
* [AccessChannel](#access_channel)
## <a name="paged_resources«message_resource»"></a>![Type: ](https://apidocs.io/img/method.png "PagedResources«MessageResource»") PagedResources«MessageResource»



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| content | object |  ``` Optional ```  | TODO: Add a property description | 
| links | [Link](#link) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| page | [PageMetadata](#page_metadata) |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "content": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": false
    }
  ],
  "page": {
    "number": 39,
    "size": 39,
    "totalElements": 39,
    "totalPages": 39
  }
}
```



## <a name="message_resource"></a>![Type: ](https://apidocs.io/img/method.png "MessageResource") MessageResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| accessChannel | [AccessChannel](#access_channel) |  ``` Optional ```  | TODO: Add a property description | 
| campaignName | string |  ``` Optional ```  | TODO: Add a property description | 
| clientReference | string |  ``` Optional ```  | TODO: Add a property description | 
| cost | string |  ``` Optional ```  | TODO: Add a property description | 
| creationDate | string |  ``` Optional ```  | TODO: Add a property description | 
| from | string |  ``` Optional ```  | TODO: Add a property description | 
| groups | string |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| idMessage | string |  ``` Optional ```  | TODO: Add a property description | 
| links | [Link](#link) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| recipientCount | number |  ``` Optional ```  | TODO: Add a property description | 
| recipients | string |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| sentDate | string |  ``` Optional ```  | TODO: Add a property description | 
| text | string |  ``` Optional ```  | TODO: Add a property description | 
| type | string |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "accessChannel": "UNKNOWN",
  "campaignName": "campaignName",
  "clientReference": "clientReference",
  "cost": "cost",
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "from": "from",
  "groups": [
    "groups"
  ],
  "idMessage": "idMessage",
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": false
    }
  ],
  "recipientCount": 39,
  "recipients": [
    "recipients"
  ],
  "sentDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "text": "text",
  "type": "type"
}
```



## <a name="customer_resource"></a>![Type: ](https://apidocs.io/img/method.png "CustomerResource") CustomerResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| creationDate | string |  ``` Optional ```  | TODO: Add a property description | 
| credit | precision |  ``` Optional ```  | TODO: Add a property description | 
| creditThreshold | number |  ``` Optional ```  | TODO: Add a property description | 
| links | [Link](#link) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| name | string |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "credit": 39.5047622520964,
  "creditThreshold": 39,
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": false
    }
  ],
  "name": "name"
}
```



## <a name="resources«contact_resource»"></a>![Type: ](https://apidocs.io/img/method.png "Resources«ContactResource»") Resources«ContactResource»



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| content | object |  ``` Optional ```  | TODO: Add a property description | 
| links | [Link](#link) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 



#### Example
```
{
  "content": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": false
    }
  ]
}
```



## <a name="message_input_contact_resource"></a>![Type: ](https://apidocs.io/img/method.png "MessageInputContactResource") MessageInputContactResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| contactIdLst | number |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| fromField | string |  ``` Optional ```  | TODO: Add a property description | 
| sendDate | datetime |  ``` Optional ```  | TODO: Add a property description | 
| text | string |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "contactIdLst": [
    39
  ],
  "fromField": "fromField",
  "sendDate": "2017-11-03T13:01:11.8422432Z",
  "text": "text"
}
```



## <a name="simple_email_resource"></a>![Type: ](https://apidocs.io/img/method.png "SimpleEmailResource") SimpleEmailResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| email | string |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "email": "email"
}
```



## <a name="email_api_configuration_resource"></a>![Type: ](https://apidocs.io/img/method.png "EmailAPIConfigurationResource") EmailAPIConfigurationResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| emailDomainList | object |  ``` Optional ```  | TODO: Add a property description | 
| emailList | object |  ``` Optional ```  | TODO: Add a property description | 
| links | [Link](#link) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| secureIpAddressList | object |  ``` Optional ```  | TODO: Add a property description | 
| sender | string |  ``` Optional ```  | TODO: Add a property description | 
| useEmailSubject | boolean |  ``` Optional ```  | TODO: Add a property description | 
| useUnicode | boolean |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "emailDomainList": {},
  "emailList": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "secureIpAddressList": {},
  "sender": "sender",
  "useEmailSubject": true,
  "useUnicode": true
}
```



## <a name="message_input_resource"></a>![Type: ](https://apidocs.io/img/method.png "MessageInputResource") MessageInputResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| fromField | string |  ``` Optional ```  | TODO: Add a property description | 
| numeroLst | string |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| sendDate | datetime |  ``` Optional ```  | TODO: Add a property description | 
| text | string |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "fromField": "fromField",
  "numeroLst": [
    "numeroLst"
  ],
  "sendDate": "2017-11-03T13:01:11.8578627Z",
  "text": "text"
}
```



## <a name="deferred_result«response_entity«object»»"></a>![Type: ](https://apidocs.io/img/method.png "DeferredResult«ResponseEntity«object»»") DeferredResult«ResponseEntity«object»»



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| result | object |  ``` Optional ```  | TODO: Add a property description | 
| setOrExpired | boolean |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "result": {},
  "setOrExpired": true
}
```



## <a name="resources«message_model_resource»"></a>![Type: ](https://apidocs.io/img/method.png "Resources«MessageModelResource»") Resources«MessageModelResource»



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| content | object |  ``` Optional ```  | TODO: Add a property description | 
| links | [Link](#link) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 



#### Example
```
{
  "content": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ]
}
```



## <a name="pricing_resource"></a>![Type: ](https://apidocs.io/img/method.png "PricingResource") PricingResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| pricing | [CreditPacksResource](#credit_packs_resource) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| vatRate | precision |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "pricing": [
    {
      "count": 131,
      "priceHT": 131.000044143759,
      "priceTTC": 131.000044143759,
      "unitPriceHT": 131.000044143759,
      "unitPriceTTC": 131.000044143759
    }
  ],
  "vatRate": 131.000044143759
}
```



## <a name="credit_packs_resource"></a>![Type: ](https://apidocs.io/img/method.png "CreditPacksResource") CreditPacksResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| count | number |  ``` Optional ```  | TODO: Add a property description | 
| priceHT | precision |  ``` Optional ```  | TODO: Add a property description | 
| priceTTC | precision |  ``` Optional ```  | TODO: Add a property description | 
| unitPriceHT | precision |  ``` Optional ```  | TODO: Add a property description | 
| unitPriceTTC | precision |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "count": 131,
  "priceHT": 131.000044143759,
  "priceTTC": 131.000044143759,
  "unitPriceHT": 131.000044143759,
  "unitPriceTTC": 131.000044143759
}
```



## <a name="message_input_mixed_resource"></a>![Type: ](https://apidocs.io/img/method.png "MessageInputMixedResource") MessageInputMixedResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| contactIdLst | number |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| fromField | string |  ``` Optional ```  | TODO: Add a property description | 
| groupIdLst | number |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| numeroLst | string |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| sendDate | datetime |  ``` Optional ```  | TODO: Add a property description | 
| text | string |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "contactIdLst": [
    131
  ],
  "fromField": "fromField",
  "groupIdLst": [
    131
  ],
  "numeroLst": [
    "numeroLst"
  ],
  "sendDate": "2017-11-03T13:01:11.8578627Z",
  "text": "text"
}
```



## <a name="paged_resources«message_model_resource»"></a>![Type: ](https://apidocs.io/img/method.png "PagedResources«MessageModelResource»") PagedResources«MessageModelResource»



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| content | object |  ``` Optional ```  | TODO: Add a property description | 
| links | [Link](#link) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| page | [PageMetadata](#page_metadata) |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "content": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "page": {
    "number": 131,
    "size": 131,
    "totalElements": 131,
    "totalPages": 131
  }
}
```



## <a name="resources«message_resource»"></a>![Type: ](https://apidocs.io/img/method.png "Resources«MessageResource»") Resources«MessageResource»



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| content | object |  ``` Optional ```  | TODO: Add a property description | 
| links | [Link](#link) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 



#### Example
```
{
  "content": {},
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ]
}
```



## <a name="address_resource"></a>![Type: ](https://apidocs.io/img/method.png "AddressResource") AddressResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| address1 | string |  ``` Optional ```  | TODO: Add a property description | 
| address2 | string |  ``` Optional ```  | TODO: Add a property description | 
| city | string |  ``` Optional ```  | TODO: Add a property description | 
| country | string |  ``` Optional ```  | TODO: Add a property description | 
| links | [Link](#link) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| zipCode | string |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "address1": "address1",
  "address2": "address2",
  "city": "city",
  "country": "country",
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "zipCode": "zipCode"
}
```



## <a name="group_resource"></a>![Type: ](https://apidocs.io/img/method.png "GroupResource") GroupResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| creationDate | string |  ``` Optional ```  | TODO: Add a property description | 
| description | string |  ``` Optional ```  | TODO: Add a property description | 
| groupId | number |  ``` Optional ```  | TODO: Add a property description | 
| links | [Link](#link) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| name | string |  ``` Optional ```  | TODO: Add a property description | 
| updateDate | string |  ``` Optional ```  | TODO: Add a property description | 
| valid | boolean |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "description": "description",
  "groupId": 131,
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "name": "name",
  "updateDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "valid": true
}
```



## <a name="register_resource"></a>![Type: ](https://apidocs.io/img/method.png "RegisterResource") RegisterResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| email | string |  ``` Optional ```  | TODO: Add a property description | 
| login | string |  ``` Optional ```  | TODO: Add a property description | 
| password | string |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "email": "email",
  "login": "login",
  "password": "password"
}
```



## <a name="message_model_input_resource"></a>![Type: ](https://apidocs.io/img/method.png "MessageModelInputResource") MessageModelInputResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| fromField | string |  ``` Optional ```  | TODO: Add a property description | 
| text | string |  ``` Optional ```  | TODO: Add a property description | 
| titre | string |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "fromField": "fromField",
  "text": "text",
  "titre": "titre"
}
```



## <a name="message_model_resource"></a>![Type: ](https://apidocs.io/img/method.png "MessageModelResource") MessageModelResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| creationDate | string |  ``` Optional ```  | TODO: Add a property description | 
| fromField | string |  ``` Optional ```  | TODO: Add a property description | 
| links | [Link](#link) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| modelId | string |  ``` Optional ```  | TODO: Add a property description | 
| text | string |  ``` Optional ```  | TODO: Add a property description | 
| titre | string |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "fromField": "fromField",
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "modelId": "modelId",
  "text": "text",
  "titre": "titre"
}
```



## <a name="contact_resource"></a>![Type: ](https://apidocs.io/img/method.png "ContactResource") ContactResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| address | [AddressResource](#address_resource) |  ``` Optional ```  | TODO: Add a property description | 
| birthDate | string |  ``` Optional ```  | TODO: Add a property description | 
| company | string |  ``` Optional ```  | TODO: Add a property description | 
| contactId | number |  ``` Optional ```  | TODO: Add a property description | 
| creationDate | string |  ``` Optional ```  | TODO: Add a property description | 
| email | string |  ``` Optional ```  | TODO: Add a property description | 
| emailInvalid | boolean |  ``` Optional ```  | TODO: Add a property description | 
| emailOptout | boolean |  ``` Optional ```  | TODO: Add a property description | 
| fax | string |  ``` Optional ```  | TODO: Add a property description | 
| firstName | string |  ``` Optional ```  | TODO: Add a property description | 
| groups | [GroupResource](#group_resource) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| lastName | string |  ``` Optional ```  | TODO: Add a property description | 
| links | [Link](#link) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| mobile | string |  ``` Optional ```  | TODO: Add a property description | 
| mobileInvalid | boolean |  ``` Optional ```  | TODO: Add a property description | 
| mobileOptout | boolean |  ``` Optional ```  | TODO: Add a property description | 
| modificationDate | string |  ``` Optional ```  | TODO: Add a property description | 
| other | string |  ``` Optional ```  | TODO: Add a property description | 
| phone | string |  ``` Optional ```  | TODO: Add a property description | 
| title | string |  ``` Optional ```  | TODO: Add a property description | 
| valid | boolean |  ``` Optional ```  | TODO: Add a property description | 
| vatNumber | string |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "address": {
    "address1": "address1",
    "address2": "address2",
    "city": "city",
    "country": "country",
    "links": [
      {
        "href": "href",
        "rel": "rel",
        "templated": true
      }
    ],
    "zipCode": "zipCode"
  },
  "birthDate": "yyyy-MM-dd",
  "company": "company",
  "contactId": 131,
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "email": "email",
  "emailInvalid": true,
  "emailOptout": true,
  "fax": "fax",
  "firstName": "firstName",
  "groups": [
    {
      "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
      "description": "description",
      "groupId": 131,
      "links": [
        {
          "href": "href",
          "rel": "rel",
          "templated": true
        }
      ],
      "name": "name",
      "updateDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
      "valid": true
    }
  ],
  "lastName": "lastName",
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "mobile": "mobile",
  "mobileInvalid": true,
  "mobileOptout": true,
  "modificationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "other": "other",
  "phone": "phone",
  "title": "title",
  "valid": true,
  "vatNumber": "vatNumber"
}
```



## <a name="page_metadata"></a>![Type: ](https://apidocs.io/img/method.png "PageMetadata") PageMetadata



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| number | long |  ``` Optional ```  | TODO: Add a property description | 
| size | long |  ``` Optional ```  | TODO: Add a property description | 
| totalElements | long |  ``` Optional ```  | TODO: Add a property description | 
| totalPages | long |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "number": 131,
  "size": 131,
  "totalElements": 131,
  "totalPages": 131
}
```



## <a name="authentication_resource"></a>![Type: ](https://apidocs.io/img/method.png "AuthenticationResource") AuthenticationResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| login | string |  ``` Optional ```  | TODO: Add a property description | 
| password | string |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "login": "login",
  "password": "password"
}
```



## <a name="societe_info_research_resource"></a>![Type: ](https://apidocs.io/img/method.png "SocieteInfoResearchResource") SocieteInfoResearchResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| city | string |  ``` Optional ```  | TODO: Add a property description | 
| name | string |  ``` Optional ```  | TODO: Add a property description | 
| page | number |  ``` Optional ```  | TODO: Add a property description | 
| totalPages | number |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "city": "city",
  "name": "name",
  "page": 131,
  "totalPages": 131
}
```



## <a name="message_input_group_resource"></a>![Type: ](https://apidocs.io/img/method.png "MessageInputGroupResource") MessageInputGroupResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| fromField | string |  ``` Optional ```  | TODO: Add a property description | 
| groupIdLst | number |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| sendDate | datetime |  ``` Optional ```  | TODO: Add a property description | 
| text | string |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "fromField": "fromField",
  "groupIdLst": [
    131
  ],
  "sendDate": "2017-11-03T13:01:11.8578627Z",
  "text": "text"
}
```



## <a name="link"></a>![Type: ](https://apidocs.io/img/method.png "Link") Link



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| href | string |  ``` Optional ```  | TODO: Add a property description | 
| rel | string |  ``` Optional ```  | TODO: Add a property description | 
| templated | boolean |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "href": "href",
  "rel": "rel",
  "templated": true
}
```



## <a name="token_resource"></a>![Type: ](https://apidocs.io/img/method.png "TokenResource") TokenResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| creationDate | string |  ``` Optional ```  | TODO: Add a property description | 
| token | string |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "token": "token"
}
```



## <a name="transfer_resource"></a>![Type: ](https://apidocs.io/img/method.png "TransferResource") TransferResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| amount | precision |  ``` Optional ```  | TODO: Add a property description | 
| creationDate | datetime |  ``` Optional ```  | TODO: Add a property description | 
| links | [Link](#link) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| messageCredit | precision |  ``` Optional ```  | TODO: Add a property description | 
| reference | string |  ``` Optional ```  | TODO: Add a property description | 
| transactionAmount | precision |  ``` Optional ```  | TODO: Add a property description | 
| transactionStatus | string |  ``` Optional ```  | TODO: Add a property description | 
| transactionType | string |  ``` Optional ```  | TODO: Add a property description | 
| transferId | number |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "amount": 131.000044143759,
  "creationDate": "2017-11-03T13:01:11.8578627Z",
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "messageCredit": 131.000044143759,
  "reference": "reference",
  "transactionAmount": 131.000044143759,
  "transactionStatus": "transactionStatus",
  "transactionType": "transactionType",
  "transferId": 131
}
```



## <a name="invoice_resource"></a>![Type: ](https://apidocs.io/img/method.png "InvoiceResource") InvoiceResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| amount | precision |  ``` Optional ```  | TODO: Add a property description | 
| completionDate | string |  ``` Optional ```  | TODO: Add a property description | 
| creationDate | string |  ``` Optional ```  | TODO: Add a property description | 
| credit | precision |  ``` Optional ```  | TODO: Add a property description | 
| currency | string |  ``` Optional ```  | TODO: Add a property description | 
| invoiceId | number |  ``` Optional ```  | TODO: Add a property description | 
| links | [Link](#link) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| messageCredit | precision |  ``` Optional ```  | TODO: Add a property description | 
| reference | string |  ``` Optional ```  | TODO: Add a property description | 
| transactionStatus | string |  ``` Optional ```  | TODO: Add a property description | 
| transactionType | string |  ``` Optional ```  | TODO: Add a property description | 
| vatIncluded | boolean |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "amount": 131.000044143759,
  "completionDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "creationDate": "yyyy-MM-dd'T'HH:mm:ss'Z'",
  "credit": 131.000044143759,
  "currency": "currency",
  "invoiceId": 131,
  "links": [
    {
      "href": "href",
      "rel": "rel",
      "templated": true
    }
  ],
  "messageCredit": 131.000044143759,
  "reference": "reference",
  "transactionStatus": "transactionStatus",
  "transactionType": "transactionType",
  "vatIncluded": true
}
```



## <a name="campaign_input_resource"></a>![Type: ](https://apidocs.io/img/method.png "CampaignInputResource") CampaignInputResource



> TODO: Add a model description





| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| campaignName | string |  ``` Optional ```  | TODO: Add a property description | 
| contactIdLst | number |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| fromField | string |  ``` Optional ```  | TODO: Add a property description | 
| groupIdLst | number |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| numeroLst | string |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| sendDate | datetime |  ``` Optional ```  | TODO: Add a property description | 
| text | string |  ``` Optional ```  | TODO: Add a property description | 



#### Example
```
{
  "campaignName": "campaignName",
  "contactIdLst": [
    131
  ],
  "fromField": "fromField",
  "groupIdLst": [
    131
  ],
  "numeroLst": [
    "numeroLst"
  ],
  "sendDate": "2017-11-03T13:01:11.8578627Z",
  "text": "text"
}
```



## <a name="access_channel"></a>![Type: ](https://apidocs.io/img/method.png "AccessChannel") AccessChannel



> TODO: Add a model description





This type must take a value from the following `string` enumeration of values:

| Name | Value | Description |
| ---- | ----- | ----------- |
| UNKNOWN | `UNKNOWN` | TODO: Add description | 
| HTTP_1_0 | `HTTP_1_0` | TODO: Add description | 
| HTTP_1_5 | `HTTP_1_5` | TODO: Add description | 
| HTTP_1_6 | `HTTP_1_6` | TODO: Add description | 
| HTTP_BATCH_1_6 | `HTTP_BATCH_1_6` | TODO: Add description | 
| HTTP_2_0 | `HTTP_2_0` | TODO: Add description | 
| REST_1_0 | `REST_1_0` | TODO: Add description | 
| UI | `UI` | TODO: Add description | 
| MOBILE_UI | `MOBILE_UI` | TODO: Add description | 
| OMS_OUTLOOK_1_0 | `OMS_OUTLOOK_1_0` | TODO: Add description | 
| EMAIL_2_SMS_1_0 | `EMAIL_2_SMS_1_0` | TODO: Add description | 
| EMAIL_2_SMS_2_0 | `EMAIL_2_SMS_2_0` | TODO: Add description | 
| ORANGE_API_1_0 | `ORANGE_API_1_0` | TODO: Add description | 
| APP_ANDROID_1_0 | `APP_ANDROID_1_0` | TODO: Add description | 
| APP_IPHONE_1_0 | `APP_IPHONE_1_0` | TODO: Add description | 
| SMPP | `SMPP` | TODO: Add description | 
| GOOGLE_CALENDAR | `GOOGLE_CALENDAR` | TODO: Add description | 
| EMAIL_2_SMS_BATCH_1_0 | `EMAIL_2_SMS_BATCH_1_0` | TODO: Add description | 



#### Example
```
UNKNOWN
```




