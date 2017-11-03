# Getting started

sMsMode API-REST Documentation

## How to Build


* In order to successfully build and run your SDK files, you are required to have the following setup in your system:
    * **Go**  (Visit [https://golang.org/doc/install](https://golang.org/doc/install) for more details on how to install Go)
    * **Java VM** Version 8 or later
    * **Eclipse 4.6 (Neon)** or later ([http://www.eclipse.org/neon/](http://www.eclipse.org/neon/))
    * **GoClipse** setup within above installed Eclipse (Follow the instructions at [this link](https://github.com/GoClipse/goclipse/blob/latest/documentation/Installation.md#instructions) to setup GoClipse)
* Ensure that ```GOPATH``` environment variable is set in the system variables. If not, set it to your workspace directory where you will be adding your Go projects.
* The generated code uses unirest-go http library. Therefore, you will need internet access to resolve this dependency. If Go is properly installed and configured, run the following command to pull the dependency:

```Go
go get github.com/apimatic/unirest-go
```

This will install unirest-go in the ```GOPATH``` you specified in the system variables.

Now follow the steps mentioned below to build your SDK:

1. Open eclipse in the Go language perspective and click on the ```Import``` option in ```File``` menu.

![Importing SDK into Eclipse - Step 1](https://apidocs.io/illustration/go?step=import0)

2. Select ```General -> Existing Projects into Workspace``` option from the tree list.

![Importing SDK into Eclipse - Step 2](https://apidocs.io/illustration/go?step=import1)

3. In ```Select root directory```, provide path to the unzipped archive for the generated code. Once the path is set and the Project becomes visible under ```Projects``` click ```Finish```

![Importing SDK into Eclipse - Step 3](https://apidocs.io/illustration/go?step=import2&workspaceFolder=sMsmode%20API-REST-GoLang&projectName=smsmodeapirest_lib)

4. The Go library will be imported and its files will be visible in the Project Explorer

![Importing SDK into Eclipse - Step 4](https://apidocs.io/illustration/go?step=import3&projectName=smsmodeapirest_lib)

## How to Use

The following section explains how to use the SmsmodeapirestLib library in a new project.

### 1. Add a new Test Project

Create a new project in Eclipse by ```File``` -> ```New``` -> ```Go Project```

![Add a new project in Eclipse](https://apidocs.io/illustration/go?step=createNewProject0)

Name the Project as ```Test``` and click ```Finish```

![Create a new Maven Project - Step 1](https://apidocs.io/illustration/go?step=createNewProject1)

Create a new directory in the ```src``` directory of this project

![Create a new Maven Project - Step 2](https://apidocs.io/illustration/go?step=createNewProject2&projectName=smsmodeapirest_lib)

Name it ```test.com```

![Create a new Maven Project - Step 3](https://apidocs.io/illustration/go?step=createNewProject3&projectName=smsmodeapirest_lib)

Now create a new file inside ```src/test.com```

![Create a new Maven Project - Step 4](https://apidocs.io/illustration/go?step=createNewProject4&projectName=smsmodeapirest_lib)

Name it ```testsdk.go```

![Create a new Maven Project - Step 5](https://apidocs.io/illustration/go?step=createNewProject5&projectName=smsmodeapirest_lib)

In this Go file, you can start adding code to initialize the client library. Sample code to initialize the client library and using its methods is given in the subsequent sections.

### 2. Configure the Test Project

You need to import your generated library in this project in order to make use of its functions. In order to import the library, you can add its path in the ```GOPATH``` for this project. Follow the below steps:

Right click on the project name and click on ```Properties```

![Adding dependency to the client library - Step 1](https://apidocs.io/illustration/go?step=testProject0&projectName=smsmodeapirest_lib)

Choose ```Go Compiler``` from the side menu. Check ```Use project specific settings``` and uncheck ```Use same value as the GOPATH environment variable.```. By default, the GOPATH value from the environment variables will be visible in ```Eclipse GOPATH```. Do not remove this as this points to the unirest dependency.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/go?step=testProject1)

Append the library path to this GOPATH

![Adding dependency to the client library - Step 3](https://apidocs.io/illustration/go?step=testProject2&workspaceFolder=sMsmode%20API-REST-GoLang)

Once the path is appended, click on ```OK```

### 3. Build the Test Project

Right click on the project name and click on ```Build Project```

![Build Project](https://apidocs.io/illustration/go?step=buildProject&projectName=smsmodeapirest_lib)

### 4. Run the Test Project

If the build is successful, right click on your Go file and click on ```Run As``` -> ```Go Application```

![Run Project](https://apidocs.io/illustration/go?step=runProject&projectName=smsmodeapirest_lib)

# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [report-controller_pkg](#report_controller_pkg)
* [invoice-controller_pkg](#invoice_controller_pkg)
* [authentication-controller_pkg](#authentication_controller_pkg)
* [contact-controller_pkg](#contact_controller_pkg)
* [customer-controller_pkg](#customer_controller_pkg)
* [group-controller_pkg](#group_controller_pkg)
* [campaign-controller_pkg](#campaign_controller_pkg)
* [transfer-controller_pkg](#transfer_controller_pkg)
* [email-api-configuration-controller_pkg](#email_api_configuration_controller_pkg)
* [message-controller_pkg](#message_controller_pkg)
* [register-controler_pkg](#register_controler_pkg)
* [credit-consumption-controller_pkg](#credit_consumption_controller_pkg)
* [pricing-controller_pkg](#pricing_controller_pkg)
* [message-model-controller_pkg](#message_model_controller_pkg)
* [societe-info-controller_pkg](#societe_info_controller_pkg)

## <a name="report_controller_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".report-controller_pkg") report-controller_pkg

### Get instance

Factory for the ``` REPORT-CONTROLLER ``` interface can be accessed from the package report-controller_pkg.

```go
reportController := report-controller_pkg.NewREPORT-CONTROLLER()
```

### <a name="list_using_get8"></a>![Method: ](https://apidocs.io/img/method.png ".report-controller_pkg.ListUsingGET8") ListUsingGET8

> *Tags:*  ``` Skips Authentication ``` 

> list


```go
func (me *REPORTCONTROLLER_IMPL) ListUsingGET8(
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("154", 10, 8)

var result interface{}
result,_ = reportController.ListUsingGET8(xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get8"></a>![Method: ](https://apidocs.io/img/method.png ".report-controller_pkg.ListPageUsingGET8") ListPageUsingGET8

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```go
func (me *REPORTCONTROLLER_IMPL) ListPageUsingGET8(
            page int64,
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
page,_ := strconv.ParseInt("154", 10, 8)
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("154", 10, 8)

var result interface{}
result,_ = reportController.ListPageUsingGET8(page, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get8"></a>![Method: ](https://apidocs.io/img/method.png ".report-controller_pkg.GetUsingGET8") GetUsingGET8

> *Tags:*  ``` Skips Authentication ``` 

> get


```go
func (me *REPORTCONTROLLER_IMPL) GetUsingGET8(
            messageRef string,
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
messageRef := "messageRef"
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("154", 10, 8)

var result interface{}
result,_ = reportController.GetUsingGET8(messageRef, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_page_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".report-controller_pkg.GetPageUsingGET") GetPageUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> getPage


```go
func (me *REPORTCONTROLLER_IMPL) GetPageUsingGET(
            messageRef string,
            page int64,
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
messageRef := "messageRef"
page,_ := strconv.ParseInt("154", 10, 8)
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("154", 10, 8)

var result interface{}
result,_ = reportController.GetPageUsingGET(messageRef, page, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="find_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".report-controller_pkg.FindUsingGET") FindUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> find


```go
func (me *REPORTCONTROLLER_IMPL) FindUsingGET(
            messageRef string,
            destinataire string,
            xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| destinataire |  ``` Required ```  | destinataire |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
messageRef := "messageRef"
destinataire := "destinataire"
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = reportController.FindUsingGET(messageRef, destinataire, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="invoice_controller_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".invoice-controller_pkg") invoice-controller_pkg

### Get instance

Factory for the ``` INVOICE-CONTROLLER ``` interface can be accessed from the package invoice-controller_pkg.

```go
invoiceController := invoice-controller_pkg.NewINVOICE-CONTROLLER()
```

### <a name="list_using_get5"></a>![Method: ](https://apidocs.io/img/method.png ".invoice-controller_pkg.ListUsingGET5") ListUsingGET5

> *Tags:*  ``` Skips Authentication ``` 

> View a list of invoices


```go
func (me *INVOICECONTROLLER_IMPL) ListUsingGET5(
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("154", 10, 8)

var result interface{}
result,_ = invoiceController.ListUsingGET5(xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get5"></a>![Method: ](https://apidocs.io/img/method.png ".invoice-controller_pkg.ListPageUsingGET5") ListPageUsingGET5

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```go
func (me *INVOICECONTROLLER_IMPL) ListPageUsingGET5(
            page int64,
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
page,_ := strconv.ParseInt("154", 10, 8)
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("154", 10, 8)

var result interface{}
result,_ = invoiceController.ListPageUsingGET5(page, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_pdf_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".invoice-controller_pkg.GetPdfUsingGET") GetPdfUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Generate an invoice in a pdf file


```go
func (me *INVOICECONTROLLER_IMPL) GetPdfUsingGET(
            id int64,
            xAuthToken string,
            base64 bool)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| base64 |  ``` Required ```  | base64 |


#### Example Usage

```go
id,_ := strconv.ParseInt("154", 10, 8)
xAuthToken := "X-Auth-Token"
base64 := true

var result interface{}
result,_ = invoiceController.GetPdfUsingGET(id, xAuthToken, base64)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get5"></a>![Method: ](https://apidocs.io/img/method.png ".invoice-controller_pkg.GetUsingGET5") GetUsingGET5

> *Tags:*  ``` Skips Authentication ``` 

> Show an invoice


```go
func (me *INVOICECONTROLLER_IMPL) GetUsingGET5(
            id int64,
            xAuthToken string)(*models_pkg.InvoiceResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
id,_ := strconv.ParseInt("154", 10, 8)
xAuthToken := "X-Auth-Token"

var result *models_pkg.InvoiceResourceModel
result,_ = invoiceController.GetUsingGET5(id, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="authentication_controller_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".authentication-controller_pkg") authentication-controller_pkg

### Get instance

Factory for the ``` AUTHENTICATION-CONTROLLER ``` interface can be accessed from the package authentication-controller_pkg.

```go
authenticationController := authentication-controller_pkg.NewAUTHENTICATION-CONTROLLER()
```

### <a name="create_get_token_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".authentication-controller_pkg.CreateGetTokenUsingPOST") CreateGetTokenUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Generate the OAuth Token


```go
func (me *AUTHENTICATIONCONTROLLER_IMPL) CreateGetTokenUsingPOST(request *models_pkg.AuthenticationResourceModel)(*models_pkg.TokenResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| request |  ``` Required ```  | request |


#### Example Usage

```go
var request *models_pkg.AuthenticationResourceModel

var result *models_pkg.TokenResourceModel
result,_ = authenticationController.CreateGetTokenUsingPOST(request)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="contact_controller_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".contact-controller_pkg") contact-controller_pkg

### Get instance

Factory for the ``` CONTACT-CONTROLLER ``` interface can be accessed from the package contact-controller_pkg.

```go
contactController := contact-controller_pkg.NewCONTACT-CONTROLLER()
```

### <a name="list_using_get1"></a>![Method: ](https://apidocs.io/img/method.png ".contact-controller_pkg.ListUsingGET1") ListUsingGET1

> *Tags:*  ``` Skips Authentication ``` 

> View a list of contacts


```go
func (me *CONTACTCONTROLLER_IMPL) ListUsingGET1(
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("154", 10, 8)

var result interface{}
result,_ = contactController.ListUsingGET1(xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="add_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".contact-controller_pkg.AddUsingPOST") AddUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Add a contact


```go
func (me *CONTACTCONTROLLER_IMPL) AddUsingPOST(
            resource *models_pkg.ContactResourceModel,
            xAuthToken string)(*models_pkg.ContactResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
var resource *models_pkg.ContactResourceModel
xAuthToken := "X-Auth-Token"

var result *models_pkg.ContactResourceModel
result,_ = contactController.AddUsingPOST(resource, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_book_using_delete"></a>![Method: ](https://apidocs.io/img/method.png ".contact-controller_pkg.DeleteBookUsingDELETE") DeleteBookUsingDELETE

> *Tags:*  ``` Skips Authentication ``` 

> Remove all contacts and groups of the account


```go
func (me *CONTACTCONTROLLER_IMPL) DeleteBookUsingDELETE(xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = contactController.DeleteBookUsingDELETE(xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



### <a name="get_customer_info_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".contact-controller_pkg.GetCustomerInfoUsingGET") GetCustomerInfoUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Show contact info of customer


```go
func (me *CONTACTCONTROLLER_IMPL) GetCustomerInfoUsingGET(xAuthToken string)(*models_pkg.ContactResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"

var result *models_pkg.ContactResourceModel
result,_ = contactController.GetCustomerInfoUsingGET(xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_edit_customer_using_put"></a>![Method: ](https://apidocs.io/img/method.png ".contact-controller_pkg.UpdateEditCustomerUsingPUT") UpdateEditCustomerUsingPUT

> *Tags:*  ``` Skips Authentication ``` 

> Edit contact info of customer


```go
func (me *CONTACTCONTROLLER_IMPL) UpdateEditCustomerUsingPUT(
            xAuthToken string,
            resource *models_pkg.ContactResourceModel)(*models_pkg.ContactResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| resource |  ``` Required ```  | resource |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"
var resource *models_pkg.ContactResourceModel

var result *models_pkg.ContactResourceModel
result,_ = contactController.UpdateEditCustomerUsingPUT(xAuthToken, resource)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_delete_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".contact-controller_pkg.CreateDeleteListUsingPOST") CreateDeleteListUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Delete a list of contacts


```go
func (me *CONTACTCONTROLLER_IMPL) CreateDeleteListUsingPOST(
            idList []int64,
            xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| idList |  ``` Required ```  ``` Collection ```  | idList |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
idList := []int64{154}
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = contactController.CreateDeleteListUsingPOST(idList, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_export_contacts_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".contact-controller_pkg.CreateExportContactsUsingPOST") CreateExportContactsUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Export contacts in csv format


```go
func (me *CONTACTCONTROLLER_IMPL) CreateExportContactsUsingPOST(
            fields []string,
            xAuthToken string)(*models_pkg.DeferredResultResponseEntityObjectModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fields |  ``` Required ```  ``` Collection ```  | fields |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
fields := []string{"fields"}
xAuthToken := "X-Auth-Token"

var result *models_pkg.DeferredResultResponseEntityObjectModel
result,_ = contactController.CreateExportContactsUsingPOST(fields, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="upload_blocking_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".contact-controller_pkg.UploadBlockingUsingPOST") UploadBlockingUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Import contacts via xls or csv files


```go
func (me *CONTACTCONTROLLER_IMPL) UploadBlockingUsingPOST(
            file []byte,
            model string,
            xAuthToken string)(*models_pkg.DeferredResultResponseEntityObjectModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | file |
| model |  ``` Required ```  | model |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
file :=  []byte("")
model := "model"
xAuthToken := "X-Auth-Token"

var result *models_pkg.DeferredResultResponseEntityObjectModel
result,_ = contactController.UploadBlockingUsingPOST(file, model, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get1"></a>![Method: ](https://apidocs.io/img/method.png ".contact-controller_pkg.ListPageUsingGET1") ListPageUsingGET1

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```go
func (me *CONTACTCONTROLLER_IMPL) ListPageUsingGET1(
            page int64,
            xAuthToken string,
            limit *int64)(*models_pkg.ResourcesContactResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
page,_ := strconv.ParseInt("154", 10, 8)
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("154", 10, 8)

var result *models_pkg.ResourcesContactResourceModel
result,_ = contactController.ListPageUsingGET1(page, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="search_using_get1"></a>![Method: ](https://apidocs.io/img/method.png ".contact-controller_pkg.SearchUsingGET1") SearchUsingGET1

> *Tags:*  ``` Skips Authentication ``` 

> search


```go
func (me *CONTACTCONTROLLER_IMPL) SearchUsingGET1(
            name string,
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
name := "name"
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("154", 10, 8)

var result interface{}
result,_ = contactController.SearchUsingGET1(name, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".contact-controller_pkg.GetUsingGET") GetUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Show a contact


```go
func (me *CONTACTCONTROLLER_IMPL) GetUsingGET(
            id int64,
            xAuthToken string)(*models_pkg.ContactResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
id,_ := strconv.ParseInt("154", 10, 8)
xAuthToken := "X-Auth-Token"

var result *models_pkg.ContactResourceModel
result,_ = contactController.GetUsingGET(id, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_using_put"></a>![Method: ](https://apidocs.io/img/method.png ".contact-controller_pkg.UpdateUsingPUT") UpdateUsingPUT

> *Tags:*  ``` Skips Authentication ``` 

> Update a contact


```go
func (me *CONTACTCONTROLLER_IMPL) UpdateUsingPUT(
            id int64,
            resource *models_pkg.ContactResourceModel,
            xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
id,_ := strconv.ParseInt("154", 10, 8)
var resource *models_pkg.ContactResourceModel
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = contactController.UpdateUsingPUT(id, resource, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete1"></a>![Method: ](https://apidocs.io/img/method.png ".contact-controller_pkg.DeleteUsingDELETE1") DeleteUsingDELETE1

> *Tags:*  ``` Skips Authentication ``` 

> Delete a contact


```go
func (me *CONTACTCONTROLLER_IMPL) DeleteUsingDELETE1(
            id int64,
            xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
id,_ := strconv.ParseInt("154", 10, 8)
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = contactController.DeleteUsingDELETE1(id, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



### <a name="add_group_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".contact-controller_pkg.AddGroupUsingPOST") AddGroupUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Add a contact in a group


```go
func (me *CONTACTCONTROLLER_IMPL) AddGroupUsingPOST(
            id int64,
            groupId int64,
            xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| groupId |  ``` Required ```  | groupId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
id,_ := strconv.ParseInt("154", 10, 8)
groupId,_ := strconv.ParseInt("154", 10, 8)
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = contactController.AddGroupUsingPOST(id, groupId, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_groups_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".contact-controller_pkg.GetGroupsUsingGET") GetGroupsUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups for a contact


```go
func (me *CONTACTCONTROLLER_IMPL) GetGroupsUsingGET(
            id int64,
            page int64,
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
id,_ := strconv.ParseInt("154", 10, 8)
page,_ := strconv.ParseInt("154", 10, 8)
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("154", 10, 8)

var result interface{}
result,_ = contactController.GetGroupsUsingGET(id, page, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_group_using_delete"></a>![Method: ](https://apidocs.io/img/method.png ".contact-controller_pkg.DeleteGroupUsingDELETE") DeleteGroupUsingDELETE

> *Tags:*  ``` Skips Authentication ``` 

> Remove a contact from a group


```go
func (me *CONTACTCONTROLLER_IMPL) DeleteGroupUsingDELETE(
            id int64,
            groupId int64,
            xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| groupId |  ``` Required ```  | groupId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
id,_ := strconv.ParseInt("154", 10, 8)
groupId,_ := strconv.ParseInt("154", 10, 8)
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = contactController.DeleteGroupUsingDELETE(id, groupId, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



[Back to List of Controllers](#list_of_controllers)

## <a name="customer_controller_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".customer-controller_pkg") customer-controller_pkg

### Get instance

Factory for the ``` CUSTOMER-CONTROLLER ``` interface can be accessed from the package customer-controller_pkg.

```go
customerController := customer-controller_pkg.NewCUSTOMER-CONTROLLER()
```

### <a name="get_using_get2"></a>![Method: ](https://apidocs.io/img/method.png ".customer-controller_pkg.GetUsingGET2") GetUsingGET2

> *Tags:*  ``` Skips Authentication ``` 

> Show your account


```go
func (me *CUSTOMERCONTROLLER_IMPL) GetUsingGET2(xAuthToken string)(*models_pkg.CustomerResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"

var result *models_pkg.CustomerResourceModel
result,_ = customerController.GetUsingGET2(xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_from_fields_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".customer-controller_pkg.GetFromFieldsUsingGET") GetFromFieldsUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Get your personnalized sender IDs


```go
func (me *CUSTOMERCONTROLLER_IMPL) GetFromFieldsUsingGET(xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = customerController.GetFromFieldsUsingGET(xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_delete_sender_using_put"></a>![Method: ](https://apidocs.io/img/method.png ".customer-controller_pkg.UpdateDeleteSenderUsingPUT") UpdateDeleteSenderUsingPUT

> *Tags:*  ``` Skips Authentication ``` 

> Remove sender ID


```go
func (me *CUSTOMERCONTROLLER_IMPL) UpdateDeleteSenderUsingPUT(
            xAuthToken string,
            senderID string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| senderID |  ``` Required ```  | senderID |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"
senderID := "senderID"

var result interface{}
result,_ = customerController.UpdateDeleteSenderUsingPUT(xAuthToken, senderID)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="add_sender_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".customer-controller_pkg.AddSenderUsingPOST") AddSenderUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Add personnalized sender ID


```go
func (me *CUSTOMERCONTROLLER_IMPL) AddSenderUsingPOST(
            xAuthToken string,
            senderID string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| senderID |  ``` Required ```  | senderID |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"
senderID := "senderID"

var result interface{}
result,_ = customerController.AddSenderUsingPOST(xAuthToken, senderID)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_using_get3"></a>![Method: ](https://apidocs.io/img/method.png ".customer-controller_pkg.ListUsingGET3") ListUsingGET3

> *Tags:*  ``` Skips Authentication ``` 

> View a list of your subaccounts


```go
func (me *CUSTOMERCONTROLLER_IMPL) ListUsingGET3(
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("154", 10, 8)

var result interface{}
result,_ = customerController.ListUsingGET3(xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get3"></a>![Method: ](https://apidocs.io/img/method.png ".customer-controller_pkg.ListPageUsingGET3") ListPageUsingGET3

> *Tags:*  ``` Skips Authentication ``` 

> View a list of your subaccounts by page


```go
func (me *CUSTOMERCONTROLLER_IMPL) ListPageUsingGET3(
            page int64,
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
page,_ := strconv.ParseInt("154", 10, 8)
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("154", 10, 8)

var result interface{}
result,_ = customerController.ListPageUsingGET3(page, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="group_controller_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".group-controller_pkg") group-controller_pkg

### Get instance

Factory for the ``` GROUP-CONTROLLER ``` interface can be accessed from the package group-controller_pkg.

```go
groupController := group-controller_pkg.NewGROUP-CONTROLLER()
```

### <a name="list_using_get4"></a>![Method: ](https://apidocs.io/img/method.png ".group-controller_pkg.ListUsingGET4") ListUsingGET4

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups


```go
func (me *GROUPCONTROLLER_IMPL) ListUsingGET4(
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("154", 10, 8)

var result interface{}
result,_ = groupController.ListUsingGET4(xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="add_using_post2"></a>![Method: ](https://apidocs.io/img/method.png ".group-controller_pkg.AddUsingPOST2") AddUsingPOST2

> *Tags:*  ``` Skips Authentication ``` 

> Add a group


```go
func (me *GROUPCONTROLLER_IMPL) AddUsingPOST2(
            resource *models_pkg.GroupResourceModel,
            xAuthToken string)(*models_pkg.GroupResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
var resource *models_pkg.GroupResourceModel
xAuthToken := "X-Auth-Token"

var result *models_pkg.GroupResourceModel
result,_ = groupController.AddUsingPOST2(resource, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_delete_list_using_post1"></a>![Method: ](https://apidocs.io/img/method.png ".group-controller_pkg.CreateDeleteListUsingPOST1") CreateDeleteListUsingPOST1

> *Tags:*  ``` Skips Authentication ``` 

> Delete a list of groups


```go
func (me *GROUPCONTROLLER_IMPL) CreateDeleteListUsingPOST1(
            idList []int64,
            xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| idList |  ``` Required ```  ``` Collection ```  | idList |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
idList := []int64{154}
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = groupController.CreateDeleteListUsingPOST1(idList, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get4"></a>![Method: ](https://apidocs.io/img/method.png ".group-controller_pkg.ListPageUsingGET4") ListPageUsingGET4

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```go
func (me *GROUPCONTROLLER_IMPL) ListPageUsingGET4(
            page int64,
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
page,_ := strconv.ParseInt("154", 10, 8)
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("154", 10, 8)

var result interface{}
result,_ = groupController.ListPageUsingGET4(page, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="search_using_get2"></a>![Method: ](https://apidocs.io/img/method.png ".group-controller_pkg.SearchUsingGET2") SearchUsingGET2

> *Tags:*  ``` Skips Authentication ``` 

> search


```go
func (me *GROUPCONTROLLER_IMPL) SearchUsingGET2(
            name string,
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
name := "name"
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("154", 10, 8)

var result interface{}
result,_ = groupController.SearchUsingGET2(name, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get4"></a>![Method: ](https://apidocs.io/img/method.png ".group-controller_pkg.GetUsingGET4") GetUsingGET4

> *Tags:*  ``` Skips Authentication ``` 

> Show a group


```go
func (me *GROUPCONTROLLER_IMPL) GetUsingGET4(
            id int64,
            xAuthToken string)(*models_pkg.GroupResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
id,_ := strconv.ParseInt("154", 10, 8)
xAuthToken := "X-Auth-Token"

var result *models_pkg.GroupResourceModel
result,_ = groupController.GetUsingGET4(id, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_using_put2"></a>![Method: ](https://apidocs.io/img/method.png ".group-controller_pkg.UpdateUsingPUT2") UpdateUsingPUT2

> *Tags:*  ``` Skips Authentication ``` 

> Update a group


```go
func (me *GROUPCONTROLLER_IMPL) UpdateUsingPUT2(
            id int64,
            resource *models_pkg.GroupResourceModel,
            xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
id,_ := strconv.ParseInt("245", 10, 8)
var resource *models_pkg.GroupResourceModel
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = groupController.UpdateUsingPUT2(id, resource, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete3"></a>![Method: ](https://apidocs.io/img/method.png ".group-controller_pkg.DeleteUsingDELETE3") DeleteUsingDELETE3

> *Tags:*  ``` Skips Authentication ``` 

> Delete a group


```go
func (me *GROUPCONTROLLER_IMPL) DeleteUsingDELETE3(
            id int64,
            xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
id,_ := strconv.ParseInt("245", 10, 8)
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = groupController.DeleteUsingDELETE3(id, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



### <a name="get_contacts_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".group-controller_pkg.GetContactsUsingGET") GetContactsUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> Show a list of contacts for a group


```go
func (me *GROUPCONTROLLER_IMPL) GetContactsUsingGET(
            id int64,
            page int64,
            xAuthToken string,
            limit *int64)(*models_pkg.GroupResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
id,_ := strconv.ParseInt("245", 10, 8)
page,_ := strconv.ParseInt("245", 10, 8)
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("245", 10, 8)

var result *models_pkg.GroupResourceModel
result,_ = groupController.GetContactsUsingGET(id, page, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="campaign_controller_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".campaign-controller_pkg") campaign-controller_pkg

### Get instance

Factory for the ``` CAMPAIGN-CONTROLLER ``` interface can be accessed from the package campaign-controller_pkg.

```go
campaignController := campaign-controller_pkg.NewCAMPAIGN-CONTROLLER()
```

### <a name="list_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".campaign-controller_pkg.ListUsingGET") ListUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> list


```go
func (me *CAMPAIGNCONTROLLER_IMPL) ListUsingGET(
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("245", 10, 8)

var result interface{}
result,_ = campaignController.ListUsingGET(xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_send_to_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".campaign-controller_pkg.CreateSendToListUsingPOST") CreateSendToListUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> sendToList


```go
func (me *CAMPAIGNCONTROLLER_IMPL) CreateSendToListUsingPOST(
            resource *models_pkg.CampaignInputResourceModel,
            xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
var resource *models_pkg.CampaignInputResourceModel
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = campaignController.CreateSendToListUsingPOST(resource, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".campaign-controller_pkg.ListPageUsingGET") ListPageUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```go
func (me *CAMPAIGNCONTROLLER_IMPL) ListPageUsingGET(
            page int64,
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
page,_ := strconv.ParseInt("245", 10, 8)
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("245", 10, 8)

var result interface{}
result,_ = campaignController.ListPageUsingGET(page, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="search_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".campaign-controller_pkg.SearchUsingGET") SearchUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> search


```go
func (me *CAMPAIGNCONTROLLER_IMPL) SearchUsingGET(
            name string,
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
name := "name"
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("245", 10, 8)

var result interface{}
result,_ = campaignController.SearchUsingGET(name, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete"></a>![Method: ](https://apidocs.io/img/method.png ".campaign-controller_pkg.DeleteUsingDELETE") DeleteUsingDELETE

> *Tags:*  ``` Skips Authentication ``` 

> delete


```go
func (me *CAMPAIGNCONTROLLER_IMPL) DeleteUsingDELETE(
            messsageId string,
            xAuthToken string,
            id string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsageId |  ``` Required ```  | messsageId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| id |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
messsageId := "messsageId"
xAuthToken := "X-Auth-Token"
id := "id"

var result interface{}
result,_ = campaignController.DeleteUsingDELETE(messsageId, xAuthToken, id)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



[Back to List of Controllers](#list_of_controllers)

## <a name="transfer_controller_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".transfer-controller_pkg") transfer-controller_pkg

### Get instance

Factory for the ``` TRANSFER-CONTROLLER ``` interface can be accessed from the package transfer-controller_pkg.

```go
transferController := transfer-controller_pkg.NewTRANSFER-CONTROLLER()
```

### <a name="list_using_get9"></a>![Method: ](https://apidocs.io/img/method.png ".transfer-controller_pkg.ListUsingGET9") ListUsingGET9

> *Tags:*  ``` Skips Authentication ``` 

> View a list of transferts


```go
func (me *TRANSFERCONTROLLER_IMPL) ListUsingGET9(
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("245", 10, 8)

var result interface{}
result,_ = transferController.ListUsingGET9(xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get9"></a>![Method: ](https://apidocs.io/img/method.png ".transfer-controller_pkg.ListPageUsingGET9") ListPageUsingGET9

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```go
func (me *TRANSFERCONTROLLER_IMPL) ListPageUsingGET9(
            page int64,
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
page,_ := strconv.ParseInt("245", 10, 8)
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("245", 10, 8)

var result interface{}
result,_ = transferController.ListPageUsingGET9(page, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get9"></a>![Method: ](https://apidocs.io/img/method.png ".transfer-controller_pkg.GetUsingGET9") GetUsingGET9

> *Tags:*  ``` Skips Authentication ``` 

> Show a transfet


```go
func (me *TRANSFERCONTROLLER_IMPL) GetUsingGET9(
            id int64,
            xAuthToken string)(*models_pkg.TransferResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
id,_ := strconv.ParseInt("245", 10, 8)
xAuthToken := "X-Auth-Token"

var result *models_pkg.TransferResourceModel
result,_ = transferController.GetUsingGET9(id, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="email_api_configuration_controller_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".email-api-configuration-controller_pkg") email-api-configuration-controller_pkg

### Get instance

Factory for the ``` EMAIL-API-CONFIGURATION-CONTROLLER ``` interface can be accessed from the package email-api-configuration-controller_pkg.

```go
emailApiConfigurationController := email-api-configuration-controller_pkg.NewEMAIL-API-CONFIGURATION-CONTROLLER()
```

### <a name="get_using_get3"></a>![Method: ](https://apidocs.io/img/method.png ".email-api-configuration-controller_pkg.GetUsingGET3") GetUsingGET3

> *Tags:*  ``` Skips Authentication ``` 

> Show your configuration


```go
func (me *EMAILAPICONFIGURATIONCONTROLLER_IMPL) GetUsingGET3(xAuthToken string)(*models_pkg.EmailAPIConfigurationResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"

var result *models_pkg.EmailAPIConfigurationResourceModel
result,_ = emailApiConfigurationController.GetUsingGET3(xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_using_put1"></a>![Method: ](https://apidocs.io/img/method.png ".email-api-configuration-controller_pkg.UpdateUsingPUT1") UpdateUsingPUT1

> *Tags:*  ``` Skips Authentication ``` 

> Update your configuration


```go
func (me *EMAILAPICONFIGURATIONCONTROLLER_IMPL) UpdateUsingPUT1(
            resource *models_pkg.EmailAPIConfigurationResourceModel,
            xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
var resource *models_pkg.EmailAPIConfigurationResourceModel
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = emailApiConfigurationController.UpdateUsingPUT1(resource, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="add_using_post1"></a>![Method: ](https://apidocs.io/img/method.png ".email-api-configuration-controller_pkg.AddUsingPOST1") AddUsingPOST1

> *Tags:*  ``` Skips Authentication ``` 

> Create your configuration


```go
func (me *EMAILAPICONFIGURATIONCONTROLLER_IMPL) AddUsingPOST1(
            resource *models_pkg.EmailAPIConfigurationResourceModel,
            xAuthToken string)(*models_pkg.EmailAPIConfigurationResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
var resource *models_pkg.EmailAPIConfigurationResourceModel
xAuthToken := "X-Auth-Token"

var result *models_pkg.EmailAPIConfigurationResourceModel
result,_ = emailApiConfigurationController.AddUsingPOST1(resource, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete2"></a>![Method: ](https://apidocs.io/img/method.png ".email-api-configuration-controller_pkg.DeleteUsingDELETE2") DeleteUsingDELETE2

> *Tags:*  ``` Skips Authentication ``` 

> Delete your configuration


```go
func (me *EMAILAPICONFIGURATIONCONTROLLER_IMPL) DeleteUsingDELETE2(xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = emailApiConfigurationController.DeleteUsingDELETE2(xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



[Back to List of Controllers](#list_of_controllers)

## <a name="message_controller_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".message-controller_pkg") message-controller_pkg

### Get instance

Factory for the ``` MESSAGE-CONTROLLER ``` interface can be accessed from the package message-controller_pkg.

```go
messageController := message-controller_pkg.NewMESSAGE-CONTROLLER()
```

### <a name="list_using_get6"></a>![Method: ](https://apidocs.io/img/method.png ".message-controller_pkg.ListUsingGET6") ListUsingGET6

> *Tags:*  ``` Skips Authentication ``` 

> list


```go
func (me *MESSAGECONTROLLER_IMPL) ListUsingGET6(
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("245", 10, 8)

var result interface{}
result,_ = messageController.ListUsingGET6(xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get6"></a>![Method: ](https://apidocs.io/img/method.png ".message-controller_pkg.ListPageUsingGET6") ListPageUsingGET6

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```go
func (me *MESSAGECONTROLLER_IMPL) ListPageUsingGET6(
            page int64,
            xAuthToken string,
            limit *int64)(*models_pkg.PagedResourcesMessageResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
page,_ := strconv.ParseInt("245", 10, 8)
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("245", 10, 8)

var result *models_pkg.PagedResourcesMessageResourceModel
result,_ = messageController.ListPageUsingGET6(page, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_responses_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".message-controller_pkg.ListResponsesUsingGET") ListResponsesUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> listResponses


```go
func (me *MESSAGECONTROLLER_IMPL) ListResponsesUsingGET(
            xAuthToken string,
            limit *int64)(*models_pkg.ResourcesMessageResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("245", 10, 8)

var result *models_pkg.ResourcesMessageResourceModel
result,_ = messageController.ListResponsesUsingGET(xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_responses_page_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".message-controller_pkg.ListResponsesPageUsingGET") ListResponsesPageUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> listResponsesPage


```go
func (me *MESSAGECONTROLLER_IMPL) ListResponsesPageUsingGET(
            page int64,
            xAuthToken string,
            limit *int64)(*models_pkg.PagedResourcesMessageResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
page,_ := strconv.ParseInt("245", 10, 8)
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("245", 10, 8)

var result *models_pkg.PagedResourcesMessageResourceModel
result,_ = messageController.ListResponsesPageUsingGET(page, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_scheduled_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".message-controller_pkg.ListScheduledUsingGET") ListScheduledUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> listScheduled


```go
func (me *MESSAGECONTROLLER_IMPL) ListScheduledUsingGET(
            xAuthToken string,
            limit *int64)(*models_pkg.ResourcesMessageResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("245", 10, 8)

var result *models_pkg.ResourcesMessageResourceModel
result,_ = messageController.ListScheduledUsingGET(xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_scheduled_page_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".message-controller_pkg.ListScheduledPageUsingGET") ListScheduledPageUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> listScheduledPage


```go
func (me *MESSAGECONTROLLER_IMPL) ListScheduledPageUsingGET(
            page int64,
            xAuthToken string,
            limit *int64)(*models_pkg.PagedResourcesMessageResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
page,_ := strconv.ParseInt("245", 10, 8)
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("245", 10, 8)

var result *models_pkg.PagedResourcesMessageResourceModel
result,_ = messageController.ListScheduledPageUsingGET(page, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="search_using_get3"></a>![Method: ](https://apidocs.io/img/method.png ".message-controller_pkg.SearchUsingGET3") SearchUsingGET3

> *Tags:*  ``` Skips Authentication ``` 

> search


```go
func (me *MESSAGECONTROLLER_IMPL) SearchUsingGET3(
            id string,
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
id := "id"
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("245", 10, 8)

var result interface{}
result,_ = messageController.SearchUsingGET3(id, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_send_to_list_using_post1"></a>![Method: ](https://apidocs.io/img/method.png ".message-controller_pkg.CreateSendToListUsingPOST1") CreateSendToListUsingPOST1

> *Tags:*  ``` Skips Authentication ``` 

> sendToList


```go
func (me *MESSAGECONTROLLER_IMPL) CreateSendToListUsingPOST1(
            resource *models_pkg.MessageInputMixedResourceModel,
            xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
var resource *models_pkg.MessageInputMixedResourceModel
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = messageController.CreateSendToListUsingPOST1(resource, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_send_to_contact_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".message-controller_pkg.CreateSendToContactListUsingPOST") CreateSendToContactListUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> sendToContactList


```go
func (me *MESSAGECONTROLLER_IMPL) CreateSendToContactListUsingPOST(
            resource *models_pkg.MessageInputContactResourceModel,
            xAuthToken string)(,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
var resource *models_pkg.MessageInputContactResourceModel
xAuthToken := "X-Auth-Token"

var result 
result,_ = messageController.CreateSendToContactListUsingPOST(resource, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_send_to_group_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".message-controller_pkg.CreateSendToGroupListUsingPOST") CreateSendToGroupListUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> sendToGroupList


```go
func (me *MESSAGECONTROLLER_IMPL) CreateSendToGroupListUsingPOST(
            resource *models_pkg.MessageInputGroupResourceModel,
            xAuthToken string)(,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
var resource *models_pkg.MessageInputGroupResourceModel
xAuthToken := "X-Auth-Token"

var result 
result,_ = messageController.CreateSendToGroupListUsingPOST(resource, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_send_to_number_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".message-controller_pkg.CreateSendToNumberListUsingPOST") CreateSendToNumberListUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> sendToNumberList


```go
func (me *MESSAGECONTROLLER_IMPL) CreateSendToNumberListUsingPOST(
            resource *models_pkg.MessageInputResourceModel,
            xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
var resource *models_pkg.MessageInputResourceModel
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = messageController.CreateSendToNumberListUsingPOST(resource, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete4"></a>![Method: ](https://apidocs.io/img/method.png ".message-controller_pkg.DeleteUsingDELETE4") DeleteUsingDELETE4

> *Tags:*  ``` Skips Authentication ``` 

> delete


```go
func (me *MESSAGECONTROLLER_IMPL) DeleteUsingDELETE4(
            messsageId string,
            xAuthToken string,
            id string)(,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsageId |  ``` Required ```  | messsageId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| id |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
messsageId := "messsageId"
xAuthToken := "X-Auth-Token"
id := "id"

var result 
result,_ = messageController.DeleteUsingDELETE4(messsageId, xAuthToken, id)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



[Back to List of Controllers](#list_of_controllers)

## <a name="register_controler_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".register-controler_pkg") register-controler_pkg

### Get instance

Factory for the ``` REGISTER-CONTROLER ``` interface can be accessed from the package register-controler_pkg.

```go
registerControler := register-controler_pkg.NewREGISTER-CONTROLER()
```

### <a name="create_register_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".register-controler_pkg.CreateRegisterUsingPOST") CreateRegisterUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> register


```go
func (me *REGISTERCONTROLER_IMPL) CreateRegisterUsingPOST(resource *models_pkg.RegisterResourceModel)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |


#### Example Usage

```go
var resource *models_pkg.RegisterResourceModel

var result interface{}
result,_ = registerControler.CreateRegisterUsingPOST(resource)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_refresh_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".register-controler_pkg.CreateRefreshUsingPOST") CreateRefreshUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> refresh


```go
func (me *REGISTERCONTROLER_IMPL) CreateRefreshUsingPOST(resource *models_pkg.SimpleEmailResourceModel)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |


#### Example Usage

```go
var resource *models_pkg.SimpleEmailResourceModel

var result interface{}
result,_ = registerControler.CreateRefreshUsingPOST(resource)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_activate_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".register-controler_pkg.GetActivateUsingGET") GetActivateUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> activate


```go
func (me *REGISTERCONTROLER_IMPL) GetActivateUsingGET(
            token string,
            id int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| token |  ``` Required ```  | token |
| id |  ``` Required ```  | id |


#### Example Usage

```go
token := "token"
id,_ := strconv.ParseInt("245", 10, 8)

var result interface{}
result,_ = registerControler.GetActivateUsingGET(token, id)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="credit_consumption_controller_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".credit-consumption-controller_pkg") credit-consumption-controller_pkg

### Get instance

Factory for the ``` CREDIT-CONSUMPTION-CONTROLLER ``` interface can be accessed from the package credit-consumption-controller_pkg.

```go
creditConsumptionController := credit-consumption-controller_pkg.NewCREDIT-CONSUMPTION-CONTROLLER()
```

### <a name="list_using_get2"></a>![Method: ](https://apidocs.io/img/method.png ".credit-consumption-controller_pkg.ListUsingGET2") ListUsingGET2

> *Tags:*  ``` Skips Authentication ``` 

> Get the consumption of the last months


```go
func (me *CREDITCONSUMPTIONCONTROLLER_IMPL) ListUsingGET2(
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("245", 10, 8)

var result interface{}
result,_ = creditConsumptionController.ListUsingGET2(xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get2"></a>![Method: ](https://apidocs.io/img/method.png ".credit-consumption-controller_pkg.ListPageUsingGET2") ListPageUsingGET2

> *Tags:*  ``` Skips Authentication ``` 

> Get pageable consumption of the last months


```go
func (me *CREDITCONSUMPTIONCONTROLLER_IMPL) ListPageUsingGET2(
            page int64,
            xAuthToken string,
            limit *int64)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
page,_ := strconv.ParseInt("245", 10, 8)
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("245", 10, 8)

var result interface{}
result,_ = creditConsumptionController.ListPageUsingGET2(page, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get1"></a>![Method: ](https://apidocs.io/img/method.png ".credit-consumption-controller_pkg.GetUsingGET1") GetUsingGET1

> *Tags:*  ``` Skips Authentication ``` 

> Get specific consumption by id 


```go
func (me *CREDITCONSUMPTIONCONTROLLER_IMPL) GetUsingGET1(
            id int64,
            xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
id,_ := strconv.ParseInt("245", 10, 8)
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = creditConsumptionController.GetUsingGET1(id, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="pricing_controller_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".pricing-controller_pkg") pricing-controller_pkg

### Get instance

Factory for the ``` PRICING-CONTROLLER ``` interface can be accessed from the package pricing-controller_pkg.

```go
pricingController := pricing-controller_pkg.NewPRICING-CONTROLLER()
```

### <a name="get_using_get7"></a>![Method: ](https://apidocs.io/img/method.png ".pricing-controller_pkg.GetUsingGET7") GetUsingGET7

> *Tags:*  ``` Skips Authentication ``` 

> get


```go
func (me *PRICINGCONTROLLER_IMPL) GetUsingGET7(xAuthToken string)(*models_pkg.PricingResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"

var result *models_pkg.PricingResourceModel
result,_ = pricingController.GetUsingGET7(xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="message_model_controller_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".message-model-controller_pkg") message-model-controller_pkg

### Get instance

Factory for the ``` MESSAGE-MODEL-CONTROLLER ``` interface can be accessed from the package message-model-controller_pkg.

```go
messageModelController := message-model-controller_pkg.NewMESSAGE-MODEL-CONTROLLER()
```

### <a name="list_using_get7"></a>![Method: ](https://apidocs.io/img/method.png ".message-model-controller_pkg.ListUsingGET7") ListUsingGET7

> *Tags:*  ``` Skips Authentication ``` 

> list


```go
func (me *MESSAGEMODELCONTROLLER_IMPL) ListUsingGET7(
            xAuthToken string,
            size *int64)(*models_pkg.ResourcesMessageModelResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| size |  ``` Optional ```  | size |


#### Example Usage

```go
xAuthToken := "X-Auth-Token"
size,_ := strconv.ParseInt("245", 10, 8)

var result *models_pkg.ResourcesMessageModelResourceModel
result,_ = messageModelController.ListUsingGET7(xAuthToken, size)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="add_using_post3"></a>![Method: ](https://apidocs.io/img/method.png ".message-model-controller_pkg.AddUsingPOST3") AddUsingPOST3

> *Tags:*  ``` Skips Authentication ``` 

> add


```go
func (me *MESSAGEMODELCONTROLLER_IMPL) AddUsingPOST3(
            resource *models_pkg.MessageModelInputResourceModel,
            xAuthToken string)(*models_pkg.MessageModelResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
var resource *models_pkg.MessageModelInputResourceModel
xAuthToken := "X-Auth-Token"

var result *models_pkg.MessageModelResourceModel
result,_ = messageModelController.AddUsingPOST3(resource, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_delete_multiple_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".message-model-controller_pkg.CreateDeleteMultipleUsingPOST") CreateDeleteMultipleUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> deleteMultiple


```go
func (me *MESSAGEMODELCONTROLLER_IMPL) CreateDeleteMultipleUsingPOST(
            ids []string,
            xAuthToken string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ids |  ``` Required ```  ``` Collection ```  | ids |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
ids := []string{"ids"}
xAuthToken := "X-Auth-Token"

var result interface{}
result,_ = messageModelController.CreateDeleteMultipleUsingPOST(ids, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get7"></a>![Method: ](https://apidocs.io/img/method.png ".message-model-controller_pkg.ListPageUsingGET7") ListPageUsingGET7

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```go
func (me *MESSAGEMODELCONTROLLER_IMPL) ListPageUsingGET7(
            page int64,
            xAuthToken string,
            limit *int64)(*models_pkg.PagedResourcesMessageModelResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```go
page,_ := strconv.ParseInt("245", 10, 8)
xAuthToken := "X-Auth-Token"
limit,_ := strconv.ParseInt("245", 10, 8)

var result *models_pkg.PagedResourcesMessageModelResourceModel
result,_ = messageModelController.ListPageUsingGET7(page, xAuthToken, limit)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get6"></a>![Method: ](https://apidocs.io/img/method.png ".message-model-controller_pkg.GetUsingGET6") GetUsingGET6

> *Tags:*  ``` Skips Authentication ``` 

> get


```go
func (me *MESSAGEMODELCONTROLLER_IMPL) GetUsingGET6(
            id string,
            xAuthToken string)(*models_pkg.MessageModelResourceModel,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
id := "id"
xAuthToken := "X-Auth-Token"

var result *models_pkg.MessageModelResourceModel
result,_ = messageModelController.GetUsingGET6(id, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_using_put3"></a>![Method: ](https://apidocs.io/img/method.png ".message-model-controller_pkg.UpdateUsingPUT3") UpdateUsingPUT3

> *Tags:*  ``` Skips Authentication ``` 

> update


```go
func (me *MESSAGEMODELCONTROLLER_IMPL) UpdateUsingPUT3(
            id string,
            resource *models_pkg.MessageModelInputResourceModel,
            xAuthToken string)(,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
id := "id"
var resource *models_pkg.MessageModelInputResourceModel
xAuthToken := "X-Auth-Token"

var result 
result,_ = messageModelController.UpdateUsingPUT3(id, resource, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete5"></a>![Method: ](https://apidocs.io/img/method.png ".message-model-controller_pkg.DeleteUsingDELETE5") DeleteUsingDELETE5

> *Tags:*  ``` Skips Authentication ``` 

> delete


```go
func (me *MESSAGEMODELCONTROLLER_IMPL) DeleteUsingDELETE5(
            id string,
            xAuthToken string)(,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```go
id := "id"
xAuthToken := "X-Auth-Token"

var result 
result,_ = messageModelController.DeleteUsingDELETE5(id, xAuthToken)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



[Back to List of Controllers](#list_of_controllers)

## <a name="societe_info_controller_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".societe-info-controller_pkg") societe-info-controller_pkg

### Get instance

Factory for the ``` SOCIETE-INFO-CONTROLLER ``` interface can be accessed from the package societe-info-controller_pkg.

```go
societeInfoController := societe-info-controller_pkg.NewSOCIETE-INFO-CONTROLLER()
```

### <a name="create_research_company_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".societe-info-controller_pkg.CreateResearchCompanyUsingPOST") CreateResearchCompanyUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> researchCompany


```go
func (me *SOCIETEINFOCONTROLLER_IMPL) CreateResearchCompanyUsingPOST(research *models_pkg.SocieteInfoResearchResourceModel)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| research |  ``` Required ```  | research |


#### Example Usage

```go
var research *models_pkg.SocieteInfoResearchResourceModel

var result interface{}
result,_ = societeInfoController.CreateResearchCompanyUsingPOST(research)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_details_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".societe-info-controller_pkg.GetDetailsUsingGET") GetDetailsUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> getDetails


```go
func (me *SOCIETEINFOCONTROLLER_IMPL) GetDetailsUsingGET(id string)(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |


#### Example Usage

```go
id := "id"

var result interface{}
result,_ = societeInfoController.GetDetailsUsingGET(id)

```

#### Errors
 
| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)



