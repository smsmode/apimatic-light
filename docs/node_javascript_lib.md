# Getting started

sMsMode API-REST Documentation

## How to Build

The generated SDK relies on [Node Package Manager](https://www.npmjs.com/) (NPM) being available to resolve dependencies. If you don't already have NPM installed, please go ahead and follow instructions to install NPM from [here](https://nodejs.org/en/download/).
The SDK also requires Node to be installed. If Node isn't already installed, please install it from [here](https://nodejs.org/en/download/)
> NPM is installed by default when Node is installed

To check if node and npm have been successfully installed, write the following commands in command prompt:

* `node --version`
* `npm -version`

![Version Check](https://apidocs.io/illustration/nodejs?step=versionCheck&workspaceFolder=sMsmode%20API-REST-Node)

Now use npm to resolve all dependencies by running the following command in the root directory (of the SDK folder):

```bash
npm install
```

![Resolve Dependencies](https://apidocs.io/illustration/nodejs?step=resolveDependency1&workspaceFolder=sMsmode%20API-REST-Node)

![Resolve Dependencies](https://apidocs.io/illustration/nodejs?step=resolveDependency2)

This will install all dependencies in the `node_modules` folder.

Once dependencies are resolved, you will need to move the folder `SMsmodeAPIRESTLib ` in to your `node_modules` folder.

## How to Use

The following section explains how to use the library in a new project.

### 1. Open Project Folder
Open an IDE/Text Editor for JavaScript like Sublime Text. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.

Click on `File` and select `Open Folder`.

![Open Folder](https://apidocs.io/illustration/nodejs?step=openFolder)

Select the folder of your SDK and click on `Select Folder` to open it up in Sublime Text. The folder will become visible in the bar on the left.

![Open Project](https://apidocs.io/illustration/nodejs?step=openProject&workspaceFolder=sMsmode%20API-REST-Node)

### 2. Creating a Test File

Now right click on the folder name and select the `New File` option to create a new test file. Save it as `index.js` Now import the generated NodeJS library using the following lines of code:

```js
var lib = require('lib');
```

Save changes.

![Create new file](https://apidocs.io/illustration/nodejs?step=createNewFile&workspaceFolder=sMsmode%20API-REST-Node)

![Save new file](https://apidocs.io/illustration/nodejs?step=saveNewFile&workspaceFolder=sMsmode%20API-REST-Node)

### 3. Running The Test File

To run the `index.js` file, open up the command prompt and navigate to the Path where the SDK folder resides. Type the following command to run the file:

```
node index.js
```

![Run file](https://apidocs.io/illustration/nodejs?step=runProject&workspaceFolder=sMsmode%20API-REST-Node)


## How to Test

These tests use Mocha framework for testing, coupled with Chai for assertions. These dependencies need to be installed for tests to run.
Tests can be run in a number of ways:

### Method 1 (Run all tests)

1. Navigate to the root directory of the SDK folder from command prompt.
2. Type `mocha --recursive` to run all the tests.

### Method 2 (Run all tests)

1. Navigate to the `../test/Controllers/` directory from command prompt.
2. Type `mocha *` to run all the tests.

### Method 3 (Run specific controller's tests)

1. Navigate to the `../test/Controllers/` directory from command prompt.
2. Type `mocha  sMsmode API-RESTController`  to run all the tests in that controller file.

> To increase mocha's default timeout, you can change the `TEST_TIMEOUT` parameter's value in `TestBootstrap.js`.

![Run Tests](https://apidocs.io/illustration/nodejs?step=runTests&controllerName=sMsmode%20API-RESTController)

## Initialization

### 

API client can be initialized as following:

```JavaScript
const lib = require('lib');


```



# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [ReportController](#report_controller)
* [InvoiceController](#invoice_controller)
* [AuthenticationController](#authentication_controller)
* [ContactController](#contact_controller)
* [CustomerController](#customer_controller)
* [GroupController](#group_controller)
* [CampaignController](#campaign_controller)
* [TransferController](#transfer_controller)
* [EmailApiConfigurationController](#email_api_configuration_controller)
* [MessageController](#message_controller)
* [RegisterControlerController](#register_controler_controller)
* [CreditConsumptionController](#credit_consumption_controller)
* [PricingController](#pricing_controller)
* [MessageModelController](#message_model_controller)
* [SocieteInfoController](#societe_info_controller)

## <a name="report_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ReportController") ReportController

### Get singleton instance

The singleton instance of the ``` ReportController ``` class can be accessed from the API Client.

```javascript
var controller = lib.ReportController;
```

### <a name="list_using_get8"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.listUsingGET8") listUsingGET8

> *Tags:*  ``` Skips Authentication ``` 

> list


```javascript
function listUsingGET8(xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.listUsingGET8(xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get8"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.listPageUsingGET8") listPageUsingGET8

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```javascript
function listPageUsingGET8(page, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var page = 40;
    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.listPageUsingGET8(page, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_using_get8"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.getUsingGET8") getUsingGET8

> *Tags:*  ``` Skips Authentication ``` 

> get


```javascript
function getUsingGET8(messageRef, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var messageRef = 'messageRef';
    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.getUsingGET8(messageRef, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_page_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.getPageUsingGET") getPageUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> getPage


```javascript
function getPageUsingGET(messageRef, page, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var messageRef = 'messageRef';
    var page = 40;
    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.getPageUsingGET(messageRef, page, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="find_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.findUsingGET") findUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> find


```javascript
function findUsingGET(messageRef, destinataire, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| destinataire |  ``` Required ```  | destinataire |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var messageRef = 'messageRef';
    var destinataire = 'destinataire';
    var xAuthToken = 'X-Auth-Token';

    controller.findUsingGET(messageRef, destinataire, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="invoice_controller"></a>![Class: ](https://apidocs.io/img/class.png ".InvoiceController") InvoiceController

### Get singleton instance

The singleton instance of the ``` InvoiceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.InvoiceController;
```

### <a name="list_using_get5"></a>![Method: ](https://apidocs.io/img/method.png ".InvoiceController.listUsingGET5") listUsingGET5

> *Tags:*  ``` Skips Authentication ``` 

> View a list of invoices


```javascript
function listUsingGET5(xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.listUsingGET5(xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get5"></a>![Method: ](https://apidocs.io/img/method.png ".InvoiceController.listPageUsingGET5") listPageUsingGET5

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```javascript
function listPageUsingGET5(page, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var page = 40;
    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.listPageUsingGET5(page, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_pdf_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".InvoiceController.getPdfUsingGET") getPdfUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Generate an invoice in a pdf file


```javascript
function getPdfUsingGET(id, xAuthToken, base64, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| base64 |  ``` Required ```  | base64 |



#### Example Usage

```javascript

    var id = 40;
    var xAuthToken = 'X-Auth-Token';
    var base64 = false;

    controller.getPdfUsingGET(id, xAuthToken, base64, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_using_get5"></a>![Method: ](https://apidocs.io/img/method.png ".InvoiceController.getUsingGET5") getUsingGET5

> *Tags:*  ``` Skips Authentication ``` 

> Show an invoice


```javascript
function getUsingGET5(id, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var id = 40;
    var xAuthToken = 'X-Auth-Token';

    controller.getUsingGET5(id, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="authentication_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AuthenticationController") AuthenticationController

### Get singleton instance

The singleton instance of the ``` AuthenticationController ``` class can be accessed from the API Client.

```javascript
var controller = lib.AuthenticationController;
```

### <a name="create_get_token_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".AuthenticationController.createGetTokenUsingPOST") createGetTokenUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Generate the OAuth Token


```javascript
function createGetTokenUsingPOST(request, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| request |  ``` Required ```  | request |



#### Example Usage

```javascript

    var request = new AuthenticationResourceModel({"key":"value"});

    controller.createGetTokenUsingPOST(request, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="contact_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactController") ContactController

### Get singleton instance

The singleton instance of the ``` ContactController ``` class can be accessed from the API Client.

```javascript
var controller = lib.ContactController;
```

### <a name="list_using_get1"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.listUsingGET1") listUsingGET1

> *Tags:*  ``` Skips Authentication ``` 

> View a list of contacts


```javascript
function listUsingGET1(xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.listUsingGET1(xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="add_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.addUsingPOST") addUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Add a contact


```javascript
function addUsingPOST(resource, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var resource = new ContactResourceModel({"key":"value"});
    var xAuthToken = 'X-Auth-Token';

    controller.addUsingPOST(resource, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="delete_book_using_delete"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.deleteBookUsingDELETE") deleteBookUsingDELETE

> *Tags:*  ``` Skips Authentication ``` 

> Remove all contacts and groups of the account


```javascript
function deleteBookUsingDELETE(xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';

    controller.deleteBookUsingDELETE(xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |




### <a name="get_customer_info_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.getCustomerInfoUsingGET") getCustomerInfoUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Show contact info of customer


```javascript
function getCustomerInfoUsingGET(xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';

    controller.getCustomerInfoUsingGET(xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="update_edit_customer_using_put"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.updateEditCustomerUsingPUT") updateEditCustomerUsingPUT

> *Tags:*  ``` Skips Authentication ``` 

> Edit contact info of customer


```javascript
function updateEditCustomerUsingPUT(xAuthToken, resource, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| resource |  ``` Required ```  | resource |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';
    var resource = new ContactResourceModel({"key":"value"});

    controller.updateEditCustomerUsingPUT(xAuthToken, resource, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_delete_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.createDeleteListUsingPOST") createDeleteListUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Delete a list of contacts


```javascript
function createDeleteListUsingPOST(idList, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| idList |  ``` Required ```  ``` Collection ```  | idList |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var idList = [40];
    var xAuthToken = 'X-Auth-Token';

    controller.createDeleteListUsingPOST(idList, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_export_contacts_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.createExportContactsUsingPOST") createExportContactsUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Export contacts in csv format


```javascript
function createExportContactsUsingPOST(fields, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fields |  ``` Required ```  ``` Collection ```  | fields |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var fields = ['fields'];
    var xAuthToken = 'X-Auth-Token';

    controller.createExportContactsUsingPOST(fields, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="upload_blocking_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.uploadBlockingUsingPOST") uploadBlockingUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Import contacts via xls or csv files


```javascript
function uploadBlockingUsingPOST(file, model, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | file |
| model |  ``` Required ```  | model |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    TestHelper.getFilePath('url', function(data) {
        var file = data;
    var model = 'model';
    var xAuthToken = 'X-Auth-Token';

        controller.uploadBlockingUsingPOST(file, model, xAuthToken, function(error, response, context) {

        });
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get1"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.listPageUsingGET1") listPageUsingGET1

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```javascript
function listPageUsingGET1(page, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var page = 40;
    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.listPageUsingGET1(page, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="search_using_get1"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.searchUsingGET1") searchUsingGET1

> *Tags:*  ``` Skips Authentication ``` 

> search


```javascript
function searchUsingGET1(name, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var name = 'name';
    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.searchUsingGET1(name, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.getUsingGET") getUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Show a contact


```javascript
function getUsingGET(id, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var id = 40;
    var xAuthToken = 'X-Auth-Token';

    controller.getUsingGET(id, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="update_using_put"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.updateUsingPUT") updateUsingPUT

> *Tags:*  ``` Skips Authentication ``` 

> Update a contact


```javascript
function updateUsingPUT(id, resource, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var id = 40;
    var resource = new ContactResourceModel({"key":"value"});
    var xAuthToken = 'X-Auth-Token';

    controller.updateUsingPUT(id, resource, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="delete_using_delete1"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.deleteUsingDELETE1") deleteUsingDELETE1

> *Tags:*  ``` Skips Authentication ``` 

> Delete a contact


```javascript
function deleteUsingDELETE1(id, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var id = 40;
    var xAuthToken = 'X-Auth-Token';

    controller.deleteUsingDELETE1(id, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |




### <a name="add_group_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.addGroupUsingPOST") addGroupUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Add a contact in a group


```javascript
function addGroupUsingPOST(id, groupId, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| groupId |  ``` Required ```  | groupId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var id = 40;
    var groupId = 40;
    var xAuthToken = 'X-Auth-Token';

    controller.addGroupUsingPOST(id, groupId, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_groups_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.getGroupsUsingGET") getGroupsUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups for a contact


```javascript
function getGroupsUsingGET(id, page, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var id = 40;
    var page = 40;
    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.getGroupsUsingGET(id, page, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="delete_group_using_delete"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.deleteGroupUsingDELETE") deleteGroupUsingDELETE

> *Tags:*  ``` Skips Authentication ``` 

> Remove a contact from a group


```javascript
function deleteGroupUsingDELETE(id, groupId, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| groupId |  ``` Required ```  | groupId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var id = 40;
    var groupId = 40;
    var xAuthToken = 'X-Auth-Token';

    controller.deleteGroupUsingDELETE(id, groupId, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |




[Back to List of Controllers](#list_of_controllers)

## <a name="customer_controller"></a>![Class: ](https://apidocs.io/img/class.png ".CustomerController") CustomerController

### Get singleton instance

The singleton instance of the ``` CustomerController ``` class can be accessed from the API Client.

```javascript
var controller = lib.CustomerController;
```

### <a name="get_using_get2"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.getUsingGET2") getUsingGET2

> *Tags:*  ``` Skips Authentication ``` 

> Show your account


```javascript
function getUsingGET2(xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';

    controller.getUsingGET2(xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_from_fields_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.getFromFieldsUsingGET") getFromFieldsUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Get your personnalized sender IDs


```javascript
function getFromFieldsUsingGET(xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';

    controller.getFromFieldsUsingGET(xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="update_delete_sender_using_put"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.updateDeleteSenderUsingPUT") updateDeleteSenderUsingPUT

> *Tags:*  ``` Skips Authentication ``` 

> Remove sender ID


```javascript
function updateDeleteSenderUsingPUT(xAuthToken, senderID, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| senderID |  ``` Required ```  | senderID |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';
    var senderID = 'senderID';

    controller.updateDeleteSenderUsingPUT(xAuthToken, senderID, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="add_sender_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.addSenderUsingPOST") addSenderUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Add personnalized sender ID


```javascript
function addSenderUsingPOST(xAuthToken, senderID, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| senderID |  ``` Required ```  | senderID |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';
    var senderID = 'senderID';

    controller.addSenderUsingPOST(xAuthToken, senderID, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_using_get3"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.listUsingGET3") listUsingGET3

> *Tags:*  ``` Skips Authentication ``` 

> View a list of your subaccounts


```javascript
function listUsingGET3(xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.listUsingGET3(xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get3"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.listPageUsingGET3") listPageUsingGET3

> *Tags:*  ``` Skips Authentication ``` 

> View a list of your subaccounts by page


```javascript
function listPageUsingGET3(page, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var page = 40;
    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.listPageUsingGET3(page, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="group_controller"></a>![Class: ](https://apidocs.io/img/class.png ".GroupController") GroupController

### Get singleton instance

The singleton instance of the ``` GroupController ``` class can be accessed from the API Client.

```javascript
var controller = lib.GroupController;
```

### <a name="list_using_get4"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.listUsingGET4") listUsingGET4

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups


```javascript
function listUsingGET4(xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.listUsingGET4(xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="add_using_post2"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.addUsingPOST2") addUsingPOST2

> *Tags:*  ``` Skips Authentication ``` 

> Add a group


```javascript
function addUsingPOST2(resource, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var resource = new GroupResourceModel({"key":"value"});
    var xAuthToken = 'X-Auth-Token';

    controller.addUsingPOST2(resource, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_delete_list_using_post1"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.createDeleteListUsingPOST1") createDeleteListUsingPOST1

> *Tags:*  ``` Skips Authentication ``` 

> Delete a list of groups


```javascript
function createDeleteListUsingPOST1(idList, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| idList |  ``` Required ```  ``` Collection ```  | idList |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var idList = [40];
    var xAuthToken = 'X-Auth-Token';

    controller.createDeleteListUsingPOST1(idList, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get4"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.listPageUsingGET4") listPageUsingGET4

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```javascript
function listPageUsingGET4(page, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var page = 40;
    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.listPageUsingGET4(page, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="search_using_get2"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.searchUsingGET2") searchUsingGET2

> *Tags:*  ``` Skips Authentication ``` 

> search


```javascript
function searchUsingGET2(name, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var name = 'name';
    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.searchUsingGET2(name, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_using_get4"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.getUsingGET4") getUsingGET4

> *Tags:*  ``` Skips Authentication ``` 

> Show a group


```javascript
function getUsingGET4(id, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var id = 40;
    var xAuthToken = 'X-Auth-Token';

    controller.getUsingGET4(id, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="update_using_put2"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.updateUsingPUT2") updateUsingPUT2

> *Tags:*  ``` Skips Authentication ``` 

> Update a group


```javascript
function updateUsingPUT2(id, resource, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var id = 40;
    var resource = new GroupResourceModel({"key":"value"});
    var xAuthToken = 'X-Auth-Token';

    controller.updateUsingPUT2(id, resource, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="delete_using_delete3"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.deleteUsingDELETE3") deleteUsingDELETE3

> *Tags:*  ``` Skips Authentication ``` 

> Delete a group


```javascript
function deleteUsingDELETE3(id, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var id = 40;
    var xAuthToken = 'X-Auth-Token';

    controller.deleteUsingDELETE3(id, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |




### <a name="get_contacts_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.getContactsUsingGET") getContactsUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Show a list of contacts for a group


```javascript
function getContactsUsingGET(id, page, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var id = 40;
    var page = 40;
    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.getContactsUsingGET(id, page, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="campaign_controller"></a>![Class: ](https://apidocs.io/img/class.png ".CampaignController") CampaignController

### Get singleton instance

The singleton instance of the ``` CampaignController ``` class can be accessed from the API Client.

```javascript
var controller = lib.CampaignController;
```

### <a name="list_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.listUsingGET") listUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> list


```javascript
function listUsingGET(xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.listUsingGET(xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_send_to_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.createSendToListUsingPOST") createSendToListUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> sendToList


```javascript
function createSendToListUsingPOST(resource, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var resource = new CampaignInputResourceModel({"key":"value"});
    var xAuthToken = 'X-Auth-Token';

    controller.createSendToListUsingPOST(resource, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.listPageUsingGET") listPageUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```javascript
function listPageUsingGET(page, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var page = 40;
    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.listPageUsingGET(page, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="search_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.searchUsingGET") searchUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> search


```javascript
function searchUsingGET(name, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var name = 'name';
    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.searchUsingGET(name, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="delete_using_delete"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.deleteUsingDELETE") deleteUsingDELETE

> *Tags:*  ``` Skips Authentication ``` 

> delete


```javascript
function deleteUsingDELETE(messsageId, xAuthToken, id, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsageId |  ``` Required ```  | messsageId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| id |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var messsageId = 'messsageId';
    var xAuthToken = 'X-Auth-Token';
    var id = 'id';

    controller.deleteUsingDELETE(messsageId, xAuthToken, id, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |




[Back to List of Controllers](#list_of_controllers)

## <a name="transfer_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TransferController") TransferController

### Get singleton instance

The singleton instance of the ``` TransferController ``` class can be accessed from the API Client.

```javascript
var controller = lib.TransferController;
```

### <a name="list_using_get9"></a>![Method: ](https://apidocs.io/img/method.png ".TransferController.listUsingGET9") listUsingGET9

> *Tags:*  ``` Skips Authentication ``` 

> View a list of transferts


```javascript
function listUsingGET9(xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.listUsingGET9(xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get9"></a>![Method: ](https://apidocs.io/img/method.png ".TransferController.listPageUsingGET9") listPageUsingGET9

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```javascript
function listPageUsingGET9(page, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var page = 40;
    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.listPageUsingGET9(page, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_using_get9"></a>![Method: ](https://apidocs.io/img/method.png ".TransferController.getUsingGET9") getUsingGET9

> *Tags:*  ``` Skips Authentication ``` 

> Show a transfet


```javascript
function getUsingGET9(id, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var id = 40;
    var xAuthToken = 'X-Auth-Token';

    controller.getUsingGET9(id, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="email_api_configuration_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailApiConfigurationController") EmailApiConfigurationController

### Get singleton instance

The singleton instance of the ``` EmailApiConfigurationController ``` class can be accessed from the API Client.

```javascript
var controller = lib.EmailApiConfigurationController;
```

### <a name="get_using_get3"></a>![Method: ](https://apidocs.io/img/method.png ".EmailApiConfigurationController.getUsingGET3") getUsingGET3

> *Tags:*  ``` Skips Authentication ``` 

> Show your configuration


```javascript
function getUsingGET3(xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';

    controller.getUsingGET3(xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="update_using_put1"></a>![Method: ](https://apidocs.io/img/method.png ".EmailApiConfigurationController.updateUsingPUT1") updateUsingPUT1

> *Tags:*  ``` Skips Authentication ``` 

> Update your configuration


```javascript
function updateUsingPUT1(resource, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var resource = new EmailAPIConfigurationResourceModel({"key":"value"});
    var xAuthToken = 'X-Auth-Token';

    controller.updateUsingPUT1(resource, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="add_using_post1"></a>![Method: ](https://apidocs.io/img/method.png ".EmailApiConfigurationController.addUsingPOST1") addUsingPOST1

> *Tags:*  ``` Skips Authentication ``` 

> Create your configuration


```javascript
function addUsingPOST1(resource, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var resource = new EmailAPIConfigurationResourceModel({"key":"value"});
    var xAuthToken = 'X-Auth-Token';

    controller.addUsingPOST1(resource, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="delete_using_delete2"></a>![Method: ](https://apidocs.io/img/method.png ".EmailApiConfigurationController.deleteUsingDELETE2") deleteUsingDELETE2

> *Tags:*  ``` Skips Authentication ``` 

> Delete your configuration


```javascript
function deleteUsingDELETE2(xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';

    controller.deleteUsingDELETE2(xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |




[Back to List of Controllers](#list_of_controllers)

## <a name="message_controller"></a>![Class: ](https://apidocs.io/img/class.png ".MessageController") MessageController

### Get singleton instance

The singleton instance of the ``` MessageController ``` class can be accessed from the API Client.

```javascript
var controller = lib.MessageController;
```

### <a name="list_using_get6"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.listUsingGET6") listUsingGET6

> *Tags:*  ``` Skips Authentication ``` 

> list


```javascript
function listUsingGET6(xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.listUsingGET6(xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get6"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.listPageUsingGET6") listPageUsingGET6

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```javascript
function listPageUsingGET6(page, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var page = 40;
    var xAuthToken = 'X-Auth-Token';
    var limit = 40;

    controller.listPageUsingGET6(page, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_responses_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.listResponsesUsingGET") listResponsesUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> listResponses


```javascript
function listResponsesUsingGET(xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';
    var limit = 253;

    controller.listResponsesUsingGET(xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_responses_page_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.listResponsesPageUsingGET") listResponsesPageUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> listResponsesPage


```javascript
function listResponsesPageUsingGET(page, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var page = 253;
    var xAuthToken = 'X-Auth-Token';
    var limit = 253;

    controller.listResponsesPageUsingGET(page, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_scheduled_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.listScheduledUsingGET") listScheduledUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> listScheduled


```javascript
function listScheduledUsingGET(xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';
    var limit = 253;

    controller.listScheduledUsingGET(xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_scheduled_page_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.listScheduledPageUsingGET") listScheduledPageUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> listScheduledPage


```javascript
function listScheduledPageUsingGET(page, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var page = 253;
    var xAuthToken = 'X-Auth-Token';
    var limit = 253;

    controller.listScheduledPageUsingGET(page, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="search_using_get3"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.searchUsingGET3") searchUsingGET3

> *Tags:*  ``` Skips Authentication ``` 

> search


```javascript
function searchUsingGET3(id, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var id = 'id';
    var xAuthToken = 'X-Auth-Token';
    var limit = 253;

    controller.searchUsingGET3(id, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_send_to_list_using_post1"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.createSendToListUsingPOST1") createSendToListUsingPOST1

> *Tags:*  ``` Skips Authentication ``` 

> sendToList


```javascript
function createSendToListUsingPOST1(resource, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var resource = new MessageInputMixedResourceModel({"key":"value"});
    var xAuthToken = 'X-Auth-Token';

    controller.createSendToListUsingPOST1(resource, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_send_to_contact_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.createSendToContactListUsingPOST") createSendToContactListUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> sendToContactList


```javascript
function createSendToContactListUsingPOST(resource, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var resource = new MessageInputContactResourceModel({"key":"value"});
    var xAuthToken = 'X-Auth-Token';

    controller.createSendToContactListUsingPOST(resource, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_send_to_group_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.createSendToGroupListUsingPOST") createSendToGroupListUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> sendToGroupList


```javascript
function createSendToGroupListUsingPOST(resource, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var resource = new MessageInputGroupResourceModel({"key":"value"});
    var xAuthToken = 'X-Auth-Token';

    controller.createSendToGroupListUsingPOST(resource, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_send_to_number_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.createSendToNumberListUsingPOST") createSendToNumberListUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> sendToNumberList


```javascript
function createSendToNumberListUsingPOST(resource, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var resource = new MessageInputResourceModel({"key":"value"});
    var xAuthToken = 'X-Auth-Token';

    controller.createSendToNumberListUsingPOST(resource, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="delete_using_delete4"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.deleteUsingDELETE4") deleteUsingDELETE4

> *Tags:*  ``` Skips Authentication ``` 

> delete


```javascript
function deleteUsingDELETE4(messsageId, xAuthToken, id, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsageId |  ``` Required ```  | messsageId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| id |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var messsageId = 'messsageId';
    var xAuthToken = 'X-Auth-Token';
    var id = 'id';

    controller.deleteUsingDELETE4(messsageId, xAuthToken, id, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |




[Back to List of Controllers](#list_of_controllers)

## <a name="register_controler_controller"></a>![Class: ](https://apidocs.io/img/class.png ".RegisterControlerController") RegisterControlerController

### Get singleton instance

The singleton instance of the ``` RegisterControlerController ``` class can be accessed from the API Client.

```javascript
var controller = lib.RegisterControlerController;
```

### <a name="create_register_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".RegisterControlerController.createRegisterUsingPOST") createRegisterUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> register


```javascript
function createRegisterUsingPOST(resource, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |



#### Example Usage

```javascript

    var resource = new RegisterResourceModel({"key":"value"});

    controller.createRegisterUsingPOST(resource, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_refresh_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".RegisterControlerController.createRefreshUsingPOST") createRefreshUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> refresh


```javascript
function createRefreshUsingPOST(resource, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |



#### Example Usage

```javascript

    var resource = new SimpleEmailResourceModel({"key":"value"});

    controller.createRefreshUsingPOST(resource, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_activate_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".RegisterControlerController.getActivateUsingGET") getActivateUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> activate


```javascript
function getActivateUsingGET(token, id, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| token |  ``` Required ```  | token |
| id |  ``` Required ```  | id |



#### Example Usage

```javascript

    var token = 'token';
    var id = 253;

    controller.getActivateUsingGET(token, id, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="credit_consumption_controller"></a>![Class: ](https://apidocs.io/img/class.png ".CreditConsumptionController") CreditConsumptionController

### Get singleton instance

The singleton instance of the ``` CreditConsumptionController ``` class can be accessed from the API Client.

```javascript
var controller = lib.CreditConsumptionController;
```

### <a name="list_using_get2"></a>![Method: ](https://apidocs.io/img/method.png ".CreditConsumptionController.listUsingGET2") listUsingGET2

> *Tags:*  ``` Skips Authentication ``` 

> Get the consumption of the last months


```javascript
function listUsingGET2(xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';
    var limit = 253;

    controller.listUsingGET2(xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get2"></a>![Method: ](https://apidocs.io/img/method.png ".CreditConsumptionController.listPageUsingGET2") listPageUsingGET2

> *Tags:*  ``` Skips Authentication ``` 

> Get pageable consumption of the last months


```javascript
function listPageUsingGET2(page, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var page = 253;
    var xAuthToken = 'X-Auth-Token';
    var limit = 253;

    controller.listPageUsingGET2(page, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_using_get1"></a>![Method: ](https://apidocs.io/img/method.png ".CreditConsumptionController.getUsingGET1") getUsingGET1

> *Tags:*  ``` Skips Authentication ``` 

> Get specific consumption by id 


```javascript
function getUsingGET1(id, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var id = 253;
    var xAuthToken = 'X-Auth-Token';

    controller.getUsingGET1(id, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="pricing_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PricingController") PricingController

### Get singleton instance

The singleton instance of the ``` PricingController ``` class can be accessed from the API Client.

```javascript
var controller = lib.PricingController;
```

### <a name="get_using_get7"></a>![Method: ](https://apidocs.io/img/method.png ".PricingController.getUsingGET7") getUsingGET7

> *Tags:*  ``` Skips Authentication ``` 

> get


```javascript
function getUsingGET7(xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';

    controller.getUsingGET7(xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="message_model_controller"></a>![Class: ](https://apidocs.io/img/class.png ".MessageModelController") MessageModelController

### Get singleton instance

The singleton instance of the ``` MessageModelController ``` class can be accessed from the API Client.

```javascript
var controller = lib.MessageModelController;
```

### <a name="list_using_get7"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.listUsingGET7") listUsingGET7

> *Tags:*  ``` Skips Authentication ``` 

> list


```javascript
function listUsingGET7(xAuthToken, size, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| size |  ``` Optional ```  | size |



#### Example Usage

```javascript

    var xAuthToken = 'X-Auth-Token';
    var size = 253;

    controller.listUsingGET7(xAuthToken, size, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="add_using_post3"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.addUsingPOST3") addUsingPOST3

> *Tags:*  ``` Skips Authentication ``` 

> add


```javascript
function addUsingPOST3(resource, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var resource = new MessageModelInputResourceModel({"key":"value"});
    var xAuthToken = 'X-Auth-Token';

    controller.addUsingPOST3(resource, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_delete_multiple_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.createDeleteMultipleUsingPOST") createDeleteMultipleUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> deleteMultiple


```javascript
function createDeleteMultipleUsingPOST(ids, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ids |  ``` Required ```  ``` Collection ```  | ids |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var ids = ['ids'];
    var xAuthToken = 'X-Auth-Token';

    controller.createDeleteMultipleUsingPOST(ids, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get7"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.listPageUsingGET7") listPageUsingGET7

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```javascript
function listPageUsingGET7(page, xAuthToken, limit, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript

    var page = 253;
    var xAuthToken = 'X-Auth-Token';
    var limit = 253;

    controller.listPageUsingGET7(page, xAuthToken, limit, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_using_get6"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.getUsingGET6") getUsingGET6

> *Tags:*  ``` Skips Authentication ``` 

> get


```javascript
function getUsingGET6(id, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var id = 'id';
    var xAuthToken = 'X-Auth-Token';

    controller.getUsingGET6(id, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="update_using_put3"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.updateUsingPUT3") updateUsingPUT3

> *Tags:*  ``` Skips Authentication ``` 

> update


```javascript
function updateUsingPUT3(id, resource, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var id = 'id';
    var resource = new MessageModelInputResourceModel({"key":"value"});
    var xAuthToken = 'X-Auth-Token';

    controller.updateUsingPUT3(id, resource, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="delete_using_delete5"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.deleteUsingDELETE5") deleteUsingDELETE5

> *Tags:*  ``` Skips Authentication ``` 

> delete


```javascript
function deleteUsingDELETE5(id, xAuthToken, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript

    var id = 'id';
    var xAuthToken = 'X-Auth-Token';

    controller.deleteUsingDELETE5(id, xAuthToken, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |




[Back to List of Controllers](#list_of_controllers)

## <a name="societe_info_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SocieteInfoController") SocieteInfoController

### Get singleton instance

The singleton instance of the ``` SocieteInfoController ``` class can be accessed from the API Client.

```javascript
var controller = lib.SocieteInfoController;
```

### <a name="create_research_company_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".SocieteInfoController.createResearchCompanyUsingPOST") createResearchCompanyUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> researchCompany


```javascript
function createResearchCompanyUsingPOST(research, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| research |  ``` Required ```  | research |



#### Example Usage

```javascript

    var research = new SocieteInfoResearchResourceModel({"key":"value"});

    controller.createResearchCompanyUsingPOST(research, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_details_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".SocieteInfoController.getDetailsUsingGET") getDetailsUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> getDetails


```javascript
function getDetailsUsingGET(id, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |



#### Example Usage

```javascript

    var id = 'id';

    controller.getDetailsUsingGET(id, function(error, response, context) {

    
    });
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)



