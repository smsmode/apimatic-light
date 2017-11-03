# Getting started

sMsMode API-REST Documentation

## How to Build

The generated SDK requires AngularJS framework to work. If you do not already have angular downloaded, please go ahead and do it from [here](https://angularjs.org/).
If any of your models have `Date` or `Datetime` type fields or your endpoints have `Date`/`Datetime` type response, you will need to download and link [angular-moment](https://cdnjs.cloudflare.com/ajax/libs/angular-moment/1.0.1/angular-moment.min.js) and [moment.js](https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.17.1/moment.min.js) with your project.

## How to Use

The following section describes how to use the generated SDK in an existing/new project.

### 1. Configure Angular and Generated SDK
Perform the following steps to configure angular and the SDK:
+ Make a `scripts` folder inside the root folder of the project. If you already have a `scripts` folder, skip to the next step.
+ Move the `angular.min.js` file inside the scripts folder. 
+ Move the `SMsmodeAPIRESTLib` folder inside the scripts folder.
+ If any of the Custom Types in your API have `Date`/`Datetime` type fields or any endpoint has `Date`/`Datetime` response, you will need to download angular-moment and moment.js. Move these 2 files into the `scripts` folder as well.

![folder-structure-image](https://apidocs.io/illustration/angularjs?step=folderStructure&workspaceFolder=sMsmode%20API-REST-Angular&projectName=SMsmodeAPIRESTLib)

### 2. Open Project Folder
Open an IDE/Text Editor for JavaScript like Sublime Text. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.  
Click on `File` and select `Open Folder`

Select the folder of your SDK and click on `Select Folder` to open it up in Sublime Text. The folder will become visible in the bar on the left.

![open-folder-image](https://apidocs.io/illustration/angularjs?step=openFolder&workspaceFolder=sMsmode%20API-REST-Angular)

### 3. Create an Angular Application
Since Angular JS is used for client-side web development, in order to use the generated library, you will have to develop an application first.
If you already have an angular application, [skip to Step 6](#6-include-sdk-references-in-html-file). Otherwise, follow these steps to create one:

+ In the IDE, click on `File` and choose `New File` to create a new file.
+ Add the following starting code in the file:
```js
var app = angular.module('myApp', []);
app.controller('testController', function($scope) 
{

});
```
+ Save it with the name `app.js` in the `scripts` folder.


### 4. Create HTML File
Skip to the next step if you are working with an existing project and already have an html file. Otherwise follow the steps to create one:
+ Inside the IDE, right click on the project folder name and select the `New File` option to create a new test file.
+ Save it with an appropriate name such as `index.html` in the root of your project folder.
`index.html` should look like this:
```html
<!DOCTYPE html>
<html>
<head>
	<title>Angular Project</title>
	<script></script>
</head>

<body>
</body>

</html>
```

![initial-html-code-image](https://apidocs.io/illustration/angularjs?step=initialCode&workspaceFolder=sMsmode%20API-REST-Angular)

### 5. Including links to Angular in HTML file
Your HTML file needs to have a link to `angular.min.js` file to use Angular-JS. Add the link using `script` tags inside the `head` section of `index.html` like:
```html
<script src="scripts/angular.min.js" ></script>
```
If any of the Custom Types that you have defined have `Date`/`Datetime` type fields or any endpoint has `Date`/`Datetime` response, you will also need to link to angular-moment and moment.js like:
```html
<script src="scripts/angular.min.js" ></script>
<script src="scripts/moment.min.js" ></script>
<script src="scripts/angular-moment.min.js" ></script>
```

### 6. Include SDK references in HTML file
Import the reference to the generated SDK files inside your html file like:
```html
<head>
    ...
    <!-- Helper files -->
    <script src="scripts/SMsmodeAPIRESTLib/Module.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Configuration.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/ModelFactory.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/ObjectMapper.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/APIHelper.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Http/Client/HttpContext.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Http/Client/RequestClient.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Http/Request/HttpRequest.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Http/Response/HttpResponse.js"></script>

    <!-- API Controllers -->
    <script src="scripts/SMsmodeAPIRESTLib/Controllers/BaseController.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Controllers/ReportController.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Controllers/InvoiceController.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Controllers/AuthenticationController.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Controllers/ContactController.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Controllers/CustomerController.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Controllers/GroupController.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Controllers/CampaignController.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Controllers/TransferController.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Controllers/EmailApiConfigurationController.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Controllers/MessageController.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Controllers/RegisterControlerController.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Controllers/CreditConsumptionController.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Controllers/PricingController.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Controllers/MessageModelController.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Controllers/SocieteInfoController.js"></script>


    <!-- Models -->
    <script src="scripts/SMsmodeAPIRESTLib/Models/BaseModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/PagedResourcesMessageResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/MessageResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/CustomerResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/ResourcesContactResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/MessageInputContactResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/SimpleEmailResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/EmailAPIConfigurationResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/MessageInputResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/DeferredResultResponseEntityObjectModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/ResourcesMessageModelResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/PricingResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/CreditPacksResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/MessageInputMixedResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/PagedResourcesMessageModelResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/ResourcesMessageResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/AddressResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/GroupResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/RegisterResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/MessageModelInputResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/MessageModelResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/ContactResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/PageMetadataModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/AuthenticationResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/SocieteInfoResearchResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/MessageInputGroupResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/LinkModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/TokenResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/TransferResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/InvoiceResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/CampaignInputResourceModel.js"></script>
    <script src="scripts/SMsmodeAPIRESTLib/Models/AccessChannelEnum.js"></script>

    ...
</head>
```
> The `Module.js` file should be imported before the other files. After `Module.js`, `Configuration.js` should be imported.
> The `ModelFactory.js` file is needed by `ObjectMapper.js` file. The `ObjectMapper` in turn, is needed by `BaseController.js`.

### 7. Including link to `app.js` in HTML file
Link your `app.js` file to your `index.html` file like:
```html
<head>
	...
	<script src="scripts/app.js"></script>
</head>
```
> The link to app.js needs to be included at the very end of the head tag, after the SDK references have been added

### 8. Initializing the Angular App
You need to initialize your app and the controller associated with your view inside your `index.html` file. Do so like:
+ Add ng-app directive to initialize your app inside the `body` tag.
```html
<body ng-app="myApp">
```
+ Add ng-controller directive to initialize your controller and bind it with your view (`index.html` file).
```html
...
<body ng-app="myApp">
	<div ng-controller="testController">
		...
	</div>
	...
</body>
...
```

### 9. Consuming the SDK 
In order to use the generated SDK's modules, controllers and factories, the project needs to be added as a dependency in your angular app's module. This will be done inside the `app.js` file.
Add the dependency like this:

```js
var app = angular.module('myApp', ['SMsmodeAPIRESTLib']);
```
At this point, the SDK has been successfully included in your project. Further steps include using a service/factory from the generated SDK. To see working example of this, please head on [over here](#list-of-controllers) and choose any class to see its functions and example usage.  

### 10. Running The App
To run the app, simply open up the `index.html` file in a browser.

![app-running](https://apidocs.io/illustration/angularjs?step=appRunning)

## Initialization


The Angular Application can be initialized as following:
```JavaScript
var app = angular.module('myApp', [SMsmodeAPIRESTLib]);
// now controllers/services can be created which import
// the factories provided by the sdk
```
### 




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

The singleton instance of the ``` ReportController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, ReportController){
	});
```

### <a name="list_using_get8"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.listUsingGET8") listUsingGET8

> *Tags:*  ``` Skips Authentication ``` 

> list


```javascript
function listUsingGET8(xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ReportController){
        var xAuthToken = 'X-Auth-Token';
        var limit = 168;


		var result = ReportController.listUsingGET8(xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function listPageUsingGET8(page, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ReportController){
        var page = 168;
        var xAuthToken = 'X-Auth-Token';
        var limit = 168;


		var result = ReportController.listPageUsingGET8(page, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getUsingGET8(messageRef, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ReportController){
        var messageRef = 'messageRef';
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = ReportController.getUsingGET8(messageRef, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getPageUsingGET(messageRef, page, xAuthToken, limit)
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


	app.controller("testController", function($scope, ReportController){
        var messageRef = 'messageRef';
        var page = 126;
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = ReportController.getPageUsingGET(messageRef, page, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function findUsingGET(messageRef, destinataire, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| destinataire |  ``` Required ```  | destinataire |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ReportController){
        var messageRef = 'messageRef';
        var destinataire = 'destinataire';
        var xAuthToken = 'X-Auth-Token';


		var result = ReportController.findUsingGET(messageRef, destinataire, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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

The singleton instance of the ``` InvoiceController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, InvoiceController, InvoiceResourceModel){
	});
```

### <a name="list_using_get5"></a>![Method: ](https://apidocs.io/img/method.png ".InvoiceController.listUsingGET5") listUsingGET5

> *Tags:*  ``` Skips Authentication ``` 

> View a list of invoices


```javascript
function listUsingGET5(xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, InvoiceController){
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = InvoiceController.listUsingGET5(xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function listPageUsingGET5(page, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, InvoiceController){
        var page = 126;
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = InvoiceController.listPageUsingGET5(page, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getPdfUsingGET(id, xAuthToken, base64)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| base64 |  ``` Required ```  | base64 |



#### Example Usage

```javascript


	app.controller("testController", function($scope, InvoiceController){
        var id = 126;
        var xAuthToken = 'X-Auth-Token';
        var base64 = false;


		var result = InvoiceController.getPdfUsingGET(id, xAuthToken, base64);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getUsingGET5(id, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, InvoiceController, InvoiceResourceModel){
        var id = 126;
        var xAuthToken = 'X-Auth-Token';


		var result = InvoiceController.getUsingGET5(id, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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

The singleton instance of the ``` AuthenticationController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, AuthenticationController, TokenResourceModel){
	});
```

### <a name="create_get_token_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".AuthenticationController.createGetTokenUsingPOST") createGetTokenUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> Generate the OAuth Token


```javascript
function createGetTokenUsingPOST(request)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| request |  ``` Required ```  | request |



#### Example Usage

```javascript


	app.controller("testController", function($scope, AuthenticationController, TokenResourceModel){
        var request = new AuthenticationResourceModel({"key":"value"});


		var result = AuthenticationController.createGetTokenUsingPOST(request);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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

The singleton instance of the ``` ContactController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, ContactController, ContactResourceModel, DeferredResultResponseEntityObjectModel, ResourcesContactResourceModel){
	});
```

### <a name="list_using_get1"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.listUsingGET1") listUsingGET1

> *Tags:*  ``` Skips Authentication ``` 

> View a list of contacts


```javascript
function listUsingGET1(xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactController){
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = ContactController.listUsingGET1(xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function addUsingPOST(resource, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactController, ContactResourceModel){
        var resource = new ContactResourceModel({"key":"value"});
        var xAuthToken = 'X-Auth-Token';


		var result = ContactController.addUsingPOST(resource, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function deleteBookUsingDELETE(xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactController){
        var xAuthToken = 'X-Auth-Token';


		var result = ContactController.deleteBookUsingDELETE(xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getCustomerInfoUsingGET(xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactController, ContactResourceModel){
        var xAuthToken = 'X-Auth-Token';


		var result = ContactController.getCustomerInfoUsingGET(xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function updateEditCustomerUsingPUT(xAuthToken, resource)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| resource |  ``` Required ```  | resource |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactController, ContactResourceModel){
        var xAuthToken = 'X-Auth-Token';
        var resource = new ContactResourceModel({"key":"value"});


		var result = ContactController.updateEditCustomerUsingPUT(xAuthToken, resource);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function createDeleteListUsingPOST(idList, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| idList |  ``` Required ```  ``` Collection ```  | idList |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactController){
        var idList = [126];
        var xAuthToken = 'X-Auth-Token';


		var result = ContactController.createDeleteListUsingPOST(idList, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function createExportContactsUsingPOST(fields, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fields |  ``` Required ```  ``` Collection ```  | fields |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactController, DeferredResultResponseEntityObjectModel){
        var fields = ['fields'];
        var xAuthToken = 'X-Auth-Token';


		var result = ContactController.createExportContactsUsingPOST(fields, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function uploadBlockingUsingPOST(file, model, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | file |
| model |  ``` Required ```  | model |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactController, $http, DeferredResultResponseEntityObjectModel){
        var file = "";
        var model = 'model';
        var xAuthToken = 'X-Auth-Token';


		$http.get(url).then(function(successData){
            file = successData;
            var result = ContactController.uploadBlockingUsingPOST(file, model, xAuthToken);
        //Function call returns a promise
            result.then(function(success){
    			//success case
    			//getting context of response
    			console.log(success.getContext());
    		},function(err){
    			//failure case
    		});
    
    	}, function(errorData){
    
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
function listPageUsingGET1(page, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactController, ResourcesContactResourceModel){
        var page = 126;
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = ContactController.listPageUsingGET1(page, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function searchUsingGET1(name, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactController){
        var name = 'name';
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = ContactController.searchUsingGET1(name, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getUsingGET(id, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactController, ContactResourceModel){
        var id = 126;
        var xAuthToken = 'X-Auth-Token';


		var result = ContactController.getUsingGET(id, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function updateUsingPUT(id, resource, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactController){
        var id = 126;
        var resource = new ContactResourceModel({"key":"value"});
        var xAuthToken = 'X-Auth-Token';


		var result = ContactController.updateUsingPUT(id, resource, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function deleteUsingDELETE1(id, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactController){
        var id = 126;
        var xAuthToken = 'X-Auth-Token';


		var result = ContactController.deleteUsingDELETE1(id, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function addGroupUsingPOST(id, groupId, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| groupId |  ``` Required ```  | groupId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactController){
        var id = 126;
        var groupId = 126;
        var xAuthToken = 'X-Auth-Token';


		var result = ContactController.addGroupUsingPOST(id, groupId, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getGroupsUsingGET(id, page, xAuthToken, limit)
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


	app.controller("testController", function($scope, ContactController){
        var id = 126;
        var page = 126;
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = ContactController.getGroupsUsingGET(id, page, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function deleteGroupUsingDELETE(id, groupId, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| groupId |  ``` Required ```  | groupId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, ContactController){
        var id = 126;
        var groupId = 126;
        var xAuthToken = 'X-Auth-Token';


		var result = ContactController.deleteGroupUsingDELETE(id, groupId, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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

The singleton instance of the ``` CustomerController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, CustomerController, CustomerResourceModel){
	});
```

### <a name="get_using_get2"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.getUsingGET2") getUsingGET2

> *Tags:*  ``` Skips Authentication ``` 

> Show your account


```javascript
function getUsingGET2(xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, CustomerController, CustomerResourceModel){
        var xAuthToken = 'X-Auth-Token';


		var result = CustomerController.getUsingGET2(xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getFromFieldsUsingGET(xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, CustomerController){
        var xAuthToken = 'X-Auth-Token';


		var result = CustomerController.getFromFieldsUsingGET(xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function updateDeleteSenderUsingPUT(xAuthToken, senderID)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| senderID |  ``` Required ```  | senderID |



#### Example Usage

```javascript


	app.controller("testController", function($scope, CustomerController){
        var xAuthToken = 'X-Auth-Token';
        var senderID = 'senderID';


		var result = CustomerController.updateDeleteSenderUsingPUT(xAuthToken, senderID);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function addSenderUsingPOST(xAuthToken, senderID)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| senderID |  ``` Required ```  | senderID |



#### Example Usage

```javascript


	app.controller("testController", function($scope, CustomerController){
        var xAuthToken = 'X-Auth-Token';
        var senderID = 'senderID';


		var result = CustomerController.addSenderUsingPOST(xAuthToken, senderID);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function listUsingGET3(xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, CustomerController){
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = CustomerController.listUsingGET3(xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function listPageUsingGET3(page, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, CustomerController){
        var page = 126;
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = CustomerController.listPageUsingGET3(page, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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

The singleton instance of the ``` GroupController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, GroupController, GroupResourceModel){
	});
```

### <a name="list_using_get4"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.listUsingGET4") listUsingGET4

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups


```javascript
function listUsingGET4(xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, GroupController){
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = GroupController.listUsingGET4(xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function addUsingPOST2(resource, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, GroupController, GroupResourceModel){
        var resource = new GroupResourceModel({"key":"value"});
        var xAuthToken = 'X-Auth-Token';


		var result = GroupController.addUsingPOST2(resource, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function createDeleteListUsingPOST1(idList, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| idList |  ``` Required ```  ``` Collection ```  | idList |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, GroupController){
        var idList = [126];
        var xAuthToken = 'X-Auth-Token';


		var result = GroupController.createDeleteListUsingPOST1(idList, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function listPageUsingGET4(page, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, GroupController){
        var page = 126;
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = GroupController.listPageUsingGET4(page, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function searchUsingGET2(name, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, GroupController){
        var name = 'name';
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = GroupController.searchUsingGET2(name, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getUsingGET4(id, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, GroupController, GroupResourceModel){
        var id = 126;
        var xAuthToken = 'X-Auth-Token';


		var result = GroupController.getUsingGET4(id, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function updateUsingPUT2(id, resource, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, GroupController){
        var id = 126;
        var resource = new GroupResourceModel({"key":"value"});
        var xAuthToken = 'X-Auth-Token';


		var result = GroupController.updateUsingPUT2(id, resource, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function deleteUsingDELETE3(id, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, GroupController){
        var id = 126;
        var xAuthToken = 'X-Auth-Token';


		var result = GroupController.deleteUsingDELETE3(id, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getContactsUsingGET(id, page, xAuthToken, limit)
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


	app.controller("testController", function($scope, GroupController, GroupResourceModel){
        var id = 126;
        var page = 126;
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = GroupController.getContactsUsingGET(id, page, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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

The singleton instance of the ``` CampaignController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, CampaignController){
	});
```

### <a name="list_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.listUsingGET") listUsingGET

> *Tags:*  ``` Skips Authentication ``` 

> list


```javascript
function listUsingGET(xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, CampaignController){
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = CampaignController.listUsingGET(xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function createSendToListUsingPOST(resource, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, CampaignController){
        var resource = new CampaignInputResourceModel({"key":"value"});
        var xAuthToken = 'X-Auth-Token';


		var result = CampaignController.createSendToListUsingPOST(resource, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function listPageUsingGET(page, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, CampaignController){
        var page = 126;
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = CampaignController.listPageUsingGET(page, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function searchUsingGET(name, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, CampaignController){
        var name = 'name';
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = CampaignController.searchUsingGET(name, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function deleteUsingDELETE(messsageId, xAuthToken, id)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsageId |  ``` Required ```  | messsageId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| id |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, CampaignController){
        var messsageId = 'messsageId';
        var xAuthToken = 'X-Auth-Token';
        var id = 'id';


		var result = CampaignController.deleteUsingDELETE(messsageId, xAuthToken, id);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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

The singleton instance of the ``` TransferController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, TransferController, TransferResourceModel){
	});
```

### <a name="list_using_get9"></a>![Method: ](https://apidocs.io/img/method.png ".TransferController.listUsingGET9") listUsingGET9

> *Tags:*  ``` Skips Authentication ``` 

> View a list of transferts


```javascript
function listUsingGET9(xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, TransferController){
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = TransferController.listUsingGET9(xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function listPageUsingGET9(page, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, TransferController){
        var page = 126;
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = TransferController.listPageUsingGET9(page, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getUsingGET9(id, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, TransferController, TransferResourceModel){
        var id = 126;
        var xAuthToken = 'X-Auth-Token';


		var result = TransferController.getUsingGET9(id, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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

The singleton instance of the ``` EmailApiConfigurationController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, EmailApiConfigurationController, EmailAPIConfigurationResourceModel){
	});
```

### <a name="get_using_get3"></a>![Method: ](https://apidocs.io/img/method.png ".EmailApiConfigurationController.getUsingGET3") getUsingGET3

> *Tags:*  ``` Skips Authentication ``` 

> Show your configuration


```javascript
function getUsingGET3(xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailApiConfigurationController, EmailAPIConfigurationResourceModel){
        var xAuthToken = 'X-Auth-Token';


		var result = EmailApiConfigurationController.getUsingGET3(xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function updateUsingPUT1(resource, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailApiConfigurationController){
        var resource = new EmailAPIConfigurationResourceModel({"key":"value"});
        var xAuthToken = 'X-Auth-Token';


		var result = EmailApiConfigurationController.updateUsingPUT1(resource, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function addUsingPOST1(resource, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailApiConfigurationController, EmailAPIConfigurationResourceModel){
        var resource = new EmailAPIConfigurationResourceModel({"key":"value"});
        var xAuthToken = 'X-Auth-Token';


		var result = EmailApiConfigurationController.addUsingPOST1(resource, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function deleteUsingDELETE2(xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, EmailApiConfigurationController){
        var xAuthToken = 'X-Auth-Token';


		var result = EmailApiConfigurationController.deleteUsingDELETE2(xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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

The singleton instance of the ``` MessageController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, MessageController, PagedResourcesMessageResourceModel, ResourcesMessageResourceModel){
	});
```

### <a name="list_using_get6"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.listUsingGET6") listUsingGET6

> *Tags:*  ``` Skips Authentication ``` 

> list


```javascript
function listUsingGET6(xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageController){
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = MessageController.listUsingGET6(xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function listPageUsingGET6(page, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageController, PagedResourcesMessageResourceModel){
        var page = 126;
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = MessageController.listPageUsingGET6(page, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function listResponsesUsingGET(xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageController, ResourcesMessageResourceModel){
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = MessageController.listResponsesUsingGET(xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function listResponsesPageUsingGET(page, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageController, PagedResourcesMessageResourceModel){
        var page = 126;
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = MessageController.listResponsesPageUsingGET(page, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function listScheduledUsingGET(xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageController, ResourcesMessageResourceModel){
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = MessageController.listScheduledUsingGET(xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function listScheduledPageUsingGET(page, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageController, PagedResourcesMessageResourceModel){
        var page = 126;
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = MessageController.listScheduledPageUsingGET(page, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function searchUsingGET3(id, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageController){
        var id = 'id';
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = MessageController.searchUsingGET3(id, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function createSendToListUsingPOST1(resource, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageController){
        var resource = new MessageInputMixedResourceModel({"key":"value"});
        var xAuthToken = 'X-Auth-Token';


		var result = MessageController.createSendToListUsingPOST1(resource, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function createSendToContactListUsingPOST(resource, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageController){
        var resource = new MessageInputContactResourceModel({"key":"value"});
        var xAuthToken = 'X-Auth-Token';


		var result = MessageController.createSendToContactListUsingPOST(resource, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function createSendToGroupListUsingPOST(resource, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageController){
        var resource = new MessageInputGroupResourceModel({"key":"value"});
        var xAuthToken = 'X-Auth-Token';


		var result = MessageController.createSendToGroupListUsingPOST(resource, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function createSendToNumberListUsingPOST(resource, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageController){
        var resource = new MessageInputResourceModel({"key":"value"});
        var xAuthToken = 'X-Auth-Token';


		var result = MessageController.createSendToNumberListUsingPOST(resource, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function deleteUsingDELETE4(messsageId, xAuthToken, id)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsageId |  ``` Required ```  | messsageId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| id |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageController){
        var messsageId = 'messsageId';
        var xAuthToken = 'X-Auth-Token';
        var id = 'id';


		var result = MessageController.deleteUsingDELETE4(messsageId, xAuthToken, id);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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

The singleton instance of the ``` RegisterControlerController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, RegisterControlerController){
	});
```

### <a name="create_register_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".RegisterControlerController.createRegisterUsingPOST") createRegisterUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> register


```javascript
function createRegisterUsingPOST(resource)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |



#### Example Usage

```javascript


	app.controller("testController", function($scope, RegisterControlerController){
        var resource = new RegisterResourceModel({"key":"value"});


		var result = RegisterControlerController.createRegisterUsingPOST(resource);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function createRefreshUsingPOST(resource)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |



#### Example Usage

```javascript


	app.controller("testController", function($scope, RegisterControlerController){
        var resource = new SimpleEmailResourceModel({"key":"value"});


		var result = RegisterControlerController.createRefreshUsingPOST(resource);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getActivateUsingGET(token, id)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| token |  ``` Required ```  | token |
| id |  ``` Required ```  | id |



#### Example Usage

```javascript


	app.controller("testController", function($scope, RegisterControlerController){
        var token = 'token';
        var id = 126;


		var result = RegisterControlerController.getActivateUsingGET(token, id);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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

The singleton instance of the ``` CreditConsumptionController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, CreditConsumptionController){
	});
```

### <a name="list_using_get2"></a>![Method: ](https://apidocs.io/img/method.png ".CreditConsumptionController.listUsingGET2") listUsingGET2

> *Tags:*  ``` Skips Authentication ``` 

> Get the consumption of the last months


```javascript
function listUsingGET2(xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, CreditConsumptionController){
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = CreditConsumptionController.listUsingGET2(xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function listPageUsingGET2(page, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, CreditConsumptionController){
        var page = 126;
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = CreditConsumptionController.listPageUsingGET2(page, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getUsingGET1(id, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, CreditConsumptionController){
        var id = 126;
        var xAuthToken = 'X-Auth-Token';


		var result = CreditConsumptionController.getUsingGET1(id, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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

The singleton instance of the ``` PricingController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, PricingController, PricingResourceModel){
	});
```

### <a name="get_using_get7"></a>![Method: ](https://apidocs.io/img/method.png ".PricingController.getUsingGET7") getUsingGET7

> *Tags:*  ``` Skips Authentication ``` 

> get


```javascript
function getUsingGET7(xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, PricingController, PricingResourceModel){
        var xAuthToken = 'X-Auth-Token';


		var result = PricingController.getUsingGET7(xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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

The singleton instance of the ``` MessageModelController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, MessageModelController, ResourcesMessageModelResourceModel, MessageModelResourceModel, PagedResourcesMessageModelResourceModel){
	});
```

### <a name="list_using_get7"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.listUsingGET7") listUsingGET7

> *Tags:*  ``` Skips Authentication ``` 

> list


```javascript
function listUsingGET7(xAuthToken, size)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| size |  ``` Optional ```  | size |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageModelController, ResourcesMessageModelResourceModel){
        var xAuthToken = 'X-Auth-Token';
        var size = 126;


		var result = MessageModelController.listUsingGET7(xAuthToken, size);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function addUsingPOST3(resource, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageModelController, MessageModelResourceModel){
        var resource = new MessageModelInputResourceModel({"key":"value"});
        var xAuthToken = 'X-Auth-Token';


		var result = MessageModelController.addUsingPOST3(resource, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function createDeleteMultipleUsingPOST(ids, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ids |  ``` Required ```  ``` Collection ```  | ids |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageModelController){
        var ids = ['ids'];
        var xAuthToken = 'X-Auth-Token';


		var result = MessageModelController.createDeleteMultipleUsingPOST(ids, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function listPageUsingGET7(page, xAuthToken, limit)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageModelController, PagedResourcesMessageModelResourceModel){
        var page = 126;
        var xAuthToken = 'X-Auth-Token';
        var limit = 126;


		var result = MessageModelController.listPageUsingGET7(page, xAuthToken, limit);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getUsingGET6(id, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageModelController, MessageModelResourceModel){
        var id = 'id';
        var xAuthToken = 'X-Auth-Token';


		var result = MessageModelController.getUsingGET6(id, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function updateUsingPUT3(id, resource, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageModelController){
        var id = 'id';
        var resource = new MessageModelInputResourceModel({"key":"value"});
        var xAuthToken = 'X-Auth-Token';


		var result = MessageModelController.updateUsingPUT3(id, resource, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function deleteUsingDELETE5(id, xAuthToken)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```javascript


	app.controller("testController", function($scope, MessageModelController){
        var id = 'id';
        var xAuthToken = 'X-Auth-Token';


		var result = MessageModelController.deleteUsingDELETE5(id, xAuthToken);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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

The singleton instance of the ``` SocieteInfoController ``` class can be accessed via Dependency Injection.

```js
	app.controller("testController", function($scope, SocieteInfoController){
	});
```

### <a name="create_research_company_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".SocieteInfoController.createResearchCompanyUsingPOST") createResearchCompanyUsingPOST

> *Tags:*  ``` Skips Authentication ``` 

> researchCompany


```javascript
function createResearchCompanyUsingPOST(research)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| research |  ``` Required ```  | research |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SocieteInfoController){
        var research = new SocieteInfoResearchResourceModel({"key":"value"});


		var result = SocieteInfoController.createResearchCompanyUsingPOST(research);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

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
function getDetailsUsingGET(id)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |



#### Example Usage

```javascript


	app.controller("testController", function($scope, SocieteInfoController){
        var id = 'id';


		var result = SocieteInfoController.getDetailsUsingGET(id);
        //Function call returns a promise
        result.then(function(success){
			//success case
			//getting context of response
			console.log(success.getContext());
		},function(err){
			//failure case
		});

	});
```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)



