# Getting started

sMsMode API-REST Documentation

## How to Build

The generated code has dependencies over external libraries like UniRest. These dependencies are defined in the ```composer.json``` file that comes with the SDK. 
To resolve these dependencies, we use the Composer package manager which requires PHP greater than 5.3.2 installed in your system. 
Visit [https://getcomposer.org/download/](https://getcomposer.org/download/) to download the installer file for Composer and run it in your system. 
Open command prompt and type ```composer --version```. This should display the current version of the Composer installed if the installation was successful.

* Using command line, navigate to the directory containing the generated files (including ```composer.json```) for the SDK. 
* Run the command ```composer install```. This should install all the required dependencies and create the ```vendor``` directory in your project directory.

![Building SDK - Step 1](https://apidocs.io/illustration/php?step=installDependencies&workspaceFolder=sMsmode%20API-REST-PHP)

### [For Windows Users Only] Configuring CURL Certificate Path in php.ini

CURL used to include a list of accepted CAs, but no longer bundles ANY CA certs. So by default it will reject all SSL certificates as unverifiable. You will have to get your CA's cert and point curl at it. The steps are as follows:

1. Download the certificate bundle (.pem file) from [https://curl.haxx.se/docs/caextract.html](https://curl.haxx.se/docs/caextract.html) on to your system.
2. Add curl.cainfo = "PATH_TO/cacert.pem" to your php.ini file located in your php installation. “PATH_TO” must be an absolute path containing the .pem file.

```ini
[curl]
; A default value for the CURLOPT_CAINFO option. This is required to be an
; absolute path.
;curl.cainfo =
```

## How to Use

The following section explains how to use the SMsmodeAPIREST library in a new project.

### 1. Open Project in an IDE

Open an IDE for PHP like PhpStorm. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.

![Open project in PHPStorm - Step 1](https://apidocs.io/illustration/php?step=openIDE&workspaceFolder=sMsmode%20API-REST-PHP)

Click on ```Open``` in PhpStorm to browse to your generated SDK directory and then click ```OK```.

![Open project in PHPStorm - Step 2](https://apidocs.io/illustration/php?step=openProject0&workspaceFolder=sMsmode%20API-REST-PHP)     

### 2. Add a new Test Project

Create a new directory by right clicking on the solution name as shown below:

![Add a new project in PHPStorm - Step 1](https://apidocs.io/illustration/php?step=createDirectory&workspaceFolder=sMsmode%20API-REST-PHP)

Name the directory as "test"

![Add a new project in PHPStorm - Step 2](https://apidocs.io/illustration/php?step=nameDirectory&workspaceFolder=sMsmode%20API-REST-PHP)
   
Add a PHP file to this project

![Add a new project in PHPStorm - Step 3](https://apidocs.io/illustration/php?step=createFile&workspaceFolder=sMsmode%20API-REST-PHP)

Name it "testSDK"

![Add a new project in PHPStorm - Step 4](https://apidocs.io/illustration/php?step=nameFile&workspaceFolder=sMsmode%20API-REST-PHP)

Depending on your project setup, you might need to include composer's autoloader in your PHP code to enable auto loading of classes.

```PHP
require_once "../vendor/autoload.php";
```

It is important that the path inside require_once correctly points to the file ```autoload.php``` inside the vendor directory created during dependency installations.

![Add a new project in PHPStorm - Step 4](https://apidocs.io/illustration/php?step=projectFiles&workspaceFolder=sMsmode%20API-REST-PHP)

After this you can add code to initialize the client library and acquire the instance of a Controller class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

### 3. Run the Test Project

To run your project you must set the Interpreter for your project. Interpreter is the PHP engine installed on your computer.

Open ```Settings``` from ```File``` menu.

![Run Test Project - Step 1](https://apidocs.io/illustration/php?step=openSettings&workspaceFolder=sMsmode%20API-REST-PHP)

Select ```PHP``` from within ```Languages & Frameworks```

![Run Test Project - Step 2](https://apidocs.io/illustration/php?step=setInterpreter0&workspaceFolder=sMsmode%20API-REST-PHP)

Browse for Interpreters near the ```Interpreter``` option and choose your interpreter.

![Run Test Project - Step 3](https://apidocs.io/illustration/php?step=setInterpreter1&workspaceFolder=sMsmode%20API-REST-PHP)

Once the interpreter is selected, click ```OK```

![Run Test Project - Step 4](https://apidocs.io/illustration/php?step=setInterpreter2&workspaceFolder=sMsmode%20API-REST-PHP)

To run your project, right click on your PHP file inside your Test project and click on ```Run```

![Run Test Project - Step 5](https://apidocs.io/illustration/php?step=runProject&workspaceFolder=sMsmode%20API-REST-PHP)

## How to Test

Unit tests in this SDK can be run using PHPUnit. 

1. First install the dependencies using composer including the `require-dev` dependencies.
2. Run `vendor\bin\phpunit --verbose` from commandline to execute tests. If you have 
   installed PHPUnit globally, run tests using `phpunit --verbose` instead.

You can change the PHPUnit test configuration in the `phpunit.xml` file.

## Initialization

### 

API client can be initialized as following.

```php

$client = new SMsmodeAPIRESTLib\SMsmodeAPIRESTClient();
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

```php
$reportController = $client->getReportController();
```

### <a name="list_using_get8"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.listUsingGET8") listUsingGET8

> *Tags:*  ``` Skips Authentication ``` 

> list


```php
function listUsingGET8(
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';
$limit = 26;

$result = $reportController->listUsingGET8($xAuthToken, $limit);

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


```php
function listPageUsingGET8(
        $page,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$page = 26;
$xAuthToken = 'X-Auth-Token';
$limit = 26;

$result = $reportController->listPageUsingGET8($page, $xAuthToken, $limit);

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


```php
function getUsingGET8(
        $messageRef,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$messageRef = 'messageRef';
$xAuthToken = 'X-Auth-Token';
$limit = 26;

$result = $reportController->getUsingGET8($messageRef, $xAuthToken, $limit);

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


```php
function getPageUsingGET(
        $messageRef,
        $page,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$messageRef = 'messageRef';
$page = 26;
$xAuthToken = 'X-Auth-Token';
$limit = 26;

$result = $reportController->getPageUsingGET($messageRef, $page, $xAuthToken, $limit);

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


```php
function findUsingGET(
        $messageRef,
        $destinataire,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| destinataire |  ``` Required ```  | destinataire |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$messageRef = 'messageRef';
$destinataire = 'destinataire';
$xAuthToken = 'X-Auth-Token';

$result = $reportController->findUsingGET($messageRef, $destinataire, $xAuthToken);

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

```php
$invoiceController = $client->getInvoiceController();
```

### <a name="list_using_get5"></a>![Method: ](https://apidocs.io/img/method.png ".InvoiceController.listUsingGET5") listUsingGET5

> *Tags:*  ``` Skips Authentication ``` 

> View a list of invoices


```php
function listUsingGET5(
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';
$limit = 26;

$result = $invoiceController->listUsingGET5($xAuthToken, $limit);

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


```php
function listPageUsingGET5(
        $page,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$page = 26;
$xAuthToken = 'X-Auth-Token';
$limit = 26;

$result = $invoiceController->listPageUsingGET5($page, $xAuthToken, $limit);

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


```php
function getPdfUsingGET(
        $id,
        $xAuthToken,
        $base64)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| base64 |  ``` Required ```  | base64 |



#### Example Usage

```php
$id = 26;
$xAuthToken = 'X-Auth-Token';
$base64 = false;

$result = $invoiceController->getPdfUsingGET($id, $xAuthToken, $base64);

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


```php
function getUsingGET5(
        $id,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$id = 26;
$xAuthToken = 'X-Auth-Token';

$result = $invoiceController->getUsingGET5($id, $xAuthToken);

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

```php
$authenticationController = $client->getAuthenticationController();
```

### <a name="create_get_token_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".AuthenticationController.createGetTokenUsingPOST") createGetTokenUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Generate the OAuth Token


```php
function createGetTokenUsingPOST($request)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| request |  ``` Required ```  | request |



#### Example Usage

```php
$request = new AuthenticationResourceModel();

$result = $authenticationController->createGetTokenUsingPOST($request);

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

```php
$contactController = $client->getContactController();
```

### <a name="list_using_get1"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.listUsingGET1") listUsingGET1

> *Tags:*  ``` Skips Authentication ``` 

> View a list of contacts


```php
function listUsingGET1(
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';
$limit = 26;

$result = $contactController->listUsingGET1($xAuthToken, $limit);

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


```php
function addUsingPOST(
        $resource,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$resource = new ContactResourceModel();
$xAuthToken = 'X-Auth-Token';

$result = $contactController->addUsingPOST($resource, $xAuthToken);

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


```php
function deleteBookUsingDELETE($xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';

$result = $contactController->deleteBookUsingDELETE($xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



### <a name="get_customer_info_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.getCustomerInfoUsingGET") getCustomerInfoUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Show contact info of customer


```php
function getCustomerInfoUsingGET($xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';

$result = $contactController->getCustomerInfoUsingGET($xAuthToken);

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


```php
function updateEditCustomerUsingPUT(
        $xAuthToken,
        $resource)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| resource |  ``` Required ```  | resource |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';
$resource = new ContactResourceModel();

$result = $contactController->updateEditCustomerUsingPUT($xAuthToken, $resource);

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


```php
function createDeleteListUsingPOST(
        $idList,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| idList |  ``` Required ```  ``` Collection ```  | idList |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$idList = array(26);
$xAuthToken = 'X-Auth-Token';

$result = $contactController->createDeleteListUsingPOST($idList, $xAuthToken);

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


```php
function createExportContactsUsingPOST(
        $fields,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fields |  ``` Required ```  ``` Collection ```  | fields |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$fields = array('fields');
$xAuthToken = 'X-Auth-Token';

$result = $contactController->createExportContactsUsingPOST($fields, $xAuthToken);

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


```php
function uploadBlockingUsingPOST(
        $file,
        $model,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | file |
| model |  ``` Required ```  | model |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$file = "PathToFile";
$model = 'model';
$xAuthToken = 'X-Auth-Token';

$result = $contactController->uploadBlockingUsingPOST($file, $model, $xAuthToken);

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


```php
function listPageUsingGET1(
        $page,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$page = 26;
$xAuthToken = 'X-Auth-Token';
$limit = 26;

$result = $contactController->listPageUsingGET1($page, $xAuthToken, $limit);

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


```php
function searchUsingGET1(
        $name,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$name = 'name';
$xAuthToken = 'X-Auth-Token';
$limit = 26;

$result = $contactController->searchUsingGET1($name, $xAuthToken, $limit);

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


```php
function getUsingGET(
        $id,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$id = 26;
$xAuthToken = 'X-Auth-Token';

$result = $contactController->getUsingGET($id, $xAuthToken);

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


```php
function updateUsingPUT(
        $id,
        $resource,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$id = 26;
$resource = new ContactResourceModel();
$xAuthToken = 'X-Auth-Token';

$result = $contactController->updateUsingPUT($id, $resource, $xAuthToken);

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


```php
function deleteUsingDELETE1(
        $id,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$id = 117;
$xAuthToken = 'X-Auth-Token';

$result = $contactController->deleteUsingDELETE1($id, $xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



### <a name="add_group_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.addGroupUsingPOST") addGroupUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Add a contact in a group


```php
function addGroupUsingPOST(
        $id,
        $groupId,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| groupId |  ``` Required ```  | groupId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$id = 117;
$groupId = 117;
$xAuthToken = 'X-Auth-Token';

$result = $contactController->addGroupUsingPOST($id, $groupId, $xAuthToken);

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


```php
function getGroupsUsingGET(
        $id,
        $page,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$id = 117;
$page = 117;
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $contactController->getGroupsUsingGET($id, $page, $xAuthToken, $limit);

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


```php
function deleteGroupUsingDELETE(
        $id,
        $groupId,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| groupId |  ``` Required ```  | groupId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$id = 117;
$groupId = 117;
$xAuthToken = 'X-Auth-Token';

$result = $contactController->deleteGroupUsingDELETE($id, $groupId, $xAuthToken);

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

```php
$customerController = $client->getCustomerController();
```

### <a name="get_using_get2"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.getUsingGET2") getUsingGET2

> *Tags:*  ``` Skips Authentication ``` 

> Show your account


```php
function getUsingGET2($xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';

$result = $customerController->getUsingGET2($xAuthToken);

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


```php
function getFromFieldsUsingGET($xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';

$result = $customerController->getFromFieldsUsingGET($xAuthToken);

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


```php
function updateDeleteSenderUsingPUT(
        $xAuthToken,
        $senderID)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| senderID |  ``` Required ```  | senderID |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';
$senderID = 'senderID';

$result = $customerController->updateDeleteSenderUsingPUT($xAuthToken, $senderID);

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


```php
function addSenderUsingPOST(
        $xAuthToken,
        $senderID)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| senderID |  ``` Required ```  | senderID |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';
$senderID = 'senderID';

$result = $customerController->addSenderUsingPOST($xAuthToken, $senderID);

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


```php
function listUsingGET3(
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $customerController->listUsingGET3($xAuthToken, $limit);

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


```php
function listPageUsingGET3(
        $page,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$page = 117;
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $customerController->listPageUsingGET3($page, $xAuthToken, $limit);

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

```php
$groupController = $client->getGroupController();
```

### <a name="list_using_get4"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.listUsingGET4") listUsingGET4

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups


```php
function listUsingGET4(
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $groupController->listUsingGET4($xAuthToken, $limit);

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


```php
function addUsingPOST2(
        $resource,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$resource = new GroupResourceModel();
$xAuthToken = 'X-Auth-Token';

$result = $groupController->addUsingPOST2($resource, $xAuthToken);

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


```php
function createDeleteListUsingPOST1(
        $idList,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| idList |  ``` Required ```  ``` Collection ```  | idList |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$idList = array(117);
$xAuthToken = 'X-Auth-Token';

$result = $groupController->createDeleteListUsingPOST1($idList, $xAuthToken);

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


```php
function listPageUsingGET4(
        $page,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$page = 117;
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $groupController->listPageUsingGET4($page, $xAuthToken, $limit);

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


```php
function searchUsingGET2(
        $name,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$name = 'name';
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $groupController->searchUsingGET2($name, $xAuthToken, $limit);

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


```php
function getUsingGET4(
        $id,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$id = 117;
$xAuthToken = 'X-Auth-Token';

$result = $groupController->getUsingGET4($id, $xAuthToken);

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


```php
function updateUsingPUT2(
        $id,
        $resource,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$id = 117;
$resource = new GroupResourceModel();
$xAuthToken = 'X-Auth-Token';

$result = $groupController->updateUsingPUT2($id, $resource, $xAuthToken);

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


```php
function deleteUsingDELETE3(
        $id,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$id = 117;
$xAuthToken = 'X-Auth-Token';

$result = $groupController->deleteUsingDELETE3($id, $xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



### <a name="get_contacts_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.getContactsUsingGET") getContactsUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Show a list of contacts for a group


```php
function getContactsUsingGET(
        $id,
        $page,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$id = 117;
$page = 117;
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $groupController->getContactsUsingGET($id, $page, $xAuthToken, $limit);

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

```php
$campaignController = $client->getCampaignController();
```

### <a name="list_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.listUsingGET") listUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> list


```php
function listUsingGET(
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $campaignController->listUsingGET($xAuthToken, $limit);

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


```php
function createSendToListUsingPOST(
        $resource,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$resource = new CampaignInputResourceModel();
$xAuthToken = 'X-Auth-Token';

$result = $campaignController->createSendToListUsingPOST($resource, $xAuthToken);

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


```php
function listPageUsingGET(
        $page,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$page = 117;
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $campaignController->listPageUsingGET($page, $xAuthToken, $limit);

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


```php
function searchUsingGET(
        $name,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$name = 'name';
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $campaignController->searchUsingGET($name, $xAuthToken, $limit);

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


```php
function deleteUsingDELETE(
        $messsageId,
        $xAuthToken,
        $id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsageId |  ``` Required ```  | messsageId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| id |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$messsageId = 'messsageId';
$xAuthToken = 'X-Auth-Token';
$id = 'id';

$result = $campaignController->deleteUsingDELETE($messsageId, $xAuthToken, $id);

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

```php
$transferController = $client->getTransferController();
```

### <a name="list_using_get9"></a>![Method: ](https://apidocs.io/img/method.png ".TransferController.listUsingGET9") listUsingGET9

> *Tags:*  ``` Skips Authentication ``` 

> View a list of transferts


```php
function listUsingGET9(
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $transferController->listUsingGET9($xAuthToken, $limit);

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


```php
function listPageUsingGET9(
        $page,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$page = 117;
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $transferController->listPageUsingGET9($page, $xAuthToken, $limit);

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


```php
function getUsingGET9(
        $id,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$id = 117;
$xAuthToken = 'X-Auth-Token';

$result = $transferController->getUsingGET9($id, $xAuthToken);

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

```php
$emailApiConfigurationController = $client->getEmailApiConfigurationController();
```

### <a name="get_using_get3"></a>![Method: ](https://apidocs.io/img/method.png ".EmailApiConfigurationController.getUsingGET3") getUsingGET3

> *Tags:*  ``` Skips Authentication ``` 

> Show your configuration


```php
function getUsingGET3($xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';

$result = $emailApiConfigurationController->getUsingGET3($xAuthToken);

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


```php
function updateUsingPUT1(
        $resource,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$resource = new EmailAPIConfigurationResourceModel();
$xAuthToken = 'X-Auth-Token';

$result = $emailApiConfigurationController->updateUsingPUT1($resource, $xAuthToken);

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


```php
function addUsingPOST1(
        $resource,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$resource = new EmailAPIConfigurationResourceModel();
$xAuthToken = 'X-Auth-Token';

$result = $emailApiConfigurationController->addUsingPOST1($resource, $xAuthToken);

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


```php
function deleteUsingDELETE2($xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';

$result = $emailApiConfigurationController->deleteUsingDELETE2($xAuthToken);

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

```php
$messageController = $client->getMessageController();
```

### <a name="list_using_get6"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.listUsingGET6") listUsingGET6

> *Tags:*  ``` Skips Authentication ``` 

> list


```php
function listUsingGET6(
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $messageController->listUsingGET6($xAuthToken, $limit);

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


```php
function listPageUsingGET6(
        $page,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$page = 117;
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $messageController->listPageUsingGET6($page, $xAuthToken, $limit);

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


```php
function listResponsesUsingGET(
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $messageController->listResponsesUsingGET($xAuthToken, $limit);

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


```php
function listResponsesPageUsingGET(
        $page,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$page = 117;
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $messageController->listResponsesPageUsingGET($page, $xAuthToken, $limit);

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


```php
function listScheduledUsingGET(
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';
$limit = 117;

$result = $messageController->listScheduledUsingGET($xAuthToken, $limit);

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


```php
function listScheduledPageUsingGET(
        $page,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$page = 75;
$xAuthToken = 'X-Auth-Token';
$limit = 75;

$result = $messageController->listScheduledPageUsingGET($page, $xAuthToken, $limit);

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


```php
function searchUsingGET3(
        $id,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$id = 'id';
$xAuthToken = 'X-Auth-Token';
$limit = 75;

$result = $messageController->searchUsingGET3($id, $xAuthToken, $limit);

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


```php
function createSendToListUsingPOST1(
        $resource,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$resource = new MessageInputMixedResourceModel();
$xAuthToken = 'X-Auth-Token';

$result = $messageController->createSendToListUsingPOST1($resource, $xAuthToken);

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


```php
function createSendToContactListUsingPOST(
        $resource,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$resource = new MessageInputContactResourceModel();
$xAuthToken = 'X-Auth-Token';

$messageController->createSendToContactListUsingPOST($resource, $xAuthToken);

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


```php
function createSendToGroupListUsingPOST(
        $resource,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$resource = new MessageInputGroupResourceModel();
$xAuthToken = 'X-Auth-Token';

$messageController->createSendToGroupListUsingPOST($resource, $xAuthToken);

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


```php
function createSendToNumberListUsingPOST(
        $resource,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$resource = new MessageInputResourceModel();
$xAuthToken = 'X-Auth-Token';

$result = $messageController->createSendToNumberListUsingPOST($resource, $xAuthToken);

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


```php
function deleteUsingDELETE4(
        $messsageId,
        $xAuthToken,
        $id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsageId |  ``` Required ```  | messsageId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| id |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$messsageId = 'messsageId';
$xAuthToken = 'X-Auth-Token';
$id = 'id';

$messageController->deleteUsingDELETE4($messsageId, $xAuthToken, $id);

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

```php
$registerControler = $client->getRegisterControler();
```

### <a name="create_register_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".RegisterControlerController.createRegisterUsingPOST") createRegisterUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> register


```php
function createRegisterUsingPOST($resource)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |



#### Example Usage

```php
$resource = new RegisterResourceModel();

$result = $registerControler->createRegisterUsingPOST($resource);

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


```php
function createRefreshUsingPOST($resource)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |



#### Example Usage

```php
$resource = new SimpleEmailResourceModel();

$result = $registerControler->createRefreshUsingPOST($resource);

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


```php
function getActivateUsingGET(
        $token,
        $id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| token |  ``` Required ```  | token |
| id |  ``` Required ```  | id |



#### Example Usage

```php
$token = 'token';
$id = 75;

$result = $registerControler->getActivateUsingGET($token, $id);

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

```php
$creditConsumptionController = $client->getCreditConsumptionController();
```

### <a name="list_using_get2"></a>![Method: ](https://apidocs.io/img/method.png ".CreditConsumptionController.listUsingGET2") listUsingGET2

> *Tags:*  ``` Skips Authentication ``` 

> Get the consumption of the last months


```php
function listUsingGET2(
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';
$limit = 75;

$result = $creditConsumptionController->listUsingGET2($xAuthToken, $limit);

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


```php
function listPageUsingGET2(
        $page,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$page = 75;
$xAuthToken = 'X-Auth-Token';
$limit = 75;

$result = $creditConsumptionController->listPageUsingGET2($page, $xAuthToken, $limit);

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


```php
function getUsingGET1(
        $id,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$id = 75;
$xAuthToken = 'X-Auth-Token';

$result = $creditConsumptionController->getUsingGET1($id, $xAuthToken);

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

```php
$pricingController = $client->getPricingController();
```

### <a name="get_using_get7"></a>![Method: ](https://apidocs.io/img/method.png ".PricingController.getUsingGET7") getUsingGET7

> *Tags:*  ``` Skips Authentication ``` 

> get


```php
function getUsingGET7($xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';

$result = $pricingController->getUsingGET7($xAuthToken);

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

```php
$messageModelController = $client->getMessageModelController();
```

### <a name="list_using_get7"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.listUsingGET7") listUsingGET7

> *Tags:*  ``` Skips Authentication ``` 

> list


```php
function listUsingGET7(
        $xAuthToken,
        $size = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| size |  ``` Optional ```  | size |



#### Example Usage

```php
$xAuthToken = 'X-Auth-Token';
$size = 75;

$result = $messageModelController->listUsingGET7($xAuthToken, $size);

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


```php
function addUsingPOST3(
        $resource,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$resource = new MessageModelInputResourceModel();
$xAuthToken = 'X-Auth-Token';

$result = $messageModelController->addUsingPOST3($resource, $xAuthToken);

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


```php
function createDeleteMultipleUsingPOST(
        $ids,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ids |  ``` Required ```  ``` Collection ```  | ids |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$ids = array('ids');
$xAuthToken = 'X-Auth-Token';

$result = $messageModelController->createDeleteMultipleUsingPOST($ids, $xAuthToken);

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


```php
function listPageUsingGET7(
        $page,
        $xAuthToken,
        $limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```php
$page = 75;
$xAuthToken = 'X-Auth-Token';
$limit = 75;

$result = $messageModelController->listPageUsingGET7($page, $xAuthToken, $limit);

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


```php
function getUsingGET6(
        $id,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$id = 'id';
$xAuthToken = 'X-Auth-Token';

$result = $messageModelController->getUsingGET6($id, $xAuthToken);

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


```php
function updateUsingPUT3(
        $id,
        $resource,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$id = 'id';
$resource = new MessageModelInputResourceModel();
$xAuthToken = 'X-Auth-Token';

$messageModelController->updateUsingPUT3($id, $resource, $xAuthToken);

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


```php
function deleteUsingDELETE5(
        $id,
        $xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```php
$id = 'id';
$xAuthToken = 'X-Auth-Token';

$messageModelController->deleteUsingDELETE5($id, $xAuthToken);

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

```php
$societeInfoController = $client->getSocieteInfoController();
```

### <a name="create_research_company_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".SocieteInfoController.createResearchCompanyUsingPOST") createResearchCompanyUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> researchCompany


```php
function createResearchCompanyUsingPOST($research)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| research |  ``` Required ```  | research |



#### Example Usage

```php
$research = new SocieteInfoResearchResourceModel();

$result = $societeInfoController->createResearchCompanyUsingPOST($research);

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


```php
function getDetailsUsingGET($id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |



#### Example Usage

```php
$id = 'id';

$result = $societeInfoController->getDetailsUsingGET($id);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)



