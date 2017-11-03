# Getting started

sMsMode API-REST Documentation

## How to Build

The generated code uses a few Maven dependencies e.g., Jackson, UniRest,
and Apache HttpClient. The reference to these dependencies is already
added in the pom.xml file will be installed automatically. Therefore,
you will need internet access for a successful build.

* In order to open the client library in Eclipse click on ``` File -> Import ```.

![Importing SDK into Eclipse - Step 1](https://apidocs.io/illustration/java?step=import0&workspaceFolder=sMsmode%20API-REST-Java&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIRESTLib&rootNamespace=com.smsmode.rest)

* In the import dialog, select ``` Existing Java Project ``` and click ``` Next ```.

![Importing SDK into Eclipse - Step 2](https://apidocs.io/illustration/java?step=import1&workspaceFolder=sMsmode%20API-REST-Java&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIRESTLib&rootNamespace=com.smsmode.rest)

* Browse to locate the folder containing the source code. Select the detected location of the project and click ``` Finish ```.

![Importing SDK into Eclipse - Step 3](https://apidocs.io/illustration/java?step=import2&workspaceFolder=sMsmode%20API-REST-Java&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIRESTLib&rootNamespace=com.smsmode.rest)

* Upon successful import, the project will be automatically built by Eclipse after automatically resolving the dependencies.

![Importing SDK into Eclipse - Step 4](https://apidocs.io/illustration/java?step=import3&workspaceFolder=sMsmode%20API-REST-Java&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIRESTLib&rootNamespace=com.smsmode.rest)

## How to Use

The following section explains how to use the SMsmodeAPIREST library in a new console project.

### 1. Starting a new project

For starting a new project, click the menu command ``` File > New > Project ```.

![Add a new project in Eclipse](https://apidocs.io/illustration/java?step=createNewProject0&workspaceFolder=sMsmode%20API-REST-Java&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIRESTLib&rootNamespace=com.smsmode.rest)

Next, choose ``` Maven > Maven Project ```and click ``` Next ```.

![Create a new Maven Project - Step 1](https://apidocs.io/illustration/java?step=createNewProject1&workspaceFolder=sMsmode%20API-REST-Java&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIRESTLib&rootNamespace=com.smsmode.rest)

Here, make sure to use the current workspace by choosing ``` Use default Workspace location ```, as shown in the picture below and click ``` Next ```.

![Create a new Maven Project - Step 2](https://apidocs.io/illustration/java?step=createNewProject2&workspaceFolder=sMsmode%20API-REST-Java&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIRESTLib&rootNamespace=com.smsmode.rest)

Following this, select the *quick start* project type to create a simple project with an existing class and a ``` main ``` method. To do this, choose ``` maven-archetype-quickstart ``` item from the list and click ``` Next ```.

![Create a new Maven Project - Step 3](https://apidocs.io/illustration/java?step=createNewProject3&workspaceFolder=sMsmode%20API-REST-Java&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIRESTLib&rootNamespace=com.smsmode.rest)

In the last step, provide a ``` Group Id ``` and ``` Artifact Id ``` as shown in the picture below and click ``` Finish ```.

![Create a new Maven Project - Step 4](https://apidocs.io/illustration/java?step=createNewProject4&workspaceFolder=sMsmode%20API-REST-Java&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIRESTLib&rootNamespace=com.smsmode.rest)

### 2. Add reference of the library project

The created Maven project manages its dependencies using its ``` pom.xml ``` file. In order to add a dependency on the *SMsmodeAPIRESTLib* client library, double click on the ``` pom.xml ``` file in the ``` Package Explorer ```. Opening the ``` pom.xml ``` file will render a graphical view on the cavas. Here, switch to the ``` Dependencies ``` tab and click the ``` Add ``` button as shown in the picture below.

![Adding dependency to the client library - Step 1](https://apidocs.io/illustration/java?step=testProject0&workspaceFolder=sMsmode%20API-REST-Java&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIRESTLib&rootNamespace=com.smsmode.rest)

Clicking the ``` Add ``` button will open a dialog where you need to specify SMsmodeAPIREST in ``` Group Id ``` and SMsmodeAPIRESTLib in the ``` Artifact Id ``` fields. Once added click ``` OK ```. Save the ``` pom.xml ``` file.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/java?step=testProject1&workspaceFolder=sMsmode%20API-REST-Java&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIRESTLib&rootNamespace=com.smsmode.rest)

### 3. Write sample code

Once the ``` SimpleConsoleApp ``` is created, a file named ``` App.java ``` will be visible in the *Package Explorer* with a ``` main ``` method. This is the entry point for the execution of the created project.
Here, you can add code to initialize the client library and instantiate a *Controller* class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/java?step=testProject2&workspaceFolder=sMsmode%20API-REST-Java&workspaceName=SMsmodeAPIREST&projectName=SMsmodeAPIRESTLib&rootNamespace=com.smsmode.rest)

## How to Test

The generated code and the server can be tested using automatically generated test cases. 
JUnit is used as the testing framework and test runner.

In Eclipse, for running the tests do the following:

1. Select the project *SMsmodeAPIRESTLib* from the package explorer.
2. Select "Run -> Run as -> JUnit Test" or use "Alt + Shift + X" followed by "T" to run the Tests.

## Initialization

### 

API client can be initialized as following.

```java

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

## <a name="report_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.smsmode.rest.controllers.ReportController") ReportController

### Get singleton instance

The singleton instance of the ``` ReportController ``` class can be accessed from the API Client.

```java
ReportController reportController = client.getReportController();
```

### <a name="list_using_get8_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ReportController.listUsingGET8Async") listUsingGET8Async

> *Tags:*  ``` Skips Authentication ``` 

> list


```java
void listUsingGET8Async(
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
Integer limit = 113;
// Invoking the API call with sample inputs
reportController.listUsingGET8Async(xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get8_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ReportController.listPageUsingGET8Async") listPageUsingGET8Async

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```java
void listPageUsingGET8Async(
        final int page,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
int page = 113;
String xAuthToken = "X-Auth-Token";
Integer limit = 113;
// Invoking the API call with sample inputs
reportController.listPageUsingGET8Async(page, xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get8_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ReportController.getUsingGET8Async") getUsingGET8Async

> *Tags:*  ``` Skips Authentication ``` 

> get


```java
void getUsingGET8Async(
        final String messageRef,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String messageRef = "messageRef";
String xAuthToken = "X-Auth-Token";
Integer limit = 113;
// Invoking the API call with sample inputs
reportController.getUsingGET8Async(messageRef, xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_page_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ReportController.getPageUsingGETAsync") getPageUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> getPage


```java
void getPageUsingGETAsync(
        final String messageRef,
        final int page,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String messageRef = "messageRef";
int page = 113;
String xAuthToken = "X-Auth-Token";
Integer limit = 113;
// Invoking the API call with sample inputs
reportController.getPageUsingGETAsync(messageRef, page, xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="find_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ReportController.findUsingGETAsync") findUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> find


```java
void findUsingGETAsync(
        final String messageRef,
        final String destinataire,
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| destinataire |  ``` Required ```  | destinataire |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
String messageRef = "messageRef";
String destinataire = "destinataire";
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
reportController.findUsingGETAsync(messageRef, destinataire, xAuthToken, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="invoice_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.smsmode.rest.controllers.InvoiceController") InvoiceController

### Get singleton instance

The singleton instance of the ``` InvoiceController ``` class can be accessed from the API Client.

```java
InvoiceController invoiceController = client.getInvoiceController();
```

### <a name="list_using_get5_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.InvoiceController.listUsingGET5Async") listUsingGET5Async

> *Tags:*  ``` Skips Authentication ``` 

> View a list of invoices


```java
void listUsingGET5Async(
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
Integer limit = 113;
// Invoking the API call with sample inputs
invoiceController.listUsingGET5Async(xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get5_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.InvoiceController.listPageUsingGET5Async") listPageUsingGET5Async

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```java
void listPageUsingGET5Async(
        final int page,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
int page = 113;
String xAuthToken = "X-Auth-Token";
Integer limit = 113;
// Invoking the API call with sample inputs
invoiceController.listPageUsingGET5Async(page, xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_pdf_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.InvoiceController.getPdfUsingGETAsync") getPdfUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> Generate an invoice in a pdf file


```java
void getPdfUsingGETAsync(
        final int id,
        final String xAuthToken,
        final boolean base64,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| base64 |  ``` Required ```  | base64 |


#### Example Usage

```java
int id = 113;
String xAuthToken = "X-Auth-Token";
boolean base64 = false;
// Invoking the API call with sample inputs
invoiceController.getPdfUsingGETAsync(id, xAuthToken, base64, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get5_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.InvoiceController.getUsingGET5Async") getUsingGET5Async

> *Tags:*  ``` Skips Authentication ``` 

> Show an invoice


```java
void getUsingGET5Async(
        final int id,
        final String xAuthToken,
        final APICallBack<InvoiceResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
int id = 113;
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
invoiceController.getUsingGET5Async(id, xAuthToken, new APICallBack<InvoiceResourceModel>() {
    public void onSuccess(HttpContext context, InvoiceResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="authentication_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.smsmode.rest.controllers.AuthenticationController") AuthenticationController

### Get singleton instance

The singleton instance of the ``` AuthenticationController ``` class can be accessed from the API Client.

```java
AuthenticationController authenticationController = client.getAuthenticationController();
```

### <a name="create_get_token_using_post_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.AuthenticationController.createGetTokenUsingPOSTAsync") createGetTokenUsingPOSTAsync

> *Tags:*  ``` Skips Authentication ``` 

> Generate the OAuth Token


```java
void createGetTokenUsingPOSTAsync(
        final AuthenticationResourceModel request,
        final APICallBack<TokenResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| request |  ``` Required ```  | request |


#### Example Usage

```java
try {
    AuthenticationResourceModel request = new AuthenticationResourceModel();
    // Invoking the API call with sample inputs
    authenticationController.createGetTokenUsingPOSTAsync(request, new APICallBack<TokenResourceModel>() {
        public void onSuccess(HttpContext context, TokenResourceModel response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="contact_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.smsmode.rest.controllers.ContactController") ContactController

### Get singleton instance

The singleton instance of the ``` ContactController ``` class can be accessed from the API Client.

```java
ContactController contactController = client.getContactController();
```

### <a name="list_using_get1_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ContactController.listUsingGET1Async") listUsingGET1Async

> *Tags:*  ``` Skips Authentication ``` 

> View a list of contacts


```java
void listUsingGET1Async(
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
Integer limit = 113;
// Invoking the API call with sample inputs
contactController.listUsingGET1Async(xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="add_using_post_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ContactController.addUsingPOSTAsync") addUsingPOSTAsync

> *Tags:*  ``` Skips Authentication ``` 

> Add a contact


```java
void addUsingPOSTAsync(
        final ContactResourceModel resource,
        final String xAuthToken,
        final APICallBack<ContactResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    ContactResourceModel resource = new ContactResourceModel();
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    contactController.addUsingPOSTAsync(resource, xAuthToken, new APICallBack<ContactResourceModel>() {
        public void onSuccess(HttpContext context, ContactResourceModel response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_book_using_delete_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ContactController.deleteBookUsingDELETEAsync") deleteBookUsingDELETEAsync

> *Tags:*  ``` Skips Authentication ``` 

> Remove all contacts and groups of the account


```java
void deleteBookUsingDELETEAsync(
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
contactController.deleteBookUsingDELETEAsync(xAuthToken, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



### <a name="get_customer_info_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ContactController.getCustomerInfoUsingGETAsync") getCustomerInfoUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> Show contact info of customer


```java
void getCustomerInfoUsingGETAsync(
        final String xAuthToken,
        final APICallBack<ContactResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
contactController.getCustomerInfoUsingGETAsync(xAuthToken, new APICallBack<ContactResourceModel>() {
    public void onSuccess(HttpContext context, ContactResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_edit_customer_using_put_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ContactController.updateEditCustomerUsingPUTAsync") updateEditCustomerUsingPUTAsync

> *Tags:*  ``` Skips Authentication ``` 

> Edit contact info of customer


```java
void updateEditCustomerUsingPUTAsync(
        final String xAuthToken,
        final ContactResourceModel resource,
        final APICallBack<ContactResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| resource |  ``` Required ```  | resource |


#### Example Usage

```java
try {
    String xAuthToken = "X-Auth-Token";
    ContactResourceModel resource = new ContactResourceModel();
    // Invoking the API call with sample inputs
    contactController.updateEditCustomerUsingPUTAsync(xAuthToken, resource, new APICallBack<ContactResourceModel>() {
        public void onSuccess(HttpContext context, ContactResourceModel response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_delete_list_using_post_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ContactController.createDeleteListUsingPOSTAsync") createDeleteListUsingPOSTAsync

> *Tags:*  ``` Skips Authentication ``` 

> Delete a list of contacts


```java
void createDeleteListUsingPOSTAsync(
        final List<Integer> idList,
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| idList |  ``` Required ```  ``` Collection ```  | idList |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    List<Integer> idList = new LinkedList<Integer>(Arrays.asList(113));
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    contactController.createDeleteListUsingPOSTAsync(idList, xAuthToken, new APICallBack<DynamicResponse>() {
        public void onSuccess(HttpContext context, DynamicResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_export_contacts_using_post_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ContactController.createExportContactsUsingPOSTAsync") createExportContactsUsingPOSTAsync

> *Tags:*  ``` Skips Authentication ``` 

> Export contacts in csv format


```java
void createExportContactsUsingPOSTAsync(
        final List<String> fields,
        final String xAuthToken,
        final APICallBack<DeferredResultResponseEntityObjectModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fields |  ``` Required ```  ``` Collection ```  | fields |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    List<String> fields = new LinkedList<String>(Arrays.asList("fields"));
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    contactController.createExportContactsUsingPOSTAsync(fields, xAuthToken, new APICallBack<DeferredResultResponseEntityObjectModel>() {
        public void onSuccess(HttpContext context, DeferredResultResponseEntityObjectModel response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="upload_blocking_using_post_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ContactController.uploadBlockingUsingPOSTAsync") uploadBlockingUsingPOSTAsync

> *Tags:*  ``` Skips Authentication ``` 

> Import contacts via xls or csv files


```java
void uploadBlockingUsingPOSTAsync(
        final File file,
        final String model,
        final String xAuthToken,
        final APICallBack<DeferredResultResponseEntityObjectModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | file |
| model |  ``` Required ```  | model |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
File file = new File("PathToFile");
String model = "model";
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
contactController.uploadBlockingUsingPOSTAsync(file, model, xAuthToken, new APICallBack<DeferredResultResponseEntityObjectModel>() {
    public void onSuccess(HttpContext context, DeferredResultResponseEntityObjectModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get1_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ContactController.listPageUsingGET1Async") listPageUsingGET1Async

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```java
void listPageUsingGET1Async(
        final int page,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<ResourcesContactResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
int page = 113;
String xAuthToken = "X-Auth-Token";
Integer limit = 113;
// Invoking the API call with sample inputs
contactController.listPageUsingGET1Async(page, xAuthToken, limit, new APICallBack<ResourcesContactResourceModel>() {
    public void onSuccess(HttpContext context, ResourcesContactResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="search_using_get1_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ContactController.searchUsingGET1Async") searchUsingGET1Async

> *Tags:*  ``` Skips Authentication ``` 

> search


```java
void searchUsingGET1Async(
        final String name,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String name = "name";
String xAuthToken = "X-Auth-Token";
Integer limit = 113;
// Invoking the API call with sample inputs
contactController.searchUsingGET1Async(name, xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ContactController.getUsingGETAsync") getUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> Show a contact


```java
void getUsingGETAsync(
        final int id,
        final String xAuthToken,
        final APICallBack<ContactResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
int id = 113;
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
contactController.getUsingGETAsync(id, xAuthToken, new APICallBack<ContactResourceModel>() {
    public void onSuccess(HttpContext context, ContactResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_using_put_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ContactController.updateUsingPUTAsync") updateUsingPUTAsync

> *Tags:*  ``` Skips Authentication ``` 

> Update a contact


```java
void updateUsingPUTAsync(
        final int id,
        final ContactResourceModel resource,
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    int id = 113;
    ContactResourceModel resource = new ContactResourceModel();
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    contactController.updateUsingPUTAsync(id, resource, xAuthToken, new APICallBack<DynamicResponse>() {
        public void onSuccess(HttpContext context, DynamicResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete1_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ContactController.deleteUsingDELETE1Async") deleteUsingDELETE1Async

> *Tags:*  ``` Skips Authentication ``` 

> Delete a contact


```java
void deleteUsingDELETE1Async(
        final int id,
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
int id = 113;
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
contactController.deleteUsingDELETE1Async(id, xAuthToken, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



### <a name="add_group_using_post_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ContactController.addGroupUsingPOSTAsync") addGroupUsingPOSTAsync

> *Tags:*  ``` Skips Authentication ``` 

> Add a contact in a group


```java
void addGroupUsingPOSTAsync(
        final int id,
        final int groupId,
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| groupId |  ``` Required ```  | groupId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
int id = 113;
int groupId = 113;
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
contactController.addGroupUsingPOSTAsync(id, groupId, xAuthToken, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_groups_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ContactController.getGroupsUsingGETAsync") getGroupsUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups for a contact


```java
void getGroupsUsingGETAsync(
        final int id,
        final int page,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
int id = 113;
int page = 113;
String xAuthToken = "X-Auth-Token";
Integer limit = 113;
// Invoking the API call with sample inputs
contactController.getGroupsUsingGETAsync(id, page, xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_group_using_delete_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.ContactController.deleteGroupUsingDELETEAsync") deleteGroupUsingDELETEAsync

> *Tags:*  ``` Skips Authentication ``` 

> Remove a contact from a group


```java
void deleteGroupUsingDELETEAsync(
        final int id,
        final int groupId,
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| groupId |  ``` Required ```  | groupId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
int id = 113;
int groupId = 113;
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
contactController.deleteGroupUsingDELETEAsync(id, groupId, xAuthToken, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



[Back to List of Controllers](#list_of_controllers)

## <a name="customer_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.smsmode.rest.controllers.CustomerController") CustomerController

### Get singleton instance

The singleton instance of the ``` CustomerController ``` class can be accessed from the API Client.

```java
CustomerController customerController = client.getCustomerController();
```

### <a name="get_using_get2_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.CustomerController.getUsingGET2Async") getUsingGET2Async

> *Tags:*  ``` Skips Authentication ``` 

> Show your account


```java
void getUsingGET2Async(
        final String xAuthToken,
        final APICallBack<CustomerResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
customerController.getUsingGET2Async(xAuthToken, new APICallBack<CustomerResourceModel>() {
    public void onSuccess(HttpContext context, CustomerResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_from_fields_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.CustomerController.getFromFieldsUsingGETAsync") getFromFieldsUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> Get your personnalized sender IDs


```java
void getFromFieldsUsingGETAsync(
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
customerController.getFromFieldsUsingGETAsync(xAuthToken, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_delete_sender_using_put_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.CustomerController.updateDeleteSenderUsingPUTAsync") updateDeleteSenderUsingPUTAsync

> *Tags:*  ``` Skips Authentication ``` 

> Remove sender ID


```java
void updateDeleteSenderUsingPUTAsync(
        final String xAuthToken,
        final String senderID,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| senderID |  ``` Required ```  | senderID |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
String senderID = "senderID";
// Invoking the API call with sample inputs
customerController.updateDeleteSenderUsingPUTAsync(xAuthToken, senderID, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="add_sender_using_post_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.CustomerController.addSenderUsingPOSTAsync") addSenderUsingPOSTAsync

> *Tags:*  ``` Skips Authentication ``` 

> Add personnalized sender ID


```java
void addSenderUsingPOSTAsync(
        final String xAuthToken,
        final String senderID,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| senderID |  ``` Required ```  | senderID |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
String senderID = "senderID";
// Invoking the API call with sample inputs
customerController.addSenderUsingPOSTAsync(xAuthToken, senderID, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_using_get3_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.CustomerController.listUsingGET3Async") listUsingGET3Async

> *Tags:*  ``` Skips Authentication ``` 

> View a list of your subaccounts


```java
void listUsingGET3Async(
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
customerController.listUsingGET3Async(xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get3_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.CustomerController.listPageUsingGET3Async") listPageUsingGET3Async

> *Tags:*  ``` Skips Authentication ``` 

> View a list of your subaccounts by page


```java
void listPageUsingGET3Async(
        final int page,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
int page = 204;
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
customerController.listPageUsingGET3Async(page, xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="group_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.smsmode.rest.controllers.GroupController") GroupController

### Get singleton instance

The singleton instance of the ``` GroupController ``` class can be accessed from the API Client.

```java
GroupController groupController = client.getGroupController();
```

### <a name="list_using_get4_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.GroupController.listUsingGET4Async") listUsingGET4Async

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups


```java
void listUsingGET4Async(
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
groupController.listUsingGET4Async(xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="add_using_post2_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.GroupController.addUsingPOST2Async") addUsingPOST2Async

> *Tags:*  ``` Skips Authentication ``` 

> Add a group


```java
void addUsingPOST2Async(
        final GroupResourceModel resource,
        final String xAuthToken,
        final APICallBack<GroupResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    GroupResourceModel resource = new GroupResourceModel();
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    groupController.addUsingPOST2Async(resource, xAuthToken, new APICallBack<GroupResourceModel>() {
        public void onSuccess(HttpContext context, GroupResourceModel response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_delete_list_using_post1_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.GroupController.createDeleteListUsingPOST1Async") createDeleteListUsingPOST1Async

> *Tags:*  ``` Skips Authentication ``` 

> Delete a list of groups


```java
void createDeleteListUsingPOST1Async(
        final List<Integer> idList,
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| idList |  ``` Required ```  ``` Collection ```  | idList |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    List<Integer> idList = new LinkedList<Integer>(Arrays.asList(204));
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    groupController.createDeleteListUsingPOST1Async(idList, xAuthToken, new APICallBack<DynamicResponse>() {
        public void onSuccess(HttpContext context, DynamicResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get4_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.GroupController.listPageUsingGET4Async") listPageUsingGET4Async

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```java
void listPageUsingGET4Async(
        final int page,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
int page = 204;
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
groupController.listPageUsingGET4Async(page, xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="search_using_get2_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.GroupController.searchUsingGET2Async") searchUsingGET2Async

> *Tags:*  ``` Skips Authentication ``` 

> search


```java
void searchUsingGET2Async(
        final String name,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String name = "name";
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
groupController.searchUsingGET2Async(name, xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get4_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.GroupController.getUsingGET4Async") getUsingGET4Async

> *Tags:*  ``` Skips Authentication ``` 

> Show a group


```java
void getUsingGET4Async(
        final int id,
        final String xAuthToken,
        final APICallBack<GroupResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
int id = 204;
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
groupController.getUsingGET4Async(id, xAuthToken, new APICallBack<GroupResourceModel>() {
    public void onSuccess(HttpContext context, GroupResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_using_put2_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.GroupController.updateUsingPUT2Async") updateUsingPUT2Async

> *Tags:*  ``` Skips Authentication ``` 

> Update a group


```java
void updateUsingPUT2Async(
        final int id,
        final GroupResourceModel resource,
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    int id = 204;
    GroupResourceModel resource = new GroupResourceModel();
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    groupController.updateUsingPUT2Async(id, resource, xAuthToken, new APICallBack<DynamicResponse>() {
        public void onSuccess(HttpContext context, DynamicResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete3_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.GroupController.deleteUsingDELETE3Async") deleteUsingDELETE3Async

> *Tags:*  ``` Skips Authentication ``` 

> Delete a group


```java
void deleteUsingDELETE3Async(
        final int id,
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
int id = 204;
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
groupController.deleteUsingDELETE3Async(id, xAuthToken, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



### <a name="get_contacts_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.GroupController.getContactsUsingGETAsync") getContactsUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> Show a list of contacts for a group


```java
void getContactsUsingGETAsync(
        final int id,
        final int page,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<GroupResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
int id = 204;
int page = 204;
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
groupController.getContactsUsingGETAsync(id, page, xAuthToken, limit, new APICallBack<GroupResourceModel>() {
    public void onSuccess(HttpContext context, GroupResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="campaign_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.smsmode.rest.controllers.CampaignController") CampaignController

### Get singleton instance

The singleton instance of the ``` CampaignController ``` class can be accessed from the API Client.

```java
CampaignController campaignController = client.getCampaignController();
```

### <a name="list_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.CampaignController.listUsingGETAsync") listUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> list


```java
void listUsingGETAsync(
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
campaignController.listUsingGETAsync(xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_send_to_list_using_post_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.CampaignController.createSendToListUsingPOSTAsync") createSendToListUsingPOSTAsync

> *Tags:*  ``` Skips Authentication ``` 

> sendToList


```java
void createSendToListUsingPOSTAsync(
        final CampaignInputResourceModel resource,
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    CampaignInputResourceModel resource = new CampaignInputResourceModel();
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    campaignController.createSendToListUsingPOSTAsync(resource, xAuthToken, new APICallBack<DynamicResponse>() {
        public void onSuccess(HttpContext context, DynamicResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.CampaignController.listPageUsingGETAsync") listPageUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```java
void listPageUsingGETAsync(
        final int page,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
int page = 204;
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
campaignController.listPageUsingGETAsync(page, xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="search_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.CampaignController.searchUsingGETAsync") searchUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> search


```java
void searchUsingGETAsync(
        final String name,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String name = "name";
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
campaignController.searchUsingGETAsync(name, xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.CampaignController.deleteUsingDELETEAsync") deleteUsingDELETEAsync

> *Tags:*  ``` Skips Authentication ``` 

> delete


```java
void deleteUsingDELETEAsync(
        final String messsageId,
        final String xAuthToken,
        final String id,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsageId |  ``` Required ```  | messsageId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| id |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
String messsageId = "messsageId";
String xAuthToken = "X-Auth-Token";
String id = "id";
// Invoking the API call with sample inputs
campaignController.deleteUsingDELETEAsync(messsageId, xAuthToken, id, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



[Back to List of Controllers](#list_of_controllers)

## <a name="transfer_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.smsmode.rest.controllers.TransferController") TransferController

### Get singleton instance

The singleton instance of the ``` TransferController ``` class can be accessed from the API Client.

```java
TransferController transferController = client.getTransferController();
```

### <a name="list_using_get9_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.TransferController.listUsingGET9Async") listUsingGET9Async

> *Tags:*  ``` Skips Authentication ``` 

> View a list of transferts


```java
void listUsingGET9Async(
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
transferController.listUsingGET9Async(xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get9_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.TransferController.listPageUsingGET9Async") listPageUsingGET9Async

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```java
void listPageUsingGET9Async(
        final int page,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
int page = 204;
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
transferController.listPageUsingGET9Async(page, xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get9_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.TransferController.getUsingGET9Async") getUsingGET9Async

> *Tags:*  ``` Skips Authentication ``` 

> Show a transfet


```java
void getUsingGET9Async(
        final int id,
        final String xAuthToken,
        final APICallBack<TransferResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
int id = 204;
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
transferController.getUsingGET9Async(id, xAuthToken, new APICallBack<TransferResourceModel>() {
    public void onSuccess(HttpContext context, TransferResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="email_api_configuration_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.smsmode.rest.controllers.EmailApiConfigurationController") EmailApiConfigurationController

### Get singleton instance

The singleton instance of the ``` EmailApiConfigurationController ``` class can be accessed from the API Client.

```java
EmailApiConfigurationController emailApiConfigurationController = client.getEmailApiConfigurationController();
```

### <a name="get_using_get3_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.EmailApiConfigurationController.getUsingGET3Async") getUsingGET3Async

> *Tags:*  ``` Skips Authentication ``` 

> Show your configuration


```java
void getUsingGET3Async(
        final String xAuthToken,
        final APICallBack<EmailAPIConfigurationResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
emailApiConfigurationController.getUsingGET3Async(xAuthToken, new APICallBack<EmailAPIConfigurationResourceModel>() {
    public void onSuccess(HttpContext context, EmailAPIConfigurationResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_using_put1_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.EmailApiConfigurationController.updateUsingPUT1Async") updateUsingPUT1Async

> *Tags:*  ``` Skips Authentication ``` 

> Update your configuration


```java
void updateUsingPUT1Async(
        final EmailAPIConfigurationResourceModel resource,
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    EmailAPIConfigurationResourceModel resource = new EmailAPIConfigurationResourceModel();
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    emailApiConfigurationController.updateUsingPUT1Async(resource, xAuthToken, new APICallBack<DynamicResponse>() {
        public void onSuccess(HttpContext context, DynamicResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="add_using_post1_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.EmailApiConfigurationController.addUsingPOST1Async") addUsingPOST1Async

> *Tags:*  ``` Skips Authentication ``` 

> Create your configuration


```java
void addUsingPOST1Async(
        final EmailAPIConfigurationResourceModel resource,
        final String xAuthToken,
        final APICallBack<EmailAPIConfigurationResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    EmailAPIConfigurationResourceModel resource = new EmailAPIConfigurationResourceModel();
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    emailApiConfigurationController.addUsingPOST1Async(resource, xAuthToken, new APICallBack<EmailAPIConfigurationResourceModel>() {
        public void onSuccess(HttpContext context, EmailAPIConfigurationResourceModel response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete2_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.EmailApiConfigurationController.deleteUsingDELETE2Async") deleteUsingDELETE2Async

> *Tags:*  ``` Skips Authentication ``` 

> Delete your configuration


```java
void deleteUsingDELETE2Async(
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
emailApiConfigurationController.deleteUsingDELETE2Async(xAuthToken, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



[Back to List of Controllers](#list_of_controllers)

## <a name="message_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.smsmode.rest.controllers.MessageController") MessageController

### Get singleton instance

The singleton instance of the ``` MessageController ``` class can be accessed from the API Client.

```java
MessageController messageController = client.getMessageController();
```

### <a name="list_using_get6_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageController.listUsingGET6Async") listUsingGET6Async

> *Tags:*  ``` Skips Authentication ``` 

> list


```java
void listUsingGET6Async(
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
messageController.listUsingGET6Async(xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get6_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageController.listPageUsingGET6Async") listPageUsingGET6Async

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```java
void listPageUsingGET6Async(
        final int page,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<PagedResourcesMessageResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
int page = 204;
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
messageController.listPageUsingGET6Async(page, xAuthToken, limit, new APICallBack<PagedResourcesMessageResourceModel>() {
    public void onSuccess(HttpContext context, PagedResourcesMessageResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_responses_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageController.listResponsesUsingGETAsync") listResponsesUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> listResponses


```java
void listResponsesUsingGETAsync(
        final String xAuthToken,
        final Integer limit,
        final APICallBack<ResourcesMessageResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
messageController.listResponsesUsingGETAsync(xAuthToken, limit, new APICallBack<ResourcesMessageResourceModel>() {
    public void onSuccess(HttpContext context, ResourcesMessageResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_responses_page_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageController.listResponsesPageUsingGETAsync") listResponsesPageUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> listResponsesPage


```java
void listResponsesPageUsingGETAsync(
        final int page,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<PagedResourcesMessageResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
int page = 204;
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
messageController.listResponsesPageUsingGETAsync(page, xAuthToken, limit, new APICallBack<PagedResourcesMessageResourceModel>() {
    public void onSuccess(HttpContext context, PagedResourcesMessageResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_scheduled_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageController.listScheduledUsingGETAsync") listScheduledUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> listScheduled


```java
void listScheduledUsingGETAsync(
        final String xAuthToken,
        final Integer limit,
        final APICallBack<ResourcesMessageResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
messageController.listScheduledUsingGETAsync(xAuthToken, limit, new APICallBack<ResourcesMessageResourceModel>() {
    public void onSuccess(HttpContext context, ResourcesMessageResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_scheduled_page_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageController.listScheduledPageUsingGETAsync") listScheduledPageUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> listScheduledPage


```java
void listScheduledPageUsingGETAsync(
        final int page,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<PagedResourcesMessageResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
int page = 204;
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
messageController.listScheduledPageUsingGETAsync(page, xAuthToken, limit, new APICallBack<PagedResourcesMessageResourceModel>() {
    public void onSuccess(HttpContext context, PagedResourcesMessageResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="search_using_get3_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageController.searchUsingGET3Async") searchUsingGET3Async

> *Tags:*  ``` Skips Authentication ``` 

> search


```java
void searchUsingGET3Async(
        final String id,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String id = "id";
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
messageController.searchUsingGET3Async(id, xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_send_to_list_using_post1_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageController.createSendToListUsingPOST1Async") createSendToListUsingPOST1Async

> *Tags:*  ``` Skips Authentication ``` 

> sendToList


```java
void createSendToListUsingPOST1Async(
        final MessageInputMixedResourceModel resource,
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    MessageInputMixedResourceModel resource = new MessageInputMixedResourceModel();
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    messageController.createSendToListUsingPOST1Async(resource, xAuthToken, new APICallBack<DynamicResponse>() {
        public void onSuccess(HttpContext context, DynamicResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_send_to_contact_list_using_post_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageController.createSendToContactListUsingPOSTAsync") createSendToContactListUsingPOSTAsync

> *Tags:*  ``` Skips Authentication ``` 

> sendToContactList


```java
void createSendToContactListUsingPOSTAsync(
        final MessageInputContactResourceModel resource,
        final String xAuthToken,
        final APICallBack<Object> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    MessageInputContactResourceModel resource = new MessageInputContactResourceModel();
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    messageController.createSendToContactListUsingPOSTAsync(resource, xAuthToken, new APICallBack<void>() {
        public void onSuccess(HttpContext context, void response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_send_to_group_list_using_post_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageController.createSendToGroupListUsingPOSTAsync") createSendToGroupListUsingPOSTAsync

> *Tags:*  ``` Skips Authentication ``` 

> sendToGroupList


```java
void createSendToGroupListUsingPOSTAsync(
        final MessageInputGroupResourceModel resource,
        final String xAuthToken,
        final APICallBack<Object> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    MessageInputGroupResourceModel resource = new MessageInputGroupResourceModel();
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    messageController.createSendToGroupListUsingPOSTAsync(resource, xAuthToken, new APICallBack<void>() {
        public void onSuccess(HttpContext context, void response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_send_to_number_list_using_post_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageController.createSendToNumberListUsingPOSTAsync") createSendToNumberListUsingPOSTAsync

> *Tags:*  ``` Skips Authentication ``` 

> sendToNumberList


```java
void createSendToNumberListUsingPOSTAsync(
        final MessageInputResourceModel resource,
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    MessageInputResourceModel resource = new MessageInputResourceModel();
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    messageController.createSendToNumberListUsingPOSTAsync(resource, xAuthToken, new APICallBack<DynamicResponse>() {
        public void onSuccess(HttpContext context, DynamicResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete4_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageController.deleteUsingDELETE4Async") deleteUsingDELETE4Async

> *Tags:*  ``` Skips Authentication ``` 

> delete


```java
void deleteUsingDELETE4Async(
        final String messsageId,
        final String xAuthToken,
        final String id,
        final APICallBack<Object> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsageId |  ``` Required ```  | messsageId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| id |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
String messsageId = "messsageId";
String xAuthToken = "X-Auth-Token";
String id = "id";
// Invoking the API call with sample inputs
messageController.deleteUsingDELETE4Async(messsageId, xAuthToken, id, new APICallBack<void>() {
    public void onSuccess(HttpContext context, void response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



[Back to List of Controllers](#list_of_controllers)

## <a name="register_controler_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.smsmode.rest.controllers.RegisterControlerController") RegisterControlerController

### Get singleton instance

The singleton instance of the ``` RegisterControlerController ``` class can be accessed from the API Client.

```java
RegisterControlerController registerControler = client.getRegisterControler();
```

### <a name="create_register_using_post_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.RegisterControlerController.createRegisterUsingPOSTAsync") createRegisterUsingPOSTAsync

> *Tags:*  ``` Skips Authentication ``` 

> register


```java
void createRegisterUsingPOSTAsync(
        final RegisterResourceModel resource,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |


#### Example Usage

```java
try {
    RegisterResourceModel resource = new RegisterResourceModel();
    // Invoking the API call with sample inputs
    registerControler.createRegisterUsingPOSTAsync(resource, new APICallBack<DynamicResponse>() {
        public void onSuccess(HttpContext context, DynamicResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_refresh_using_post_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.RegisterControlerController.createRefreshUsingPOSTAsync") createRefreshUsingPOSTAsync

> *Tags:*  ``` Skips Authentication ``` 

> refresh


```java
void createRefreshUsingPOSTAsync(
        final SimpleEmailResourceModel resource,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |


#### Example Usage

```java
try {
    SimpleEmailResourceModel resource = new SimpleEmailResourceModel();
    // Invoking the API call with sample inputs
    registerControler.createRefreshUsingPOSTAsync(resource, new APICallBack<DynamicResponse>() {
        public void onSuccess(HttpContext context, DynamicResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_activate_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.RegisterControlerController.getActivateUsingGETAsync") getActivateUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> activate


```java
void getActivateUsingGETAsync(
        final String token,
        final int id,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| token |  ``` Required ```  | token |
| id |  ``` Required ```  | id |


#### Example Usage

```java
String token = "token";
int id = 204;
// Invoking the API call with sample inputs
registerControler.getActivateUsingGETAsync(token, id, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="credit_consumption_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.smsmode.rest.controllers.CreditConsumptionController") CreditConsumptionController

### Get singleton instance

The singleton instance of the ``` CreditConsumptionController ``` class can be accessed from the API Client.

```java
CreditConsumptionController creditConsumptionController = client.getCreditConsumptionController();
```

### <a name="list_using_get2_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.CreditConsumptionController.listUsingGET2Async") listUsingGET2Async

> *Tags:*  ``` Skips Authentication ``` 

> Get the consumption of the last months


```java
void listUsingGET2Async(
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
creditConsumptionController.listUsingGET2Async(xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get2_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.CreditConsumptionController.listPageUsingGET2Async") listPageUsingGET2Async

> *Tags:*  ``` Skips Authentication ``` 

> Get pageable consumption of the last months


```java
void listPageUsingGET2Async(
        final int page,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
int page = 204;
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
creditConsumptionController.listPageUsingGET2Async(page, xAuthToken, limit, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get1_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.CreditConsumptionController.getUsingGET1Async") getUsingGET1Async

> *Tags:*  ``` Skips Authentication ``` 

> Get specific consumption by id 


```java
void getUsingGET1Async(
        final int id,
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
int id = 204;
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
creditConsumptionController.getUsingGET1Async(id, xAuthToken, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="pricing_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.smsmode.rest.controllers.PricingController") PricingController

### Get singleton instance

The singleton instance of the ``` PricingController ``` class can be accessed from the API Client.

```java
PricingController pricingController = client.getPricingController();
```

### <a name="get_using_get7_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.PricingController.getUsingGET7Async") getUsingGET7Async

> *Tags:*  ``` Skips Authentication ``` 

> get


```java
void getUsingGET7Async(
        final String xAuthToken,
        final APICallBack<PricingResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
pricingController.getUsingGET7Async(xAuthToken, new APICallBack<PricingResourceModel>() {
    public void onSuccess(HttpContext context, PricingResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)

## <a name="message_model_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.smsmode.rest.controllers.MessageModelController") MessageModelController

### Get singleton instance

The singleton instance of the ``` MessageModelController ``` class can be accessed from the API Client.

```java
MessageModelController messageModelController = client.getMessageModelController();
```

### <a name="list_using_get7_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageModelController.listUsingGET7Async") listUsingGET7Async

> *Tags:*  ``` Skips Authentication ``` 

> list


```java
void listUsingGET7Async(
        final String xAuthToken,
        final Integer size,
        final APICallBack<ResourcesMessageModelResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| size |  ``` Optional ```  | size |


#### Example Usage

```java
String xAuthToken = "X-Auth-Token";
Integer size = 204;
// Invoking the API call with sample inputs
messageModelController.listUsingGET7Async(xAuthToken, size, new APICallBack<ResourcesMessageModelResourceModel>() {
    public void onSuccess(HttpContext context, ResourcesMessageModelResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="add_using_post3_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageModelController.addUsingPOST3Async") addUsingPOST3Async

> *Tags:*  ``` Skips Authentication ``` 

> add


```java
void addUsingPOST3Async(
        final MessageModelInputResourceModel resource,
        final String xAuthToken,
        final APICallBack<MessageModelResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    MessageModelInputResourceModel resource = new MessageModelInputResourceModel();
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    messageModelController.addUsingPOST3Async(resource, xAuthToken, new APICallBack<MessageModelResourceModel>() {
        public void onSuccess(HttpContext context, MessageModelResourceModel response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="create_delete_multiple_using_post_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageModelController.createDeleteMultipleUsingPOSTAsync") createDeleteMultipleUsingPOSTAsync

> *Tags:*  ``` Skips Authentication ``` 

> deleteMultiple


```java
void createDeleteMultipleUsingPOSTAsync(
        final List<String> ids,
        final String xAuthToken,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ids |  ``` Required ```  ``` Collection ```  | ids |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    List<String> ids = new LinkedList<String>(Arrays.asList("ids"));
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    messageModelController.createDeleteMultipleUsingPOSTAsync(ids, xAuthToken, new APICallBack<DynamicResponse>() {
        public void onSuccess(HttpContext context, DynamicResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="list_page_using_get7_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageModelController.listPageUsingGET7Async") listPageUsingGET7Async

> *Tags:*  ``` Skips Authentication ``` 

> listPage


```java
void listPageUsingGET7Async(
        final int page,
        final String xAuthToken,
        final Integer limit,
        final APICallBack<PagedResourcesMessageModelResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```java
int page = 204;
String xAuthToken = "X-Auth-Token";
Integer limit = 204;
// Invoking the API call with sample inputs
messageModelController.listPageUsingGET7Async(page, xAuthToken, limit, new APICallBack<PagedResourcesMessageModelResourceModel>() {
    public void onSuccess(HttpContext context, PagedResourcesMessageModelResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_using_get6_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageModelController.getUsingGET6Async") getUsingGET6Async

> *Tags:*  ``` Skips Authentication ``` 

> get


```java
void getUsingGET6Async(
        final String id,
        final String xAuthToken,
        final APICallBack<MessageModelResourceModel> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
String id = "id";
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
messageModelController.getUsingGET6Async(id, xAuthToken, new APICallBack<MessageModelResourceModel>() {
    public void onSuccess(HttpContext context, MessageModelResourceModel response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="update_using_put3_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageModelController.updateUsingPUT3Async") updateUsingPUT3Async

> *Tags:*  ``` Skips Authentication ``` 

> update


```java
void updateUsingPUT3Async(
        final String id,
        final MessageModelInputResourceModel resource,
        final String xAuthToken,
        final APICallBack<Object> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
try {
    String id = "id";
    MessageModelInputResourceModel resource = new MessageModelInputResourceModel();
    String xAuthToken = "X-Auth-Token";
    // Invoking the API call with sample inputs
    messageModelController.updateUsingPUT3Async(id, resource, xAuthToken, new APICallBack<void>() {
        public void onSuccess(HttpContext context, void response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="delete_using_delete5_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.MessageModelController.deleteUsingDELETE5Async") deleteUsingDELETE5Async

> *Tags:*  ``` Skips Authentication ``` 

> delete


```java
void deleteUsingDELETE5Async(
        final String id,
        final String xAuthToken,
        final APICallBack<Object> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```java
String id = "id";
String xAuthToken = "X-Auth-Token";
// Invoking the API call with sample inputs
messageModelController.deleteUsingDELETE5Async(id, xAuthToken, new APICallBack<void>() {
    public void onSuccess(HttpContext context, void response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



[Back to List of Controllers](#list_of_controllers)

## <a name="societe_info_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.smsmode.rest.controllers.SocieteInfoController") SocieteInfoController

### Get singleton instance

The singleton instance of the ``` SocieteInfoController ``` class can be accessed from the API Client.

```java
SocieteInfoController societeInfoController = client.getSocieteInfoController();
```

### <a name="create_research_company_using_post_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.SocieteInfoController.createResearchCompanyUsingPOSTAsync") createResearchCompanyUsingPOSTAsync

> *Tags:*  ``` Skips Authentication ``` 

> researchCompany


```java
void createResearchCompanyUsingPOSTAsync(
        final SocieteInfoResearchResourceModel research,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| research |  ``` Required ```  | research |


#### Example Usage

```java
try {
    SocieteInfoResearchResourceModel research = new SocieteInfoResearchResourceModel();
    // Invoking the API call with sample inputs
    societeInfoController.createResearchCompanyUsingPOSTAsync(research, new APICallBack<DynamicResponse>() {
        public void onSuccess(HttpContext context, DynamicResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



### <a name="get_details_using_get_async"></a>![Method: ](https://apidocs.io/img/method.png "com.smsmode.rest.controllers.SocieteInfoController.getDetailsUsingGETAsync") getDetailsUsingGETAsync

> *Tags:*  ``` Skips Authentication ``` 

> getDetails


```java
void getDetailsUsingGETAsync(
        final String id,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |


#### Example Usage

```java
String id = "id";
// Invoking the API call with sample inputs
societeInfoController.getDetailsUsingGETAsync(id, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)



