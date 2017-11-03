# Getting started

sMsMode API-REST Documentation

## How to Build


The generated code has dependencies over external libraries like UniRest. These dependencies are defined in the ```PodFile``` file that comes with the SDK. 
To resolve these dependencies, we use the Cocoapods package manager.
Visit https://guides.cocoapods.org/using/getting-started.html to setup Cocoapods on your system.
Open command prompt and type ```pod --version```. This should display the current version of Cocoapods installed if the installation was successful.

Using command line, navigate to the directory containing the generated files (including ```PodFile```) for the SDK. 
Run the command ```pod install```. This should install all the required dependencies and create the ```pods``` directory in your project directory.

![Installing dependencies using Cocoapods](https://apidocs.io/illustration/objc?step=AddDependencies&workspaceFolder=sMsmode%20API-REST-ObjC&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST&rootNamespace=SMsmodeAPIREST)

Open the project workspace using the (SMsmodeAPIREST.xcworkspace) file. Invoke the build process using `Command(⌘)+B` shortcut key or using the `Build` menu as shown below.

![Building SDK using Xcode](https://apidocs.io/illustration/objc?step=BuildSDK&workspaceFolder=sMsmode%20API-REST-ObjC&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST&rootNamespace=SMsmodeAPIREST)


## How to Use

The generated code is a Cocoa Touch Static Library which can be used in any iOS project. The support for these generated libraries go all the way back to iOS 6.

The following section explains how to use the SMsmodeAPIREST library in a new iOS project.     
### 1. Starting a new project
To start a new project, left-click on the ```Create a new Xcode project```.
![Create Test Project - Step 1](https://apidocs.io/illustration/objc?step=Test1&workspaceFolder=sMsmode%20API-REST-ObjC&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST&rootNamespace=SMsmodeAPIREST)

Next, choose **Single View Application** and click ```Next```.
![Create Test Project - Step 2](https://apidocs.io/illustration/objc?step=Test2&workspaceFolder=sMsmode%20API-REST-ObjC&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST&rootNamespace=SMsmodeAPIREST)

Provide **Test-Project** as the product name click ```Next```.
![Create Test Project - Step 3](https://apidocs.io/illustration/objc?step=Test3&workspaceFolder=sMsmode%20API-REST-ObjC&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST&rootNamespace=SMsmodeAPIREST)

Choose the desired location of your project folder and click ```Create```.
![Create Test Project - Step 4](https://apidocs.io/illustration/objc?step=Test4&workspaceFolder=sMsmode%20API-REST-ObjC&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST&rootNamespace=SMsmodeAPIREST)

### 2. Adding the static library dependency
To add this dependency open a terminal and navigate to your project folder. Next, input ```pod init``` and press enter.
![Add dependency - Step 1](https://apidocs.io/illustration/objc?step=Add0&workspaceFolder=sMsmode%20API-REST-ObjC&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST&rootNamespace=SMsmodeAPIREST)

Next, open the newly created ```PodFile``` in your favourite text editor. Add the following line : pod 'SMsmodeAPIREST', :path => 'Vendor/SMsmodeAPIREST'
![Add dependency - Step 2](https://apidocs.io/illustration/objc?step=Add1&workspaceFolder=sMsmode%20API-REST-ObjC&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST&rootNamespace=SMsmodeAPIREST)

Execute `pod install` from terminal to install the dependecy in your project. This would add the dependency to the newly created test project.
![Add dependency - Step 3](https://apidocs.io/illustration/objc?step=Add2&workspaceFolder=sMsmode%20API-REST-ObjC&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST&rootNamespace=SMsmodeAPIREST)


## How to Test

Unit tests in this SDK can be run using Xcode. 

First build the SDK as shown in the steps above and naivgate to the project directory and open the SMsmodeAPIREST.xcworkspace file.

Go to the test explorer in Xcode as shown in the picture below and click on `run tests` from the menu. 
![Run tests](https://apidocs.io/illustration/objc?step=RunTests&workspaceFolder=sMsmode%20API-REST-ObjC&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST&rootNamespace=SMsmodeAPIREST)


## Initialization

### 

Configuration variables can be set as following.
```Objc

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
```objc
ReportController* reportController = [[ReportController alloc]init] ;
```

### <a name="list_using_get8_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.listUsingGET8AsyncWithXAuthToken") listUsingGET8AsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> list


```objc
function listUsingGET8AsyncWithXAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListUsingGET8) onCompleted(xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 90;

    [self.reportController listUsingGET8AsyncWithXAuthToken: xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get8_async_with_page"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.listPageUsingGET8AsyncWithPage") listPageUsingGET8AsyncWithPage

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```objc
function listPageUsingGET8AsyncWithPage:(int) page
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListPageUsingGET8) onCompleted(page xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    int page = 90;
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 90;

    [self.reportController listPageUsingGET8AsyncWithPage: page xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get8_async_with_message_ref"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.getUsingGET8AsyncWithMessageRef") getUsingGET8AsyncWithMessageRef

> *Tags:*  ``` Skips Authentication ``` 

> get


```objc
function getUsingGET8AsyncWithMessageRef:(NSString*) messageRef
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetUsingGET8) onCompleted(messageRef xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* messageRef = @"messageRef";
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 90;

    [self.reportController getUsingGET8AsyncWithMessageRef: messageRef xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_page_using_get_async_with_message_ref"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.getPageUsingGETAsyncWithMessageRef") getPageUsingGETAsyncWithMessageRef

> *Tags:*  ``` Skips Authentication ``` 

> getPage


```objc
function getPageUsingGETAsyncWithMessageRef:(NSString*) messageRef
                page:(int) page
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetPageUsingGET) onCompleted(messageRef page : page xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* messageRef = @"messageRef";
    int page = 90;
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 90;

    [self.reportController getPageUsingGETAsyncWithMessageRef: messageRef page : page xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="find_using_get_async_with_message_ref"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.findUsingGETAsyncWithMessageRef") findUsingGETAsyncWithMessageRef

> *Tags:*  ``` Skips Authentication ``` 

> find


```objc
function findUsingGETAsyncWithMessageRef:(NSString*) messageRef
                destinataire:(NSString*) destinataire
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedGetFindUsingGET) onCompleted(messageRef destinataire : destinataire xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| destinataire |  ``` Required ```  | destinataire |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* messageRef = @"messageRef";
    NSString* destinataire = @"destinataire";
    NSString* xAuthToken = @"X-Auth-Token";

    [self.reportController findUsingGETAsyncWithMessageRef: messageRef destinataire : destinataire xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
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
```objc
InvoiceController* invoiceController = [[InvoiceController alloc]init] ;
```

### <a name="list_using_get5_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".InvoiceController.listUsingGET5AsyncWithXAuthToken") listUsingGET5AsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> View a list of invoices


```objc
function listUsingGET5AsyncWithXAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListUsingGET5) onCompleted(xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 181;

    [self.invoiceController listUsingGET5AsyncWithXAuthToken: xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get5_async_with_page"></a>![Method: ](https://apidocs.io/img/method.png ".InvoiceController.listPageUsingGET5AsyncWithPage") listPageUsingGET5AsyncWithPage

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```objc
function listPageUsingGET5AsyncWithPage:(int) page
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListPageUsingGET5) onCompleted(page xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    int page = 181;
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 181;

    [self.invoiceController listPageUsingGET5AsyncWithPage: page xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_pdf_using_get_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".InvoiceController.getPdfUsingGETAsyncWithId") getPdfUsingGETAsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> Generate an invoice in a pdf file


```objc
function getPdfUsingGETAsyncWithId:(int) mid
                xAuthToken:(NSString*) xAuthToken
                base64:(BOOL) base64
                completionBlock:(CompletedGetPdfUsingGET) onCompleted(mid xAuthToken : xAuthToken base64 : base64)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| base64 |  ``` Required ```  | base64 |





#### Example Usage

```objc
    // Parameters for the API call
    int mid = 181;
    NSString* xAuthToken = @"X-Auth-Token";
    BOOL base64 = true;

    [self.invoiceController getPdfUsingGETAsyncWithId: mid xAuthToken : xAuthToken base64 : base64  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get5_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".InvoiceController.getUsingGET5AsyncWithId") getUsingGET5AsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> Show an invoice


```objc
function getUsingGET5AsyncWithId:(int) mid
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedGetUsingGET5) onCompleted(mid xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    int mid = 181;
    NSString* xAuthToken = @"X-Auth-Token";

    [self.invoiceController getUsingGET5AsyncWithId: mid xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, InvoiceResourceModel* response, NSError* error) { 
       //Add code here
    }];
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
```objc
AuthenticationController* authenticationController = [[AuthenticationController alloc]init] ;
```

### <a name="create_get_token_using_post_async_with_request"></a>![Method: ](https://apidocs.io/img/method.png ".AuthenticationController.createGetTokenUsingPOSTAsyncWithRequest") createGetTokenUsingPOSTAsyncWithRequest

> *Tags:*  ``` Skips Authentication ``` 

> Generate the OAuth Token


```objc
function createGetTokenUsingPOSTAsyncWithRequest:(AuthenticationResourceModel*) request
                completionBlock:(CompletedPostGetTokenUsingPOST) onCompleted(request)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| request |  ``` Required ```  | request |





#### Example Usage

```objc
    // Parameters for the API call
    AuthenticationResourceModel* request = [[AuthenticationResourceModel alloc]init];

    [self.authenticationController createGetTokenUsingPOSTAsyncWithRequest: request  completionBlock:^(BOOL success, HttpContext* context, TokenResourceModel* response, NSError* error) { 
       //Add code here
    }];
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
```objc
ContactController* contactController = [[ContactController alloc]init] ;
```

### <a name="list_using_get1_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.listUsingGET1AsyncWithXAuthToken") listUsingGET1AsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> View a list of contacts


```objc
function listUsingGET1AsyncWithXAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListUsingGET1) onCompleted(xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 181;

    [self.contactController listUsingGET1AsyncWithXAuthToken: xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="add_using_post_async_with_resource"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.addUsingPOSTAsyncWithResource") addUsingPOSTAsyncWithResource

> *Tags:*  ``` Skips Authentication ``` 

> Add a contact


```objc
function addUsingPOSTAsyncWithResource:(ContactResourceModel*) resource
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPostAddUsingPOST) onCompleted(resource xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    ContactResourceModel* resource = [[ContactResourceModel alloc]init];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.contactController addUsingPOSTAsyncWithResource: resource xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, ContactResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_book_using_delete_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.deleteBookUsingDELETEAsyncWithXAuthToken") deleteBookUsingDELETEAsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> Remove all contacts and groups of the account


```objc
function deleteBookUsingDELETEAsyncWithXAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedDeleteBookUsingDELETE) onCompleted(xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";

    [self.contactController deleteBookUsingDELETEAsyncWithXAuthToken: xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



### <a name="get_customer_info_using_get_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.getCustomerInfoUsingGETAsyncWithXAuthToken") getCustomerInfoUsingGETAsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> Show contact info of customer


```objc
function getCustomerInfoUsingGETAsyncWithXAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedGetCustomerInfoUsingGET) onCompleted(xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";

    [self.contactController getCustomerInfoUsingGETAsyncWithXAuthToken: xAuthToken  completionBlock:^(BOOL success, HttpContext* context, ContactResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_edit_customer_using_put_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.updateEditCustomerUsingPUTAsyncWithXAuthToken") updateEditCustomerUsingPUTAsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> Edit contact info of customer


```objc
function updateEditCustomerUsingPUTAsyncWithXAuthToken:(NSString*) xAuthToken
                resource:(ContactResourceModel*) resource
                completionBlock:(CompletedPutEditCustomerUsingPUT) onCompleted(xAuthToken resource : resource)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| resource |  ``` Required ```  | resource |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";
    ContactResourceModel* resource = [[ContactResourceModel alloc]init];

    [self.contactController updateEditCustomerUsingPUTAsyncWithXAuthToken: xAuthToken resource : resource  completionBlock:^(BOOL success, HttpContext* context, ContactResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_delete_list_using_post_async_with_id_list"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.createDeleteListUsingPOSTAsyncWithIdList") createDeleteListUsingPOSTAsyncWithIdList

> *Tags:*  ``` Skips Authentication ``` 

> Delete a list of contacts


```objc
function createDeleteListUsingPOSTAsyncWithIdList:(NSArray*) idList
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPostDeleteListUsingPOST) onCompleted(idList xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| idList |  ``` Required ```  ``` Collection ```  | idList |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* idList = @[181,181,181];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.contactController createDeleteListUsingPOSTAsyncWithIdList: idList xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_export_contacts_using_post_async_with_fields"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.createExportContactsUsingPOSTAsyncWithFields") createExportContactsUsingPOSTAsyncWithFields

> *Tags:*  ``` Skips Authentication ``` 

> Export contacts in csv format


```objc
function createExportContactsUsingPOSTAsyncWithFields:(NSArray*) fields
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPostExportContactsUsingPOST) onCompleted(fields xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fields |  ``` Required ```  ``` Collection ```  | fields |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* fields = @[@"fields",@"fields",@"fields"];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.contactController createExportContactsUsingPOSTAsyncWithFields: fields xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, DeferredResultResponseEntityObjectModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="upload_blocking_using_post_async_with_file"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.uploadBlockingUsingPOSTAsyncWithFile") uploadBlockingUsingPOSTAsyncWithFile

> *Tags:*  ``` Skips Authentication ``` 

> Import contacts via xls or csv files


```objc
function uploadBlockingUsingPOSTAsyncWithFile:(NSURL*) file
                model:(NSString*) model
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPostUploadBlockingUsingPOST) onCompleted(file model : model xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | file |
| model |  ``` Required ```  | model |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    NSURL* file = [NSURL URLWithString: @"pathtofile"];
    NSString* model = @"model";
    NSString* xAuthToken = @"X-Auth-Token";

    [self.contactController uploadBlockingUsingPOSTAsyncWithFile: file model : model xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, DeferredResultResponseEntityObjectModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get1_async_with_page"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.listPageUsingGET1AsyncWithPage") listPageUsingGET1AsyncWithPage

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```objc
function listPageUsingGET1AsyncWithPage:(int) page
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListPageUsingGET1) onCompleted(page xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    int page = 181;
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 181;

    [self.contactController listPageUsingGET1AsyncWithPage: page xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, ResourcesContactResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="search_using_get1_async_with_name"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.searchUsingGET1AsyncWithName") searchUsingGET1AsyncWithName

> *Tags:*  ``` Skips Authentication ``` 

> search


```objc
function searchUsingGET1AsyncWithName:(NSString*) name
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetSearchUsingGET1) onCompleted(name xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* name = @"name";
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 181;

    [self.contactController searchUsingGET1AsyncWithName: name xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.getUsingGETAsyncWithId") getUsingGETAsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> Show a contact


```objc
function getUsingGETAsyncWithId:(int) mid
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedGetUsingGET) onCompleted(mid xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    int mid = 181;
    NSString* xAuthToken = @"X-Auth-Token";

    [self.contactController getUsingGETAsyncWithId: mid xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, ContactResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_using_put_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.updateUsingPUTAsyncWithId") updateUsingPUTAsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> Update a contact


```objc
function updateUsingPUTAsyncWithId:(int) mid
                resource:(ContactResourceModel*) resource
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPutUpdateUsingPUT) onCompleted(mid resource : resource xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    int mid = 181;
    ContactResourceModel* resource = [[ContactResourceModel alloc]init];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.contactController updateUsingPUTAsyncWithId: mid resource : resource xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete1_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.deleteUsingDELETE1AsyncWithId") deleteUsingDELETE1AsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> Delete a contact


```objc
function deleteUsingDELETE1AsyncWithId:(int) mid
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedDeleteUsingDELETE1) onCompleted(mid xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    int mid = 181;
    NSString* xAuthToken = @"X-Auth-Token";

    [self.contactController deleteUsingDELETE1AsyncWithId: mid xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



### <a name="add_group_using_post_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.addGroupUsingPOSTAsyncWithId") addGroupUsingPOSTAsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> Add a contact in a group


```objc
function addGroupUsingPOSTAsyncWithId:(int) mid
                groupId:(int) groupId
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPostAddGroupUsingPOST) onCompleted(mid groupId : groupId xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| groupId |  ``` Required ```  | groupId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    int mid = 181;
    int groupId = 181;
    NSString* xAuthToken = @"X-Auth-Token";

    [self.contactController addGroupUsingPOSTAsyncWithId: mid groupId : groupId xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_groups_using_get_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.getGroupsUsingGETAsyncWithId") getGroupsUsingGETAsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups for a contact


```objc
function getGroupsUsingGETAsyncWithId:(int) mid
                page:(int) page
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetGroupsUsingGET) onCompleted(mid page : page xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    int mid = 181;
    int page = 181;
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 181;

    [self.contactController getGroupsUsingGETAsyncWithId: mid page : page xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_group_using_delete_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.deleteGroupUsingDELETEAsyncWithId") deleteGroupUsingDELETEAsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> Remove a contact from a group


```objc
function deleteGroupUsingDELETEAsyncWithId:(int) mid
                groupId:(int) groupId
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedDeleteGroupUsingDELETE) onCompleted(mid groupId : groupId xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| groupId |  ``` Required ```  | groupId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    int mid = 181;
    int groupId = 181;
    NSString* xAuthToken = @"X-Auth-Token";

    [self.contactController deleteGroupUsingDELETEAsyncWithId: mid groupId : groupId xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



[Back to List of Controllers](#list_of_controllers)

## <a name="customer_controller"></a>![Class: ](https://apidocs.io/img/class.png ".CustomerController") CustomerController

### Get singleton instance
```objc
CustomerController* customerController = [[CustomerController alloc]init] ;
```

### <a name="get_using_get2_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.getUsingGET2AsyncWithXAuthToken") getUsingGET2AsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> Show your account


```objc
function getUsingGET2AsyncWithXAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedGetUsingGET2) onCompleted(xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";

    [self.customerController getUsingGET2AsyncWithXAuthToken: xAuthToken  completionBlock:^(BOOL success, HttpContext* context, CustomerResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_from_fields_using_get_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.getFromFieldsUsingGETAsyncWithXAuthToken") getFromFieldsUsingGETAsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> Get your personnalized sender IDs


```objc
function getFromFieldsUsingGETAsyncWithXAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedGetFromFieldsUsingGET) onCompleted(xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";

    [self.customerController getFromFieldsUsingGETAsyncWithXAuthToken: xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_delete_sender_using_put_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.updateDeleteSenderUsingPUTAsyncWithXAuthToken") updateDeleteSenderUsingPUTAsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> Remove sender ID


```objc
function updateDeleteSenderUsingPUTAsyncWithXAuthToken:(NSString*) xAuthToken
                senderID:(NSString*) senderID
                completionBlock:(CompletedPutDeleteSenderUsingPUT) onCompleted(xAuthToken senderID : senderID)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| senderID |  ``` Required ```  | senderID |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";
    NSString* senderID = @"senderID";

    [self.customerController updateDeleteSenderUsingPUTAsyncWithXAuthToken: xAuthToken senderID : senderID  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="add_sender_using_post_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.addSenderUsingPOSTAsyncWithXAuthToken") addSenderUsingPOSTAsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> Add personnalized sender ID


```objc
function addSenderUsingPOSTAsyncWithXAuthToken:(NSString*) xAuthToken
                senderID:(NSString*) senderID
                completionBlock:(CompletedPostAddSenderUsingPOST) onCompleted(xAuthToken senderID : senderID)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| senderID |  ``` Required ```  | senderID |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";
    NSString* senderID = @"senderID";

    [self.customerController addSenderUsingPOSTAsyncWithXAuthToken: xAuthToken senderID : senderID  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_using_get3_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.listUsingGET3AsyncWithXAuthToken") listUsingGET3AsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> View a list of your subaccounts


```objc
function listUsingGET3AsyncWithXAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListUsingGET3) onCompleted(xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 181;

    [self.customerController listUsingGET3AsyncWithXAuthToken: xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get3_async_with_page"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.listPageUsingGET3AsyncWithPage") listPageUsingGET3AsyncWithPage

> *Tags:*  ``` Skips Authentication ``` 

> View a list of your subaccounts by page


```objc
function listPageUsingGET3AsyncWithPage:(int) page
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListPageUsingGET3) onCompleted(page xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    int page = 181;
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 181;

    [self.customerController listPageUsingGET3AsyncWithPage: page xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
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
```objc
GroupController* groupController = [[GroupController alloc]init] ;
```

### <a name="list_using_get4_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.listUsingGET4AsyncWithXAuthToken") listUsingGET4AsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups


```objc
function listUsingGET4AsyncWithXAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListUsingGET4) onCompleted(xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 181;

    [self.groupController listUsingGET4AsyncWithXAuthToken: xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="add_using_post2_async_with_resource"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.addUsingPOST2AsyncWithResource") addUsingPOST2AsyncWithResource

> *Tags:*  ``` Skips Authentication ``` 

> Add a group


```objc
function addUsingPOST2AsyncWithResource:(GroupResourceModel*) resource
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPostAddUsingPOST2) onCompleted(resource xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    GroupResourceModel* resource = [[GroupResourceModel alloc]init];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.groupController addUsingPOST2AsyncWithResource: resource xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, GroupResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_delete_list_using_post1_async_with_id_list"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.createDeleteListUsingPOST1AsyncWithIdList") createDeleteListUsingPOST1AsyncWithIdList

> *Tags:*  ``` Skips Authentication ``` 

> Delete a list of groups


```objc
function createDeleteListUsingPOST1AsyncWithIdList:(NSArray*) idList
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPostDeleteListUsingPOST1) onCompleted(idList xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| idList |  ``` Required ```  ``` Collection ```  | idList |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* idList = @[181,181,181];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.groupController createDeleteListUsingPOST1AsyncWithIdList: idList xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get4_async_with_page"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.listPageUsingGET4AsyncWithPage") listPageUsingGET4AsyncWithPage

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```objc
function listPageUsingGET4AsyncWithPage:(int) page
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListPageUsingGET4) onCompleted(page xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    int page = 181;
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 181;

    [self.groupController listPageUsingGET4AsyncWithPage: page xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="search_using_get2_async_with_name"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.searchUsingGET2AsyncWithName") searchUsingGET2AsyncWithName

> *Tags:*  ``` Skips Authentication ``` 

> search


```objc
function searchUsingGET2AsyncWithName:(NSString*) name
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetSearchUsingGET2) onCompleted(name xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* name = @"name";
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 181;

    [self.groupController searchUsingGET2AsyncWithName: name xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get4_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.getUsingGET4AsyncWithId") getUsingGET4AsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> Show a group


```objc
function getUsingGET4AsyncWithId:(int) mid
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedGetUsingGET4) onCompleted(mid xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    int mid = 181;
    NSString* xAuthToken = @"X-Auth-Token";

    [self.groupController getUsingGET4AsyncWithId: mid xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, GroupResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_using_put2_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.updateUsingPUT2AsyncWithId") updateUsingPUT2AsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> Update a group


```objc
function updateUsingPUT2AsyncWithId:(int) mid
                resource:(GroupResourceModel*) resource
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPutUpdateUsingPUT2) onCompleted(mid resource : resource xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    int mid = 139;
    GroupResourceModel* resource = [[GroupResourceModel alloc]init];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.groupController updateUsingPUT2AsyncWithId: mid resource : resource xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete3_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.deleteUsingDELETE3AsyncWithId") deleteUsingDELETE3AsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> Delete a group


```objc
function deleteUsingDELETE3AsyncWithId:(int) mid
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedDeleteUsingDELETE3) onCompleted(mid xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    int mid = 139;
    NSString* xAuthToken = @"X-Auth-Token";

    [self.groupController deleteUsingDELETE3AsyncWithId: mid xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



### <a name="get_contacts_using_get_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.getContactsUsingGETAsyncWithId") getContactsUsingGETAsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> Show a list of contacts for a group


```objc
function getContactsUsingGETAsyncWithId:(int) mid
                page:(int) page
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetContactsUsingGET) onCompleted(mid page : page xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    int mid = 139;
    int page = 139;
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 139;

    [self.groupController getContactsUsingGETAsyncWithId: mid page : page xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, GroupResourceModel* response, NSError* error) { 
       //Add code here
    }];
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
```objc
CampaignController* campaignController = [[CampaignController alloc]init] ;
```

### <a name="list_using_get_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.listUsingGETAsyncWithXAuthToken") listUsingGETAsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> list


```objc
function listUsingGETAsyncWithXAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListUsingGET) onCompleted(xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 139;

    [self.campaignController listUsingGETAsyncWithXAuthToken: xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_send_to_list_using_post_async_with_resource"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.createSendToListUsingPOSTAsyncWithResource") createSendToListUsingPOSTAsyncWithResource

> *Tags:*  ``` Skips Authentication ``` 

> sendToList


```objc
function createSendToListUsingPOSTAsyncWithResource:(CampaignInputResourceModel*) resource
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPostSendToListUsingPOST) onCompleted(resource xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    CampaignInputResourceModel* resource = [[CampaignInputResourceModel alloc]init];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.campaignController createSendToListUsingPOSTAsyncWithResource: resource xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get_async_with_page"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.listPageUsingGETAsyncWithPage") listPageUsingGETAsyncWithPage

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```objc
function listPageUsingGETAsyncWithPage:(int) page
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListPageUsingGET) onCompleted(page xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    int page = 139;
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 139;

    [self.campaignController listPageUsingGETAsyncWithPage: page xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="search_using_get_async_with_name"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.searchUsingGETAsyncWithName") searchUsingGETAsyncWithName

> *Tags:*  ``` Skips Authentication ``` 

> search


```objc
function searchUsingGETAsyncWithName:(NSString*) name
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetSearchUsingGET) onCompleted(name xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* name = @"name";
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 139;

    [self.campaignController searchUsingGETAsyncWithName: name xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete_async_with_messsage_id"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.deleteUsingDELETEAsyncWithMesssageId") deleteUsingDELETEAsyncWithMesssageId

> *Tags:*  ``` Skips Authentication ``` 

> delete


```objc
function deleteUsingDELETEAsyncWithMesssageId:(NSString*) messsageId
                xAuthToken:(NSString*) xAuthToken
                mid:(NSString*) mid
                completionBlock:(CompletedDeleteUsingDELETE) onCompleted(messsageId xAuthToken : xAuthToken mid : mid)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsageId |  ``` Required ```  | messsageId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| mid |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* messsageId = @"messsageId";
    NSString* xAuthToken = @"X-Auth-Token";
    NSString* mid = @"id";

    [self.campaignController deleteUsingDELETEAsyncWithMesssageId: messsageId xAuthToken : xAuthToken mid : mid  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



[Back to List of Controllers](#list_of_controllers)

## <a name="transfer_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TransferController") TransferController

### Get singleton instance
```objc
TransferController* transferController = [[TransferController alloc]init] ;
```

### <a name="list_using_get9_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".TransferController.listUsingGET9AsyncWithXAuthToken") listUsingGET9AsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> View a list of transferts


```objc
function listUsingGET9AsyncWithXAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListUsingGET9) onCompleted(xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 139;

    [self.transferController listUsingGET9AsyncWithXAuthToken: xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get9_async_with_page"></a>![Method: ](https://apidocs.io/img/method.png ".TransferController.listPageUsingGET9AsyncWithPage") listPageUsingGET9AsyncWithPage

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```objc
function listPageUsingGET9AsyncWithPage:(int) page
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListPageUsingGET9) onCompleted(page xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    int page = 139;
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 139;

    [self.transferController listPageUsingGET9AsyncWithPage: page xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get9_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".TransferController.getUsingGET9AsyncWithId") getUsingGET9AsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> Show a transfet


```objc
function getUsingGET9AsyncWithId:(int) mid
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedGetUsingGET9) onCompleted(mid xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    int mid = 139;
    NSString* xAuthToken = @"X-Auth-Token";

    [self.transferController getUsingGET9AsyncWithId: mid xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, TransferResourceModel* response, NSError* error) { 
       //Add code here
    }];
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
```objc
EmailApiConfigurationController* emailApiConfigurationController = [[EmailApiConfigurationController alloc]init] ;
```

### <a name="get_using_get3_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".EmailApiConfigurationController.getUsingGET3AsyncWithXAuthToken") getUsingGET3AsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> Show your configuration


```objc
function getUsingGET3AsyncWithXAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedGetUsingGET3) onCompleted(xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";

    [self.emailApiConfigurationController getUsingGET3AsyncWithXAuthToken: xAuthToken  completionBlock:^(BOOL success, HttpContext* context, EmailAPIConfigurationResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_using_put1_async_with_resource"></a>![Method: ](https://apidocs.io/img/method.png ".EmailApiConfigurationController.updateUsingPUT1AsyncWithResource") updateUsingPUT1AsyncWithResource

> *Tags:*  ``` Skips Authentication ``` 

> Update your configuration


```objc
function updateUsingPUT1AsyncWithResource:(EmailAPIConfigurationResourceModel*) resource
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPutUpdateUsingPUT1) onCompleted(resource xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    EmailAPIConfigurationResourceModel* resource = [[EmailAPIConfigurationResourceModel alloc]init];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.emailApiConfigurationController updateUsingPUT1AsyncWithResource: resource xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="add_using_post1_async_with_resource"></a>![Method: ](https://apidocs.io/img/method.png ".EmailApiConfigurationController.addUsingPOST1AsyncWithResource") addUsingPOST1AsyncWithResource

> *Tags:*  ``` Skips Authentication ``` 

> Create your configuration


```objc
function addUsingPOST1AsyncWithResource:(EmailAPIConfigurationResourceModel*) resource
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPostAddUsingPOST1) onCompleted(resource xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    EmailAPIConfigurationResourceModel* resource = [[EmailAPIConfigurationResourceModel alloc]init];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.emailApiConfigurationController addUsingPOST1AsyncWithResource: resource xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, EmailAPIConfigurationResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete2_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".EmailApiConfigurationController.deleteUsingDELETE2AsyncWithXAuthToken") deleteUsingDELETE2AsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> Delete your configuration


```objc
function deleteUsingDELETE2AsyncWithXAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedDeleteUsingDELETE2) onCompleted(xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";

    [self.emailApiConfigurationController deleteUsingDELETE2AsyncWithXAuthToken: xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



[Back to List of Controllers](#list_of_controllers)

## <a name="message_controller"></a>![Class: ](https://apidocs.io/img/class.png ".MessageController") MessageController

### Get singleton instance
```objc
MessageController* messageController = [[MessageController alloc]init] ;
```

### <a name="list_using_get6_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.listUsingGET6AsyncWithXAuthToken") listUsingGET6AsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> list


```objc
function listUsingGET6AsyncWithXAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListUsingGET6) onCompleted(xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 139;

    [self.messageController listUsingGET6AsyncWithXAuthToken: xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get6_async_with_page"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.listPageUsingGET6AsyncWithPage") listPageUsingGET6AsyncWithPage

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```objc
function listPageUsingGET6AsyncWithPage:(int) page
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListPageUsingGET6) onCompleted(page xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    int page = 139;
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 139;

    [self.messageController listPageUsingGET6AsyncWithPage: page xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, PagedResourcesMessageResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_responses_using_get_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.listResponsesUsingGETAsyncWithXAuthToken") listResponsesUsingGETAsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> listResponses


```objc
function listResponsesUsingGETAsyncWithXAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListResponsesUsingGET) onCompleted(xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 139;

    [self.messageController listResponsesUsingGETAsyncWithXAuthToken: xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, ResourcesMessageResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_responses_page_using_get_async_with_page"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.listResponsesPageUsingGETAsyncWithPage") listResponsesPageUsingGETAsyncWithPage

> *Tags:*  ``` Skips Authentication ``` 

> listResponsesPage


```objc
function listResponsesPageUsingGETAsyncWithPage:(int) page
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListResponsesPageUsingGET) onCompleted(page xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    int page = 139;
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 139;

    [self.messageController listResponsesPageUsingGETAsyncWithPage: page xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, PagedResourcesMessageResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_scheduled_using_get_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.listScheduledUsingGETAsyncWithXAuthToken") listScheduledUsingGETAsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> listScheduled


```objc
function listScheduledUsingGETAsyncWithXAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListScheduledUsingGET) onCompleted(xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 139;

    [self.messageController listScheduledUsingGETAsyncWithXAuthToken: xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, ResourcesMessageResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_scheduled_page_using_get_async_with_page"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.listScheduledPageUsingGETAsyncWithPage") listScheduledPageUsingGETAsyncWithPage

> *Tags:*  ``` Skips Authentication ``` 

> listScheduledPage


```objc
function listScheduledPageUsingGETAsyncWithPage:(int) page
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListScheduledPageUsingGET) onCompleted(page xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    int page = 139;
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 139;

    [self.messageController listScheduledPageUsingGETAsyncWithPage: page xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, PagedResourcesMessageResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="search_using_get3_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.searchUsingGET3AsyncWithId") searchUsingGET3AsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> search


```objc
function searchUsingGET3AsyncWithId:(NSString*) mid
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetSearchUsingGET3) onCompleted(mid xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* mid = @"id";
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 139;

    [self.messageController searchUsingGET3AsyncWithId: mid xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_send_to_list_using_post1_async_with_resource"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.createSendToListUsingPOST1AsyncWithResource") createSendToListUsingPOST1AsyncWithResource

> *Tags:*  ``` Skips Authentication ``` 

> sendToList


```objc
function createSendToListUsingPOST1AsyncWithResource:(MessageInputMixedResourceModel*) resource
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPostSendToListUsingPOST1) onCompleted(resource xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    MessageInputMixedResourceModel* resource = [[MessageInputMixedResourceModel alloc]init];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.messageController createSendToListUsingPOST1AsyncWithResource: resource xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_send_to_contact_list_using_post_async_with_resource"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.createSendToContactListUsingPOSTAsyncWithResource") createSendToContactListUsingPOSTAsyncWithResource

> *Tags:*  ``` Skips Authentication ``` 

> sendToContactList


```objc
function createSendToContactListUsingPOSTAsyncWithResource:(MessageInputContactResourceModel*) resource
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPostSendToContactListUsingPOST) onCompleted(resource xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    MessageInputContactResourceModel* resource = [[MessageInputContactResourceModel alloc]init];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.messageController createSendToContactListUsingPOSTAsyncWithResource: resource xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_send_to_group_list_using_post_async_with_resource"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.createSendToGroupListUsingPOSTAsyncWithResource") createSendToGroupListUsingPOSTAsyncWithResource

> *Tags:*  ``` Skips Authentication ``` 

> sendToGroupList


```objc
function createSendToGroupListUsingPOSTAsyncWithResource:(MessageInputGroupResourceModel*) resource
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPostSendToGroupListUsingPOST) onCompleted(resource xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    MessageInputGroupResourceModel* resource = [[MessageInputGroupResourceModel alloc]init];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.messageController createSendToGroupListUsingPOSTAsyncWithResource: resource xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_send_to_number_list_using_post_async_with_resource"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.createSendToNumberListUsingPOSTAsyncWithResource") createSendToNumberListUsingPOSTAsyncWithResource

> *Tags:*  ``` Skips Authentication ``` 

> sendToNumberList


```objc
function createSendToNumberListUsingPOSTAsyncWithResource:(MessageInputResourceModel*) resource
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPostSendToNumberListUsingPOST) onCompleted(resource xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    MessageInputResourceModel* resource = [[MessageInputResourceModel alloc]init];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.messageController createSendToNumberListUsingPOSTAsyncWithResource: resource xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete4_async_with_messsage_id"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.deleteUsingDELETE4AsyncWithMesssageId") deleteUsingDELETE4AsyncWithMesssageId

> *Tags:*  ``` Skips Authentication ``` 

> delete


```objc
function deleteUsingDELETE4AsyncWithMesssageId:(NSString*) messsageId
                xAuthToken:(NSString*) xAuthToken
                mid:(NSString*) mid
                completionBlock:(CompletedDeleteUsingDELETE4) onCompleted(messsageId xAuthToken : xAuthToken mid : mid)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsageId |  ``` Required ```  | messsageId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| mid |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* messsageId = @"messsageId";
    NSString* xAuthToken = @"X-Auth-Token";
    NSString* mid = @"id";

    [self.messageController deleteUsingDELETE4AsyncWithMesssageId: messsageId xAuthToken : xAuthToken mid : mid  completionBlock:^(BOOL success, HttpContext* context, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



[Back to List of Controllers](#list_of_controllers)

## <a name="register_controler_controller"></a>![Class: ](https://apidocs.io/img/class.png ".RegisterControlerController") RegisterControlerController

### Get singleton instance
```objc
RegisterControler* registerControler = [[RegisterControler alloc]init] ;
```

### <a name="create_register_using_post_async_with_resource"></a>![Method: ](https://apidocs.io/img/method.png ".RegisterControlerController.createRegisterUsingPOSTAsyncWithResource") createRegisterUsingPOSTAsyncWithResource

> *Tags:*  ``` Skips Authentication ``` 

> register


```objc
function createRegisterUsingPOSTAsyncWithResource:(RegisterResourceModel*) resource
                completionBlock:(CompletedPostRegisterUsingPOST) onCompleted(resource)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |





#### Example Usage

```objc
    // Parameters for the API call
    RegisterResourceModel* resource = [[RegisterResourceModel alloc]init];

    [self.registerControler createRegisterUsingPOSTAsyncWithResource: resource  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_refresh_using_post_async_with_resource"></a>![Method: ](https://apidocs.io/img/method.png ".RegisterControlerController.createRefreshUsingPOSTAsyncWithResource") createRefreshUsingPOSTAsyncWithResource

> *Tags:*  ``` Skips Authentication ``` 

> refresh


```objc
function createRefreshUsingPOSTAsyncWithResource:(SimpleEmailResourceModel*) resource
                completionBlock:(CompletedPostRefreshUsingPOST) onCompleted(resource)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |





#### Example Usage

```objc
    // Parameters for the API call
    SimpleEmailResourceModel* resource = [[SimpleEmailResourceModel alloc]init];

    [self.registerControler createRefreshUsingPOSTAsyncWithResource: resource  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_activate_using_get_async_with_token"></a>![Method: ](https://apidocs.io/img/method.png ".RegisterControlerController.getActivateUsingGETAsyncWithToken") getActivateUsingGETAsyncWithToken

> *Tags:*  ``` Skips Authentication ``` 

> activate


```objc
function getActivateUsingGETAsyncWithToken:(NSString*) token
                mid:(int) mid
                completionBlock:(CompletedGetActivateUsingGET) onCompleted(token mid : mid)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| token |  ``` Required ```  | token |
| mid |  ``` Required ```  | id |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* token = @"token";
    int mid = 139;

    [self.registerControler getActivateUsingGETAsyncWithToken: token mid : mid  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
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
```objc
CreditConsumptionController* creditConsumptionController = [[CreditConsumptionController alloc]init] ;
```

### <a name="list_using_get2_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".CreditConsumptionController.listUsingGET2AsyncWithXAuthToken") listUsingGET2AsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> Get the consumption of the last months


```objc
function listUsingGET2AsyncWithXAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListUsingGET2) onCompleted(xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 139;

    [self.creditConsumptionController listUsingGET2AsyncWithXAuthToken: xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get2_async_with_page"></a>![Method: ](https://apidocs.io/img/method.png ".CreditConsumptionController.listPageUsingGET2AsyncWithPage") listPageUsingGET2AsyncWithPage

> *Tags:*  ``` Skips Authentication ``` 

> Get pageable consumption of the last months


```objc
function listPageUsingGET2AsyncWithPage:(int) page
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListPageUsingGET2) onCompleted(page xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    int page = 139;
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 139;

    [self.creditConsumptionController listPageUsingGET2AsyncWithPage: page xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get1_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".CreditConsumptionController.getUsingGET1AsyncWithId") getUsingGET1AsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> Get specific consumption by id 


```objc
function getUsingGET1AsyncWithId:(int) mid
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedGetUsingGET1) onCompleted(mid xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    int mid = 139;
    NSString* xAuthToken = @"X-Auth-Token";

    [self.creditConsumptionController getUsingGET1AsyncWithId: mid xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
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
```objc
PricingController* pricingController = [[PricingController alloc]init] ;
```

### <a name="get_using_get7_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".PricingController.getUsingGET7AsyncWithXAuthToken") getUsingGET7AsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> get


```objc
function getUsingGET7AsyncWithXAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedGetUsingGET7) onCompleted(xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";

    [self.pricingController getUsingGET7AsyncWithXAuthToken: xAuthToken  completionBlock:^(BOOL success, HttpContext* context, PricingResourceModel* response, NSError* error) { 
       //Add code here
    }];
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
```objc
MessageModelController* messageModelController = [[MessageModelController alloc]init] ;
```

### <a name="list_using_get7_async_with_x_auth_token"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.listUsingGET7AsyncWithXAuthToken") listUsingGET7AsyncWithXAuthToken

> *Tags:*  ``` Skips Authentication ``` 

> list


```objc
function listUsingGET7AsyncWithXAuthToken:(NSString*) xAuthToken
                size:(NSNumber*) size
                completionBlock:(CompletedGetListUsingGET7) onCompleted(xAuthToken size : size)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| size |  ``` Optional ```  | size |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* size = 139;

    [self.messageModelController listUsingGET7AsyncWithXAuthToken: xAuthToken size : size  completionBlock:^(BOOL success, HttpContext* context, ResourcesMessageModelResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="add_using_post3_async_with_resource"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.addUsingPOST3AsyncWithResource") addUsingPOST3AsyncWithResource

> *Tags:*  ``` Skips Authentication ``` 

> add


```objc
function addUsingPOST3AsyncWithResource:(MessageModelInputResourceModel*) resource
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPostAddUsingPOST3) onCompleted(resource xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    MessageModelInputResourceModel* resource = [[MessageModelInputResourceModel alloc]init];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.messageModelController addUsingPOST3AsyncWithResource: resource xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, MessageModelResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_delete_multiple_using_post_async_with_ids"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.createDeleteMultipleUsingPOSTAsyncWithIds") createDeleteMultipleUsingPOSTAsyncWithIds

> *Tags:*  ``` Skips Authentication ``` 

> deleteMultiple


```objc
function createDeleteMultipleUsingPOSTAsyncWithIds:(NSArray*) ids
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPostDeleteMultipleUsingPOST) onCompleted(ids xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ids |  ``` Required ```  ``` Collection ```  | ids |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* ids = @[@"ids",@"ids",@"ids"];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.messageModelController createDeleteMultipleUsingPOSTAsyncWithIds: ids xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get7_async_with_page"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.listPageUsingGET7AsyncWithPage") listPageUsingGET7AsyncWithPage

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```objc
function listPageUsingGET7AsyncWithPage:(int) page
                xAuthToken:(NSString*) xAuthToken
                limit:(NSNumber*) limit
                completionBlock:(CompletedGetListPageUsingGET7) onCompleted(page xAuthToken : xAuthToken limit : limit)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |





#### Example Usage

```objc
    // Parameters for the API call
    int page = 139;
    NSString* xAuthToken = @"X-Auth-Token";
    NSNumber* limit = 139;

    [self.messageModelController listPageUsingGET7AsyncWithPage: page xAuthToken : xAuthToken limit : limit  completionBlock:^(BOOL success, HttpContext* context, PagedResourcesMessageModelResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get6_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.getUsingGET6AsyncWithId") getUsingGET6AsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> get


```objc
function getUsingGET6AsyncWithId:(NSString*) mid
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedGetUsingGET6) onCompleted(mid xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* mid = @"id";
    NSString* xAuthToken = @"X-Auth-Token";

    [self.messageModelController getUsingGET6AsyncWithId: mid xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, MessageModelResourceModel* response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_using_put3_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.updateUsingPUT3AsyncWithId") updateUsingPUT3AsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> update


```objc
function updateUsingPUT3AsyncWithId:(NSString*) mid
                resource:(MessageModelInputResourceModel*) resource
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedPutUpdateUsingPUT3) onCompleted(mid resource : resource xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* mid = @"id";
    MessageModelInputResourceModel* resource = [[MessageModelInputResourceModel alloc]init];
    NSString* xAuthToken = @"X-Auth-Token";

    [self.messageModelController updateUsingPUT3AsyncWithId: mid resource : resource xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete5_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.deleteUsingDELETE5AsyncWithId") deleteUsingDELETE5AsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> delete


```objc
function deleteUsingDELETE5AsyncWithId:(NSString*) mid
                xAuthToken:(NSString*) xAuthToken
                completionBlock:(CompletedDeleteUsingDELETE5) onCompleted(mid xAuthToken : xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* mid = @"id";
    NSString* xAuthToken = @"X-Auth-Token";

    [self.messageModelController deleteUsingDELETE5AsyncWithId: mid xAuthToken : xAuthToken  completionBlock:^(BOOL success, HttpContext* context, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



[Back to List of Controllers](#list_of_controllers)

## <a name="societe_info_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SocieteInfoController") SocieteInfoController

### Get singleton instance
```objc
SocieteInfoController* societeInfoController = [[SocieteInfoController alloc]init] ;
```

### <a name="create_research_company_using_post_async_with_research"></a>![Method: ](https://apidocs.io/img/method.png ".SocieteInfoController.createResearchCompanyUsingPOSTAsyncWithResearch") createResearchCompanyUsingPOSTAsyncWithResearch

> *Tags:*  ``` Skips Authentication ``` 

> researchCompany


```objc
function createResearchCompanyUsingPOSTAsyncWithResearch:(SocieteInfoResearchResourceModel*) research
                completionBlock:(CompletedPostResearchCompanyUsingPOST) onCompleted(research)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| research |  ``` Required ```  | research |





#### Example Usage

```objc
    // Parameters for the API call
    SocieteInfoResearchResourceModel* research = [[SocieteInfoResearchResourceModel alloc]init];

    [self.societeInfoController createResearchCompanyUsingPOSTAsyncWithResearch: research  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_details_using_get_async_with_id"></a>![Method: ](https://apidocs.io/img/method.png ".SocieteInfoController.getDetailsUsingGETAsyncWithId") getDetailsUsingGETAsyncWithId

> *Tags:*  ``` Skips Authentication ``` 

> getDetails


```objc
function getDetailsUsingGETAsyncWithId:(NSString*) mid
                completionBlock:(CompletedGetDetailsUsingGET) onCompleted(mid)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mid |  ``` Required ```  | id |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* mid = @"id";

    [self.societeInfoController getDetailsUsingGETAsyncWithId: mid  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)



