# Getting started

sMsMode API-REST Documentation

## How to Build

The generated code uses the Newtonsoft Json.NET NuGet Package. If the automatic NuGet package restore
is enabled, these dependencies will be installed automatically. Therefore,
you will need internet access for build.

1. Open the solution (SMsmodeAPIREST.sln) file.
2. Invoke the build process using `Ctrl+Shift+B` shortcut key or using the `Build` menu as shown below.

![Building SDK using Visual Studio](https://apidocs.io/illustration/cs?step=buildSDK&workspaceFolder=sMsmode%20API-REST-CSharp&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST.PCL)

## How to Use

The build process generates a portable class library, which can be used like a normal class library. The generated library is compatible with Windows Forms, Windows RT, Windows Phone 8,
Silverlight 5, Xamarin iOS, Xamarin Android and Mono. More information on how to use can be found at the [MSDN Portable Class Libraries documentation](http://msdn.microsoft.com/en-us/library/vstudio/gg597391%28v=vs.100%29.aspx).

The following section explains how to use the SMsmodeAPIREST library in a new console project.

### 1. Starting a new project

For starting a new project, right click on the current solution from the *solution explorer* and choose  ``` Add -> New Project ```.

![Add a new project in the existing solution using Visual Studio](https://apidocs.io/illustration/cs?step=addProject&workspaceFolder=sMsmode%20API-REST-CSharp&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST.PCL)

Next, choose "Console Application", provide a ``` TestConsoleProject ``` as the project name and click ``` OK ```.

![Create a new console project using Visual Studio](https://apidocs.io/illustration/cs?step=createProject&workspaceFolder=sMsmode%20API-REST-CSharp&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST.PCL)

### 2. Set as startup project

The new console project is the entry point for the eventual execution. This requires us to set the ``` TestConsoleProject ``` as the start-up project. To do this, right-click on the  ``` TestConsoleProject ``` and choose  ``` Set as StartUp Project ``` form the context menu.

![Set the new cosole project as the start up project](https://apidocs.io/illustration/cs?step=setStartup&workspaceFolder=sMsmode%20API-REST-CSharp&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST.PCL)

### 3. Add reference of the library project

In order to use the SMsmodeAPIREST library in the new project, first we must add a projet reference to the ``` TestConsoleProject ```. First, right click on the ``` References ``` node in the *solution explorer* and click ``` Add Reference... ```.

![Open references of the TestConsoleProject](https://apidocs.io/illustration/cs?step=addReference&workspaceFolder=sMsmode%20API-REST-CSharp&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST.PCL)

Next, a window will be displayed where we must set the ``` checkbox ``` on ``` SMsmodeAPIREST.PCL ``` and click ``` OK ```. By doing this, we have added a reference of the ```SMsmodeAPIREST.PCL``` project into the new ``` TestConsoleProject ```.

![Add a reference to the TestConsoleProject](https://apidocs.io/illustration/cs?step=createReference&workspaceFolder=sMsmode%20API-REST-CSharp&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST.PCL)

### 4. Write sample code

Once the ``` TestConsoleProject ``` is created, a file named ``` Program.cs ``` will be visible in the *solution explorer* with an empty ``` Main ``` method. This is the entry point for the execution of the entire solution.
Here, you can add code to initialize the client library and acquire the instance of a *Controller* class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

![Add a reference to the TestConsoleProject](https://apidocs.io/illustration/cs?step=addCode&workspaceFolder=sMsmode%20API-REST-CSharp&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIREST.PCL)

## How to Test

The generated SDK also contain one or more Tests, which are contained in the Tests project.
In order to invoke these test cases, you will need *NUnit 3.0 Test Adapter Extension for Visual Studio*.
Once the SDK is complied, the test cases should appear in the Test Explorer window.
Here, you can click *Run All* to execute these test cases.

## Initialization

### 

API client can be initialized as following.

```csharp

SMsmodeAPIRESTClient client = new SMsmodeAPIRESTClient();
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

## <a name="report_controller"></a>![Class: ](https://apidocs.io/img/class.png "SMsmodeAPIREST.PCL.Controllers.ReportController") ReportController

### Get singleton instance

The singleton instance of the ``` ReportController ``` class can be accessed from the API Client.

```csharp
ReportController reportController = client.ReportController;
```

### <a name="list_using_get8"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ReportController.ListUsingGET8") ListUsingGET8

> *Tags:*  ``` Skips Authentication ``` 

> list


```csharp
Task<dynamic> ListUsingGET8(string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";
int? limit = 176;

dynamic result = await reportController.ListUsingGET8(xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="list_page_using_get8"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ReportController.ListPageUsingGET8") ListPageUsingGET8

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```csharp
Task<dynamic> ListPageUsingGET8(int page, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
int page = 176;
string xAuthToken = "X-Auth-Token";
int? limit = 176;

dynamic result = await reportController.ListPageUsingGET8(page, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="get_using_get8"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ReportController.GetUsingGET8") GetUsingGET8

> *Tags:*  ``` Skips Authentication ``` 

> get


```csharp
Task<dynamic> GetUsingGET8(string messageRef, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string messageRef = "messageRef";
string xAuthToken = "X-Auth-Token";
int? limit = 176;

dynamic result = await reportController.GetUsingGET8(messageRef, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="get_page_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ReportController.GetPageUsingGET") GetPageUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> getPage


```csharp
Task<dynamic> GetPageUsingGET(
        string messageRef,
        int page,
        string xAuthToken,
        int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string messageRef = "messageRef";
int page = 176;
string xAuthToken = "X-Auth-Token";
int? limit = 176;

dynamic result = await reportController.GetPageUsingGET(messageRef, page, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="find_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ReportController.FindUsingGET") FindUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> find


```csharp
Task<dynamic> FindUsingGET(string messageRef, string destinataire, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| destinataire |  ``` Required ```  | destinataire |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
string messageRef = "messageRef";
string destinataire = "destinataire";
string xAuthToken = "X-Auth-Token";

dynamic result = await reportController.FindUsingGET(messageRef, destinataire, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


[Back to List of Controllers](#list_of_controllers)

## <a name="invoice_controller"></a>![Class: ](https://apidocs.io/img/class.png "SMsmodeAPIREST.PCL.Controllers.InvoiceController") InvoiceController

### Get singleton instance

The singleton instance of the ``` InvoiceController ``` class can be accessed from the API Client.

```csharp
InvoiceController invoiceController = client.InvoiceController;
```

### <a name="list_using_get5"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.InvoiceController.ListUsingGET5") ListUsingGET5

> *Tags:*  ``` Skips Authentication ``` 

> View a list of invoices


```csharp
Task<dynamic> ListUsingGET5(string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";
int? limit = 176;

dynamic result = await invoiceController.ListUsingGET5(xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="list_page_using_get5"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.InvoiceController.ListPageUsingGET5") ListPageUsingGET5

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```csharp
Task<dynamic> ListPageUsingGET5(int page, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
int page = 176;
string xAuthToken = "X-Auth-Token";
int? limit = 176;

dynamic result = await invoiceController.ListPageUsingGET5(page, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="get_pdf_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.InvoiceController.GetPdfUsingGET") GetPdfUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Generate an invoice in a pdf file


```csharp
Task<dynamic> GetPdfUsingGET(int id, string xAuthToken, bool base64)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| base64 |  ``` Required ```  | base64 |


#### Example Usage

```csharp
int id = 176;
string xAuthToken = "X-Auth-Token";
bool base64 = true;

dynamic result = await invoiceController.GetPdfUsingGET(id, xAuthToken, base64);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="get_using_get5"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.InvoiceController.GetUsingGET5") GetUsingGET5

> *Tags:*  ``` Skips Authentication ``` 

> Show an invoice


```csharp
Task<Models.InvoiceResourceModel> GetUsingGET5(int id, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
int id = 176;
string xAuthToken = "X-Auth-Token";

Models.InvoiceResourceModel result = await invoiceController.GetUsingGET5(id, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


[Back to List of Controllers](#list_of_controllers)

## <a name="authentication_controller"></a>![Class: ](https://apidocs.io/img/class.png "SMsmodeAPIREST.PCL.Controllers.AuthenticationController") AuthenticationController

### Get singleton instance

The singleton instance of the ``` AuthenticationController ``` class can be accessed from the API Client.

```csharp
AuthenticationController authenticationController = client.AuthenticationController;
```

### <a name="create_get_token_using_post"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.AuthenticationController.CreateGetTokenUsingPOST") CreateGetTokenUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Generate the OAuth Token


```csharp
Task<Models.TokenResourceModel> CreateGetTokenUsingPOST(Models.AuthenticationResourceModel request)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| request |  ``` Required ```  | request |


#### Example Usage

```csharp
var request = new Models.AuthenticationResourceModel();

Models.TokenResourceModel result = await authenticationController.CreateGetTokenUsingPOST(request);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


[Back to List of Controllers](#list_of_controllers)

## <a name="contact_controller"></a>![Class: ](https://apidocs.io/img/class.png "SMsmodeAPIREST.PCL.Controllers.ContactController") ContactController

### Get singleton instance

The singleton instance of the ``` ContactController ``` class can be accessed from the API Client.

```csharp
ContactController contactController = client.ContactController;
```

### <a name="list_using_get1"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ContactController.ListUsingGET1") ListUsingGET1

> *Tags:*  ``` Skips Authentication ``` 

> View a list of contacts


```csharp
Task<dynamic> ListUsingGET1(string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";
int? limit = 176;

dynamic result = await contactController.ListUsingGET1(xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="add_using_post"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ContactController.AddUsingPOST") AddUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Add a contact


```csharp
Task<Models.ContactResourceModel> AddUsingPOST(Models.ContactResourceModel resource, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
var resource = new Models.ContactResourceModel();
string xAuthToken = "X-Auth-Token";

Models.ContactResourceModel result = await contactController.AddUsingPOST(resource, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="delete_book_using_delete"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ContactController.DeleteBookUsingDELETE") DeleteBookUsingDELETE

> *Tags:*  ``` Skips Authentication ``` 

> Remove all contacts and groups of the account


```csharp
Task<dynamic> DeleteBookUsingDELETE(string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";

dynamic result = await contactController.DeleteBookUsingDELETE(xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |


### <a name="get_customer_info_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ContactController.GetCustomerInfoUsingGET") GetCustomerInfoUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Show contact info of customer


```csharp
Task<Models.ContactResourceModel> GetCustomerInfoUsingGET(string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";

Models.ContactResourceModel result = await contactController.GetCustomerInfoUsingGET(xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="update_edit_customer_using_put"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ContactController.UpdateEditCustomerUsingPUT") UpdateEditCustomerUsingPUT

> *Tags:*  ``` Skips Authentication ``` 

> Edit contact info of customer


```csharp
Task<Models.ContactResourceModel> UpdateEditCustomerUsingPUT(string xAuthToken, Models.ContactResourceModel resource)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| resource |  ``` Required ```  | resource |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";
var resource = new Models.ContactResourceModel();

Models.ContactResourceModel result = await contactController.UpdateEditCustomerUsingPUT(xAuthToken, resource);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="create_delete_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ContactController.CreateDeleteListUsingPOST") CreateDeleteListUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Delete a list of contacts


```csharp
Task<dynamic> CreateDeleteListUsingPOST(List<int> idList, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| idList |  ``` Required ```  ``` Collection ```  | idList |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
List<int> idList = new List<int> { 176 };
string xAuthToken = "X-Auth-Token";

dynamic result = await contactController.CreateDeleteListUsingPOST(idList, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="create_export_contacts_using_post"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ContactController.CreateExportContactsUsingPOST") CreateExportContactsUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Export contacts in csv format


```csharp
Task<Models.DeferredResultResponseEntityObjectModel> CreateExportContactsUsingPOST(List<string> fields, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fields |  ``` Required ```  ``` Collection ```  | fields |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
List<string> fields = new List<string> { "fields" };
string xAuthToken = "X-Auth-Token";

Models.DeferredResultResponseEntityObjectModel result = await contactController.CreateExportContactsUsingPOST(fields, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="upload_blocking_using_post"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ContactController.UploadBlockingUsingPOST") UploadBlockingUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Import contacts via xls or csv files


```csharp
Task<Models.DeferredResultResponseEntityObjectModel> UploadBlockingUsingPOST(FileStreamInfo file, string model, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | file |
| model |  ``` Required ```  | model |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
FileStreamInfo file = new FileStreamInfo(new FileStream(@"pathToFile",FileMode.Open));
string model = "model";
string xAuthToken = "X-Auth-Token";

Models.DeferredResultResponseEntityObjectModel result = await contactController.UploadBlockingUsingPOST(file, model, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="list_page_using_get1"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ContactController.ListPageUsingGET1") ListPageUsingGET1

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```csharp
Task<Models.ResourcesContactResourceModel> ListPageUsingGET1(int page, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
int page = 12;
string xAuthToken = "X-Auth-Token";
int? limit = 12;

Models.ResourcesContactResourceModel result = await contactController.ListPageUsingGET1(page, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="search_using_get1"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ContactController.SearchUsingGET1") SearchUsingGET1

> *Tags:*  ``` Skips Authentication ``` 

> search


```csharp
Task<dynamic> SearchUsingGET1(string name, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string name = "name";
string xAuthToken = "X-Auth-Token";
int? limit = 12;

dynamic result = await contactController.SearchUsingGET1(name, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="get_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ContactController.GetUsingGET") GetUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Show a contact


```csharp
Task<Models.ContactResourceModel> GetUsingGET(int id, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
int id = 12;
string xAuthToken = "X-Auth-Token";

Models.ContactResourceModel result = await contactController.GetUsingGET(id, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="update_using_put"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ContactController.UpdateUsingPUT") UpdateUsingPUT

> *Tags:*  ``` Skips Authentication ``` 

> Update a contact


```csharp
Task<dynamic> UpdateUsingPUT(int id, Models.ContactResourceModel resource, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
int id = 12;
var resource = new Models.ContactResourceModel();
string xAuthToken = "X-Auth-Token";

dynamic result = await contactController.UpdateUsingPUT(id, resource, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="delete_using_delete1"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ContactController.DeleteUsingDELETE1") DeleteUsingDELETE1

> *Tags:*  ``` Skips Authentication ``` 

> Delete a contact


```csharp
Task<dynamic> DeleteUsingDELETE1(int id, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
int id = 12;
string xAuthToken = "X-Auth-Token";

dynamic result = await contactController.DeleteUsingDELETE1(id, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |


### <a name="add_group_using_post"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ContactController.AddGroupUsingPOST") AddGroupUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Add a contact in a group


```csharp
Task<dynamic> AddGroupUsingPOST(int id, int groupId, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| groupId |  ``` Required ```  | groupId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
int id = 12;
int groupId = 12;
string xAuthToken = "X-Auth-Token";

dynamic result = await contactController.AddGroupUsingPOST(id, groupId, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="get_groups_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ContactController.GetGroupsUsingGET") GetGroupsUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups for a contact


```csharp
Task<dynamic> GetGroupsUsingGET(
        int id,
        int page,
        string xAuthToken,
        int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
int id = 12;
int page = 12;
string xAuthToken = "X-Auth-Token";
int? limit = 12;

dynamic result = await contactController.GetGroupsUsingGET(id, page, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="delete_group_using_delete"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.ContactController.DeleteGroupUsingDELETE") DeleteGroupUsingDELETE

> *Tags:*  ``` Skips Authentication ``` 

> Remove a contact from a group


```csharp
Task<dynamic> DeleteGroupUsingDELETE(int id, int groupId, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| groupId |  ``` Required ```  | groupId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
int id = 12;
int groupId = 12;
string xAuthToken = "X-Auth-Token";

dynamic result = await contactController.DeleteGroupUsingDELETE(id, groupId, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |


[Back to List of Controllers](#list_of_controllers)

## <a name="customer_controller"></a>![Class: ](https://apidocs.io/img/class.png "SMsmodeAPIREST.PCL.Controllers.CustomerController") CustomerController

### Get singleton instance

The singleton instance of the ``` CustomerController ``` class can be accessed from the API Client.

```csharp
CustomerController customerController = client.CustomerController;
```

### <a name="get_using_get2"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.CustomerController.GetUsingGET2") GetUsingGET2

> *Tags:*  ``` Skips Authentication ``` 

> Show your account


```csharp
Task<Models.CustomerResourceModel> GetUsingGET2(string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";

Models.CustomerResourceModel result = await customerController.GetUsingGET2(xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="get_from_fields_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.CustomerController.GetFromFieldsUsingGET") GetFromFieldsUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Get your personnalized sender IDs


```csharp
Task<dynamic> GetFromFieldsUsingGET(string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";

dynamic result = await customerController.GetFromFieldsUsingGET(xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="update_delete_sender_using_put"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.CustomerController.UpdateDeleteSenderUsingPUT") UpdateDeleteSenderUsingPUT

> *Tags:*  ``` Skips Authentication ``` 

> Remove sender ID


```csharp
Task<dynamic> UpdateDeleteSenderUsingPUT(string xAuthToken, string senderID)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| senderID |  ``` Required ```  | senderID |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";
string senderID = "senderID";

dynamic result = await customerController.UpdateDeleteSenderUsingPUT(xAuthToken, senderID);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="add_sender_using_post"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.CustomerController.AddSenderUsingPOST") AddSenderUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Add personnalized sender ID


```csharp
Task<dynamic> AddSenderUsingPOST(string xAuthToken, string senderID)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| senderID |  ``` Required ```  | senderID |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";
string senderID = "senderID";

dynamic result = await customerController.AddSenderUsingPOST(xAuthToken, senderID);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="list_using_get3"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.CustomerController.ListUsingGET3") ListUsingGET3

> *Tags:*  ``` Skips Authentication ``` 

> View a list of your subaccounts


```csharp
Task<dynamic> ListUsingGET3(string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";
int? limit = 12;

dynamic result = await customerController.ListUsingGET3(xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="list_page_using_get3"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.CustomerController.ListPageUsingGET3") ListPageUsingGET3

> *Tags:*  ``` Skips Authentication ``` 

> View a list of your subaccounts by page


```csharp
Task<dynamic> ListPageUsingGET3(int page, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
int page = 12;
string xAuthToken = "X-Auth-Token";
int? limit = 12;

dynamic result = await customerController.ListPageUsingGET3(page, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


[Back to List of Controllers](#list_of_controllers)

## <a name="group_controller"></a>![Class: ](https://apidocs.io/img/class.png "SMsmodeAPIREST.PCL.Controllers.GroupController") GroupController

### Get singleton instance

The singleton instance of the ``` GroupController ``` class can be accessed from the API Client.

```csharp
GroupController groupController = client.GroupController;
```

### <a name="list_using_get4"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.GroupController.ListUsingGET4") ListUsingGET4

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups


```csharp
Task<dynamic> ListUsingGET4(string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";
int? limit = 12;

dynamic result = await groupController.ListUsingGET4(xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="add_using_post2"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.GroupController.AddUsingPOST2") AddUsingPOST2

> *Tags:*  ``` Skips Authentication ``` 

> Add a group


```csharp
Task<Models.GroupResourceModel> AddUsingPOST2(Models.GroupResourceModel resource, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
var resource = new Models.GroupResourceModel();
string xAuthToken = "X-Auth-Token";

Models.GroupResourceModel result = await groupController.AddUsingPOST2(resource, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="create_delete_list_using_post1"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.GroupController.CreateDeleteListUsingPOST1") CreateDeleteListUsingPOST1

> *Tags:*  ``` Skips Authentication ``` 

> Delete a list of groups


```csharp
Task<dynamic> CreateDeleteListUsingPOST1(List<int> idList, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| idList |  ``` Required ```  ``` Collection ```  | idList |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
List<int> idList = new List<int> { 12 };
string xAuthToken = "X-Auth-Token";

dynamic result = await groupController.CreateDeleteListUsingPOST1(idList, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="list_page_using_get4"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.GroupController.ListPageUsingGET4") ListPageUsingGET4

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```csharp
Task<dynamic> ListPageUsingGET4(int page, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
int page = 12;
string xAuthToken = "X-Auth-Token";
int? limit = 12;

dynamic result = await groupController.ListPageUsingGET4(page, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="search_using_get2"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.GroupController.SearchUsingGET2") SearchUsingGET2

> *Tags:*  ``` Skips Authentication ``` 

> search


```csharp
Task<dynamic> SearchUsingGET2(string name, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string name = "name";
string xAuthToken = "X-Auth-Token";
int? limit = 12;

dynamic result = await groupController.SearchUsingGET2(name, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="get_using_get4"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.GroupController.GetUsingGET4") GetUsingGET4

> *Tags:*  ``` Skips Authentication ``` 

> Show a group


```csharp
Task<Models.GroupResourceModel> GetUsingGET4(int id, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
int id = 12;
string xAuthToken = "X-Auth-Token";

Models.GroupResourceModel result = await groupController.GetUsingGET4(id, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="update_using_put2"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.GroupController.UpdateUsingPUT2") UpdateUsingPUT2

> *Tags:*  ``` Skips Authentication ``` 

> Update a group


```csharp
Task<dynamic> UpdateUsingPUT2(int id, Models.GroupResourceModel resource, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
int id = 12;
var resource = new Models.GroupResourceModel();
string xAuthToken = "X-Auth-Token";

dynamic result = await groupController.UpdateUsingPUT2(id, resource, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="delete_using_delete3"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.GroupController.DeleteUsingDELETE3") DeleteUsingDELETE3

> *Tags:*  ``` Skips Authentication ``` 

> Delete a group


```csharp
Task<dynamic> DeleteUsingDELETE3(int id, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
int id = 12;
string xAuthToken = "X-Auth-Token";

dynamic result = await groupController.DeleteUsingDELETE3(id, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |


### <a name="get_contacts_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.GroupController.GetContactsUsingGET") GetContactsUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Show a list of contacts for a group


```csharp
Task<Models.GroupResourceModel> GetContactsUsingGET(
        int id,
        int page,
        string xAuthToken,
        int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
int id = 12;
int page = 12;
string xAuthToken = "X-Auth-Token";
int? limit = 12;

Models.GroupResourceModel result = await groupController.GetContactsUsingGET(id, page, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


[Back to List of Controllers](#list_of_controllers)

## <a name="campaign_controller"></a>![Class: ](https://apidocs.io/img/class.png "SMsmodeAPIREST.PCL.Controllers.CampaignController") CampaignController

### Get singleton instance

The singleton instance of the ``` CampaignController ``` class can be accessed from the API Client.

```csharp
CampaignController campaignController = client.CampaignController;
```

### <a name="list_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.CampaignController.ListUsingGET") ListUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> list


```csharp
Task<dynamic> ListUsingGET(string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";
int? limit = 12;

dynamic result = await campaignController.ListUsingGET(xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="create_send_to_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.CampaignController.CreateSendToListUsingPOST") CreateSendToListUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> sendToList


```csharp
Task<dynamic> CreateSendToListUsingPOST(Models.CampaignInputResourceModel resource, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
var resource = new Models.CampaignInputResourceModel();
string xAuthToken = "X-Auth-Token";

dynamic result = await campaignController.CreateSendToListUsingPOST(resource, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="list_page_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.CampaignController.ListPageUsingGET") ListPageUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```csharp
Task<dynamic> ListPageUsingGET(int page, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
int page = 12;
string xAuthToken = "X-Auth-Token";
int? limit = 12;

dynamic result = await campaignController.ListPageUsingGET(page, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="search_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.CampaignController.SearchUsingGET") SearchUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> search


```csharp
Task<dynamic> SearchUsingGET(string name, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string name = "name";
string xAuthToken = "X-Auth-Token";
int? limit = 12;

dynamic result = await campaignController.SearchUsingGET(name, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="delete_using_delete"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.CampaignController.DeleteUsingDELETE") DeleteUsingDELETE

> *Tags:*  ``` Skips Authentication ``` 

> delete


```csharp
Task<dynamic> DeleteUsingDELETE(string messsageId, string xAuthToken, string id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsageId |  ``` Required ```  | messsageId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| id |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string messsageId = "messsageId";
string xAuthToken = "X-Auth-Token";
string id = "id";

dynamic result = await campaignController.DeleteUsingDELETE(messsageId, xAuthToken, id);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |


[Back to List of Controllers](#list_of_controllers)

## <a name="transfer_controller"></a>![Class: ](https://apidocs.io/img/class.png "SMsmodeAPIREST.PCL.Controllers.TransferController") TransferController

### Get singleton instance

The singleton instance of the ``` TransferController ``` class can be accessed from the API Client.

```csharp
TransferController transferController = client.TransferController;
```

### <a name="list_using_get9"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.TransferController.ListUsingGET9") ListUsingGET9

> *Tags:*  ``` Skips Authentication ``` 

> View a list of transferts


```csharp
Task<dynamic> ListUsingGET9(string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";
int? limit = 12;

dynamic result = await transferController.ListUsingGET9(xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="list_page_using_get9"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.TransferController.ListPageUsingGET9") ListPageUsingGET9

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```csharp
Task<dynamic> ListPageUsingGET9(int page, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
int page = 12;
string xAuthToken = "X-Auth-Token";
int? limit = 12;

dynamic result = await transferController.ListPageUsingGET9(page, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="get_using_get9"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.TransferController.GetUsingGET9") GetUsingGET9

> *Tags:*  ``` Skips Authentication ``` 

> Show a transfet


```csharp
Task<Models.TransferResourceModel> GetUsingGET9(int id, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
int id = 12;
string xAuthToken = "X-Auth-Token";

Models.TransferResourceModel result = await transferController.GetUsingGET9(id, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


[Back to List of Controllers](#list_of_controllers)

## <a name="email_api_configuration_controller"></a>![Class: ](https://apidocs.io/img/class.png "SMsmodeAPIREST.PCL.Controllers.EmailApiConfigurationController") EmailApiConfigurationController

### Get singleton instance

The singleton instance of the ``` EmailApiConfigurationController ``` class can be accessed from the API Client.

```csharp
EmailApiConfigurationController emailApiConfigurationController = client.EmailApiConfigurationController;
```

### <a name="get_using_get3"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.EmailApiConfigurationController.GetUsingGET3") GetUsingGET3

> *Tags:*  ``` Skips Authentication ``` 

> Show your configuration


```csharp
Task<Models.EmailAPIConfigurationResourceModel> GetUsingGET3(string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";

Models.EmailAPIConfigurationResourceModel result = await emailApiConfigurationController.GetUsingGET3(xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="update_using_put1"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.EmailApiConfigurationController.UpdateUsingPUT1") UpdateUsingPUT1

> *Tags:*  ``` Skips Authentication ``` 

> Update your configuration


```csharp
Task<dynamic> UpdateUsingPUT1(Models.EmailAPIConfigurationResourceModel resource, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
var resource = new Models.EmailAPIConfigurationResourceModel();
string xAuthToken = "X-Auth-Token";

dynamic result = await emailApiConfigurationController.UpdateUsingPUT1(resource, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="add_using_post1"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.EmailApiConfigurationController.AddUsingPOST1") AddUsingPOST1

> *Tags:*  ``` Skips Authentication ``` 

> Create your configuration


```csharp
Task<Models.EmailAPIConfigurationResourceModel> AddUsingPOST1(Models.EmailAPIConfigurationResourceModel resource, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
var resource = new Models.EmailAPIConfigurationResourceModel();
string xAuthToken = "X-Auth-Token";

Models.EmailAPIConfigurationResourceModel result = await emailApiConfigurationController.AddUsingPOST1(resource, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="delete_using_delete2"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.EmailApiConfigurationController.DeleteUsingDELETE2") DeleteUsingDELETE2

> *Tags:*  ``` Skips Authentication ``` 

> Delete your configuration


```csharp
Task<dynamic> DeleteUsingDELETE2(string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";

dynamic result = await emailApiConfigurationController.DeleteUsingDELETE2(xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |


[Back to List of Controllers](#list_of_controllers)

## <a name="message_controller"></a>![Class: ](https://apidocs.io/img/class.png "SMsmodeAPIREST.PCL.Controllers.MessageController") MessageController

### Get singleton instance

The singleton instance of the ``` MessageController ``` class can be accessed from the API Client.

```csharp
MessageController messageController = client.MessageController;
```

### <a name="list_using_get6"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageController.ListUsingGET6") ListUsingGET6

> *Tags:*  ``` Skips Authentication ``` 

> list


```csharp
Task<dynamic> ListUsingGET6(string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";
int? limit = 12;

dynamic result = await messageController.ListUsingGET6(xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="list_page_using_get6"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageController.ListPageUsingGET6") ListPageUsingGET6

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```csharp
Task<Models.PagedResourcesMessageResourceModel> ListPageUsingGET6(int page, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
int page = 12;
string xAuthToken = "X-Auth-Token";
int? limit = 12;

Models.PagedResourcesMessageResourceModel result = await messageController.ListPageUsingGET6(page, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="list_responses_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageController.ListResponsesUsingGET") ListResponsesUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> listResponses


```csharp
Task<Models.ResourcesMessageResourceModel> ListResponsesUsingGET(string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";
int? limit = 12;

Models.ResourcesMessageResourceModel result = await messageController.ListResponsesUsingGET(xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="list_responses_page_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageController.ListResponsesPageUsingGET") ListResponsesPageUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> listResponsesPage


```csharp
Task<Models.PagedResourcesMessageResourceModel> ListResponsesPageUsingGET(int page, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
int page = 12;
string xAuthToken = "X-Auth-Token";
int? limit = 12;

Models.PagedResourcesMessageResourceModel result = await messageController.ListResponsesPageUsingGET(page, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="list_scheduled_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageController.ListScheduledUsingGET") ListScheduledUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> listScheduled


```csharp
Task<Models.ResourcesMessageResourceModel> ListScheduledUsingGET(string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";
int? limit = 12;

Models.ResourcesMessageResourceModel result = await messageController.ListScheduledUsingGET(xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="list_scheduled_page_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageController.ListScheduledPageUsingGET") ListScheduledPageUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> listScheduledPage


```csharp
Task<Models.PagedResourcesMessageResourceModel> ListScheduledPageUsingGET(int page, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
int page = 12;
string xAuthToken = "X-Auth-Token";
int? limit = 12;

Models.PagedResourcesMessageResourceModel result = await messageController.ListScheduledPageUsingGET(page, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="search_using_get3"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageController.SearchUsingGET3") SearchUsingGET3

> *Tags:*  ``` Skips Authentication ``` 

> search


```csharp
Task<dynamic> SearchUsingGET3(string id, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string id = "id";
string xAuthToken = "X-Auth-Token";
int? limit = 12;

dynamic result = await messageController.SearchUsingGET3(id, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="create_send_to_list_using_post1"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageController.CreateSendToListUsingPOST1") CreateSendToListUsingPOST1

> *Tags:*  ``` Skips Authentication ``` 

> sendToList


```csharp
Task<dynamic> CreateSendToListUsingPOST1(Models.MessageInputMixedResourceModel resource, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
var resource = new Models.MessageInputMixedResourceModel();
string xAuthToken = "X-Auth-Token";

dynamic result = await messageController.CreateSendToListUsingPOST1(resource, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="create_send_to_contact_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageController.CreateSendToContactListUsingPOST") CreateSendToContactListUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> sendToContactList


```csharp
Task CreateSendToContactListUsingPOST(Models.MessageInputContactResourceModel resource, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
var resource = new Models.MessageInputContactResourceModel();
string xAuthToken = "X-Auth-Token";

await messageController.CreateSendToContactListUsingPOST(resource, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="create_send_to_group_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageController.CreateSendToGroupListUsingPOST") CreateSendToGroupListUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> sendToGroupList


```csharp
Task CreateSendToGroupListUsingPOST(Models.MessageInputGroupResourceModel resource, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
var resource = new Models.MessageInputGroupResourceModel();
string xAuthToken = "X-Auth-Token";

await messageController.CreateSendToGroupListUsingPOST(resource, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="create_send_to_number_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageController.CreateSendToNumberListUsingPOST") CreateSendToNumberListUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> sendToNumberList


```csharp
Task<dynamic> CreateSendToNumberListUsingPOST(Models.MessageInputResourceModel resource, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
var resource = new Models.MessageInputResourceModel();
string xAuthToken = "X-Auth-Token";

dynamic result = await messageController.CreateSendToNumberListUsingPOST(resource, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="delete_using_delete4"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageController.DeleteUsingDELETE4") DeleteUsingDELETE4

> *Tags:*  ``` Skips Authentication ``` 

> delete


```csharp
Task DeleteUsingDELETE4(string messsageId, string xAuthToken, string id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsageId |  ``` Required ```  | messsageId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| id |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string messsageId = "messsageId";
string xAuthToken = "X-Auth-Token";
string id = "id";

await messageController.DeleteUsingDELETE4(messsageId, xAuthToken, id);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |


[Back to List of Controllers](#list_of_controllers)

## <a name="register_controler_controller"></a>![Class: ](https://apidocs.io/img/class.png "SMsmodeAPIREST.PCL.Controllers.RegisterControlerController") RegisterControlerController

### Get singleton instance

The singleton instance of the ``` RegisterControlerController ``` class can be accessed from the API Client.

```csharp
RegisterControlerController registerControler = client.RegisterControler;
```

### <a name="create_register_using_post"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.RegisterControlerController.CreateRegisterUsingPOST") CreateRegisterUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> register


```csharp
Task<dynamic> CreateRegisterUsingPOST(Models.RegisterResourceModel resource)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |


#### Example Usage

```csharp
var resource = new Models.RegisterResourceModel();

dynamic result = await registerControler.CreateRegisterUsingPOST(resource);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="create_refresh_using_post"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.RegisterControlerController.CreateRefreshUsingPOST") CreateRefreshUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> refresh


```csharp
Task<dynamic> CreateRefreshUsingPOST(Models.SimpleEmailResourceModel resource)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |


#### Example Usage

```csharp
var resource = new Models.SimpleEmailResourceModel();

dynamic result = await registerControler.CreateRefreshUsingPOST(resource);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="get_activate_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.RegisterControlerController.GetActivateUsingGET") GetActivateUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> activate


```csharp
Task<dynamic> GetActivateUsingGET(string token, int id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| token |  ``` Required ```  | token |
| id |  ``` Required ```  | id |


#### Example Usage

```csharp
string token = "token";
int id = 12;

dynamic result = await registerControler.GetActivateUsingGET(token, id);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


[Back to List of Controllers](#list_of_controllers)

## <a name="credit_consumption_controller"></a>![Class: ](https://apidocs.io/img/class.png "SMsmodeAPIREST.PCL.Controllers.CreditConsumptionController") CreditConsumptionController

### Get singleton instance

The singleton instance of the ``` CreditConsumptionController ``` class can be accessed from the API Client.

```csharp
CreditConsumptionController creditConsumptionController = client.CreditConsumptionController;
```

### <a name="list_using_get2"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.CreditConsumptionController.ListUsingGET2") ListUsingGET2

> *Tags:*  ``` Skips Authentication ``` 

> Get the consumption of the last months


```csharp
Task<dynamic> ListUsingGET2(string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";
int? limit = 12;

dynamic result = await creditConsumptionController.ListUsingGET2(xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="list_page_using_get2"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.CreditConsumptionController.ListPageUsingGET2") ListPageUsingGET2

> *Tags:*  ``` Skips Authentication ``` 

> Get pageable consumption of the last months


```csharp
Task<dynamic> ListPageUsingGET2(int page, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
int page = 12;
string xAuthToken = "X-Auth-Token";
int? limit = 12;

dynamic result = await creditConsumptionController.ListPageUsingGET2(page, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="get_using_get1"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.CreditConsumptionController.GetUsingGET1") GetUsingGET1

> *Tags:*  ``` Skips Authentication ``` 

> Get specific consumption by id 


```csharp
Task<dynamic> GetUsingGET1(int id, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
int id = 12;
string xAuthToken = "X-Auth-Token";

dynamic result = await creditConsumptionController.GetUsingGET1(id, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


[Back to List of Controllers](#list_of_controllers)

## <a name="pricing_controller"></a>![Class: ](https://apidocs.io/img/class.png "SMsmodeAPIREST.PCL.Controllers.PricingController") PricingController

### Get singleton instance

The singleton instance of the ``` PricingController ``` class can be accessed from the API Client.

```csharp
PricingController pricingController = client.PricingController;
```

### <a name="get_using_get7"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.PricingController.GetUsingGET7") GetUsingGET7

> *Tags:*  ``` Skips Authentication ``` 

> get


```csharp
Task<Models.PricingResourceModel> GetUsingGET7(string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";

Models.PricingResourceModel result = await pricingController.GetUsingGET7(xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


[Back to List of Controllers](#list_of_controllers)

## <a name="message_model_controller"></a>![Class: ](https://apidocs.io/img/class.png "SMsmodeAPIREST.PCL.Controllers.MessageModelController") MessageModelController

### Get singleton instance

The singleton instance of the ``` MessageModelController ``` class can be accessed from the API Client.

```csharp
MessageModelController messageModelController = client.MessageModelController;
```

### <a name="list_using_get7"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageModelController.ListUsingGET7") ListUsingGET7

> *Tags:*  ``` Skips Authentication ``` 

> list


```csharp
Task<Models.ResourcesMessageModelResourceModel> ListUsingGET7(string xAuthToken, int? size = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| size |  ``` Optional ```  | size |


#### Example Usage

```csharp
string xAuthToken = "X-Auth-Token";
int? size = 12;

Models.ResourcesMessageModelResourceModel result = await messageModelController.ListUsingGET7(xAuthToken, size);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="add_using_post3"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageModelController.AddUsingPOST3") AddUsingPOST3

> *Tags:*  ``` Skips Authentication ``` 

> add


```csharp
Task<Models.MessageModelResourceModel> AddUsingPOST3(Models.MessageModelInputResourceModel resource, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
var resource = new Models.MessageModelInputResourceModel();
string xAuthToken = "X-Auth-Token";

Models.MessageModelResourceModel result = await messageModelController.AddUsingPOST3(resource, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="create_delete_multiple_using_post"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageModelController.CreateDeleteMultipleUsingPOST") CreateDeleteMultipleUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> deleteMultiple


```csharp
Task<dynamic> CreateDeleteMultipleUsingPOST(List<string> ids, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ids |  ``` Required ```  ``` Collection ```  | ids |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
List<string> ids = new List<string> { "ids" };
string xAuthToken = "X-Auth-Token";

dynamic result = await messageModelController.CreateDeleteMultipleUsingPOST(ids, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="list_page_using_get7"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageModelController.ListPageUsingGET7") ListPageUsingGET7

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```csharp
Task<Models.PagedResourcesMessageModelResourceModel> ListPageUsingGET7(int page, string xAuthToken, int? limit = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```csharp
int page = 12;
string xAuthToken = "X-Auth-Token";
int? limit = 12;

Models.PagedResourcesMessageModelResourceModel result = await messageModelController.ListPageUsingGET7(page, xAuthToken, limit);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="get_using_get6"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageModelController.GetUsingGET6") GetUsingGET6

> *Tags:*  ``` Skips Authentication ``` 

> get


```csharp
Task<Models.MessageModelResourceModel> GetUsingGET6(string id, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
string id = "id";
string xAuthToken = "X-Auth-Token";

Models.MessageModelResourceModel result = await messageModelController.GetUsingGET6(id, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="update_using_put3"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageModelController.UpdateUsingPUT3") UpdateUsingPUT3

> *Tags:*  ``` Skips Authentication ``` 

> update


```csharp
Task UpdateUsingPUT3(string id, Models.MessageModelInputResourceModel resource, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
string id = "id";
var resource = new Models.MessageModelInputResourceModel();
string xAuthToken = "X-Auth-Token";

await messageModelController.UpdateUsingPUT3(id, resource, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="delete_using_delete5"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.MessageModelController.DeleteUsingDELETE5") DeleteUsingDELETE5

> *Tags:*  ``` Skips Authentication ``` 

> delete


```csharp
Task DeleteUsingDELETE5(string id, string xAuthToken)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```csharp
string id = "id";
string xAuthToken = "X-Auth-Token";

await messageModelController.DeleteUsingDELETE5(id, xAuthToken);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |


[Back to List of Controllers](#list_of_controllers)

## <a name="societe_info_controller"></a>![Class: ](https://apidocs.io/img/class.png "SMsmodeAPIREST.PCL.Controllers.SocieteInfoController") SocieteInfoController

### Get singleton instance

The singleton instance of the ``` SocieteInfoController ``` class can be accessed from the API Client.

```csharp
SocieteInfoController societeInfoController = client.SocieteInfoController;
```

### <a name="create_research_company_using_post"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.SocieteInfoController.CreateResearchCompanyUsingPOST") CreateResearchCompanyUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> researchCompany


```csharp
Task<dynamic> CreateResearchCompanyUsingPOST(Models.SocieteInfoResearchResourceModel research)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| research |  ``` Required ```  | research |


#### Example Usage

```csharp
var research = new Models.SocieteInfoResearchResourceModel();

dynamic result = await societeInfoController.CreateResearchCompanyUsingPOST(research);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


### <a name="get_details_using_get"></a>![Method: ](https://apidocs.io/img/method.png "SMsmodeAPIREST.PCL.Controllers.SocieteInfoController.GetDetailsUsingGET") GetDetailsUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> getDetails


```csharp
Task<dynamic> GetDetailsUsingGET(string id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |


#### Example Usage

```csharp
string id = "id";

dynamic result = await societeInfoController.GetDetailsUsingGET(id);

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |


[Back to List of Controllers](#list_of_controllers)



