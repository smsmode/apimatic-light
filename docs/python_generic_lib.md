# Getting started

sMsMode API-REST Documentation

## How to Build


You must have Python 2 >=2.7.9 or Python 3 >=3.4 installed on your system to install and run this SDK. This SDK package depends on other Python packages like nose, jsonpickle etc. 
These dependencies are defined in the ```requirements.txt``` file that comes with the SDK.
To resolve these dependencies, you can use the PIP Dependency manager. Install it by following steps at [https://pip.pypa.io/en/stable/installing/](https://pip.pypa.io/en/stable/installing/).

Python and PIP executables should be defined in your PATH. Open command prompt and type ```pip --version```.
This should display the version of the PIP Dependency Manager installed if your installation was successful and the paths are properly defined.

* Using command line, navigate to the directory containing the generated files (including ```requirements.txt```) for the SDK.
* Run the command ```pip install -r requirements.txt```. This should install all the required dependencies.

![Building SDK - Step 1](https://apidocs.io/illustration/python?step=installDependencies&workspaceFolder=sMsmode%20API-REST-Python)


## How to Use

The following section explains how to use the Smsmodeapirest SDK package in a new project.

### 1. Open Project in an IDE

Open up a Python IDE like PyCharm. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.

![Open project in PyCharm - Step 1](https://apidocs.io/illustration/python?step=pyCharm)

Click on ```Open``` in PyCharm to browse to your generated SDK directory and then click ```OK```.

![Open project in PyCharm - Step 2](https://apidocs.io/illustration/python?step=openProject0&workspaceFolder=sMsmode%20API-REST-Python)     

The project files will be displayed in the side bar as follows:

![Open project in PyCharm - Step 3](https://apidocs.io/illustration/python?step=openProject1&workspaceFolder=sMsmode%20API-REST-Python&projectName=smsmodeapirest)     

### 2. Add a new Test Project

Create a new directory by right clicking on the solution name as shown below:

![Add a new project in PyCharm - Step 1](https://apidocs.io/illustration/python?step=createDirectory&workspaceFolder=sMsmode%20API-REST-Python&projectName=smsmodeapirest)

Name the directory as "test"

![Add a new project in PyCharm - Step 2](https://apidocs.io/illustration/python?step=nameDirectory)
   
Add a python file to this project with the name "testsdk"

![Add a new project in PyCharm - Step 3](https://apidocs.io/illustration/python?step=createFile&workspaceFolder=sMsmode%20API-REST-Python&projectName=smsmodeapirest)

Name it "testsdk"

![Add a new project in PyCharm - Step 4](https://apidocs.io/illustration/python?step=nameFile)

In your python file you will be required to import the generated python library using the following code lines

```Python
from smsmodeapirest.smsmodeapirest_client import SmsmodeapirestClient
```

![Add a new project in PyCharm - Step 4](https://apidocs.io/illustration/python?step=projectFiles&workspaceFolder=sMsmode%20API-REST-Python&libraryName=smsmodeapirest.smsmodeapirest_client&projectName=smsmodeapirest)

After this you can write code to instantiate an API client object, get a controller object and  make API calls. Sample code is given in the subsequent sections.

### 3. Run the Test Project

To run the file within your test project, right click on your Python file inside your Test project and click on ```Run```

![Run Test Project - Step 1](https://apidocs.io/illustration/python?step=runProject&workspaceFolder=sMsmode%20API-REST-Python&libraryName=smsmodeapirest.smsmodeapirest_client&projectName=smsmodeapirest)


## How to Test

You can test the generated SDK and the server with automatically generated test
cases. unittest is used as the testing framework and nose is used as the test
runner. You can run the tests as follows:

  1. From terminal/cmd navigate to the root directory of the SDK.
  2. Invoke 'pip install -r test-requirements.txt'
  3. Invoke 'nosetests'

## Initialization

### 

API client can be initialized as following.

```python

client = SmsmodeapirestClient()
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

### Get controller instance

An instance of the ``` ReportController ``` class can be accessed from the API Client.

```python
 report_controller_client = client.report_controller
```

### <a name="list_using_get_8"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.list_using_get_8") list_using_get_8

> *Tags:*  ``` Skips Authentication ``` 

> list

```python
def list_using_get_8(self,
                         x_auth_token,
                         limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'
limit = 3

result = report_controller_client.list_using_get_8(x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get_8"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.list_page_using_get_8") list_page_using_get_8

> *Tags:*  ``` Skips Authentication ``` 

> listPage

```python
def list_page_using_get_8(self,
                              page,
                              x_auth_token,
                              limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
page = 3
x_auth_token = 'X-Auth-Token'
limit = 3

result = report_controller_client.list_page_using_get_8(page, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_using_get_8"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.get_using_get_8") get_using_get_8

> *Tags:*  ``` Skips Authentication ``` 

> get

```python
def get_using_get_8(self,
                        message_ref,
                        x_auth_token,
                        limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
message_ref = 'messageRef'
x_auth_token = 'X-Auth-Token'
limit = 3

result = report_controller_client.get_using_get_8(message_ref, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_page_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.get_page_using_get") get_page_using_get

> *Tags:*  ``` Skips Authentication ``` 

> getPage

```python
def get_page_using_get(self,
                           message_ref,
                           page,
                           x_auth_token,
                           limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
message_ref = 'messageRef'
page = 3
x_auth_token = 'X-Auth-Token'
limit = 3

result = report_controller_client.get_page_using_get(message_ref, page, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="find_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.find_using_get") find_using_get

> *Tags:*  ``` Skips Authentication ``` 

> find

```python
def find_using_get(self,
                       message_ref,
                       destinataire,
                       x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messageRef |  ``` Required ```  | messageRef |
| destinataire |  ``` Required ```  | destinataire |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
message_ref = 'messageRef'
destinataire = 'destinataire'
x_auth_token = 'X-Auth-Token'

result = report_controller_client.find_using_get(message_ref, destinataire, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="invoice_controller"></a>![Class: ](https://apidocs.io/img/class.png ".InvoiceController") InvoiceController

### Get controller instance

An instance of the ``` InvoiceController ``` class can be accessed from the API Client.

```python
 invoice_controller_client = client.invoice_controller
```

### <a name="list_using_get_5"></a>![Method: ](https://apidocs.io/img/method.png ".InvoiceController.list_using_get_5") list_using_get_5

> *Tags:*  ``` Skips Authentication ``` 

> View a list of invoices

```python
def list_using_get_5(self,
                         x_auth_token,
                         limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'
limit = 3

result = invoice_controller_client.list_using_get_5(x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get_5"></a>![Method: ](https://apidocs.io/img/method.png ".InvoiceController.list_page_using_get_5") list_page_using_get_5

> *Tags:*  ``` Skips Authentication ``` 

> listPage

```python
def list_page_using_get_5(self,
                              page,
                              x_auth_token,
                              limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
page = 3
x_auth_token = 'X-Auth-Token'
limit = 3

result = invoice_controller_client.list_page_using_get_5(page, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_pdf_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".InvoiceController.get_pdf_using_get") get_pdf_using_get

> *Tags:*  ``` Skips Authentication ``` 

> Generate an invoice in a pdf file

```python
def get_pdf_using_get(self,
                          id,
                          x_auth_token,
                          base_64)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| base64 |  ``` Required ```  | base64 |



#### Example Usage

```python
id = 3
x_auth_token = 'X-Auth-Token'
base64 = False

result = invoice_controller_client.get_pdf_using_get(id, x_auth_token, base64)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_using_get_5"></a>![Method: ](https://apidocs.io/img/method.png ".InvoiceController.get_using_get_5") get_using_get_5

> *Tags:*  ``` Skips Authentication ``` 

> Show an invoice

```python
def get_using_get_5(self,
                        id,
                        x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
id = 3
x_auth_token = 'X-Auth-Token'

result = invoice_controller_client.get_using_get_5(id, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="authentication_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AuthenticationController") AuthenticationController

### Get controller instance

An instance of the ``` AuthenticationController ``` class can be accessed from the API Client.

```python
 authentication_controller_client = client.authentication_controller
```

### <a name="create_get_token_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".AuthenticationController.create_get_token_using_post") create_get_token_using_post

> *Tags:*  ``` Skips Authentication ``` 

> Generate the OAuth Token

```python
def create_get_token_using_post(self,
                                    request)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| request |  ``` Required ```  | request |



#### Example Usage

```python
request = AuthenticationResourceModel()

result = authentication_controller_client.create_get_token_using_post(request)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="contact_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ContactController") ContactController

### Get controller instance

An instance of the ``` ContactController ``` class can be accessed from the API Client.

```python
 contact_controller_client = client.contact_controller
```

### <a name="list_using_get_1"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.list_using_get_1") list_using_get_1

> *Tags:*  ``` Skips Authentication ``` 

> View a list of contacts

```python
def list_using_get_1(self,
                         x_auth_token,
                         limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'
limit = 3

result = contact_controller_client.list_using_get_1(x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="add_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.add_using_post") add_using_post

> *Tags:*  ``` Skips Authentication ``` 

> Add a contact

```python
def add_using_post(self,
                       resource,
                       x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
resource = ContactResourceModel()
x_auth_token = 'X-Auth-Token'

result = contact_controller_client.add_using_post(resource, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="delete_book_using_delete"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.delete_book_using_delete") delete_book_using_delete

> *Tags:*  ``` Skips Authentication ``` 

> Remove all contacts and groups of the account

```python
def delete_book_using_delete(self,
                                 x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'

result = contact_controller_client.delete_book_using_delete(x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |




### <a name="get_customer_info_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.get_customer_info_using_get") get_customer_info_using_get

> *Tags:*  ``` Skips Authentication ``` 

> Show contact info of customer

```python
def get_customer_info_using_get(self,
                                    x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'

result = contact_controller_client.get_customer_info_using_get(x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="update_edit_customer_using_put"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.update_edit_customer_using_put") update_edit_customer_using_put

> *Tags:*  ``` Skips Authentication ``` 

> Edit contact info of customer

```python
def update_edit_customer_using_put(self,
                                       x_auth_token,
                                       resource)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| resource |  ``` Required ```  | resource |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'
resource = ContactResourceModel()

result = contact_controller_client.update_edit_customer_using_put(x_auth_token, resource)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_delete_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.create_delete_list_using_post") create_delete_list_using_post

> *Tags:*  ``` Skips Authentication ``` 

> Delete a list of contacts

```python
def create_delete_list_using_post(self,
                                      id_list,
                                      x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| idList |  ``` Required ```  ``` Collection ```  | idList |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
id_list = [3]
x_auth_token = 'X-Auth-Token'

result = contact_controller_client.create_delete_list_using_post(id_list, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_export_contacts_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.create_export_contacts_using_post") create_export_contacts_using_post

> *Tags:*  ``` Skips Authentication ``` 

> Export contacts in csv format

```python
def create_export_contacts_using_post(self,
                                          fields,
                                          x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fields |  ``` Required ```  ``` Collection ```  | fields |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
fields = ['fields']
x_auth_token = 'X-Auth-Token'

result = contact_controller_client.create_export_contacts_using_post(fields, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="upload_blocking_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.upload_blocking_using_post") upload_blocking_using_post

> *Tags:*  ``` Skips Authentication ``` 

> Import contacts via xls or csv files

```python
def upload_blocking_using_post(self,
                                   file,
                                   model,
                                   x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | file |
| model |  ``` Required ```  | model |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
file = open("pathtofile", 'rb')
model = 'model'
x_auth_token = 'X-Auth-Token'

result = contact_controller_client.upload_blocking_using_post(file, model, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get_1"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.list_page_using_get_1") list_page_using_get_1

> *Tags:*  ``` Skips Authentication ``` 

> listPage

```python
def list_page_using_get_1(self,
                              page,
                              x_auth_token,
                              limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
page = 3
x_auth_token = 'X-Auth-Token'
limit = 3

result = contact_controller_client.list_page_using_get_1(page, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="search_using_get_1"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.search_using_get_1") search_using_get_1

> *Tags:*  ``` Skips Authentication ``` 

> search

```python
def search_using_get_1(self,
                           name,
                           x_auth_token,
                           limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
name = 'name'
x_auth_token = 'X-Auth-Token'
limit = 3

result = contact_controller_client.search_using_get_1(name, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.get_using_get") get_using_get

> *Tags:*  ``` Skips Authentication ``` 

> Show a contact

```python
def get_using_get(self,
                      id,
                      x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
id = 3
x_auth_token = 'X-Auth-Token'

result = contact_controller_client.get_using_get(id, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="update_using_put"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.update_using_put") update_using_put

> *Tags:*  ``` Skips Authentication ``` 

> Update a contact

```python
def update_using_put(self,
                         id,
                         resource,
                         x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
id = 3
resource = ContactResourceModel()
x_auth_token = 'X-Auth-Token'

result = contact_controller_client.update_using_put(id, resource, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="delete_using_delete_1"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.delete_using_delete_1") delete_using_delete_1

> *Tags:*  ``` Skips Authentication ``` 

> Delete a contact

```python
def delete_using_delete_1(self,
                              id,
                              x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
id = 217
x_auth_token = 'X-Auth-Token'

result = contact_controller_client.delete_using_delete_1(id, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |




### <a name="add_group_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.add_group_using_post") add_group_using_post

> *Tags:*  ``` Skips Authentication ``` 

> Add a contact in a group

```python
def add_group_using_post(self,
                             id,
                             group_id,
                             x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| groupId |  ``` Required ```  | groupId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
id = 217
group_id = 217
x_auth_token = 'X-Auth-Token'

result = contact_controller_client.add_group_using_post(id, group_id, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_groups_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.get_groups_using_get") get_groups_using_get

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups for a contact

```python
def get_groups_using_get(self,
                             id,
                             page,
                             x_auth_token,
                             limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
id = 217
page = 217
x_auth_token = 'X-Auth-Token'
limit = 217

result = contact_controller_client.get_groups_using_get(id, page, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="delete_group_using_delete"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.delete_group_using_delete") delete_group_using_delete

> *Tags:*  ``` Skips Authentication ``` 

> Remove a contact from a group

```python
def delete_group_using_delete(self,
                                  id,
                                  group_id,
                                  x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| groupId |  ``` Required ```  | groupId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
id = 217
group_id = 217
x_auth_token = 'X-Auth-Token'

result = contact_controller_client.delete_group_using_delete(id, group_id, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |




[Back to List of Controllers](#list_of_controllers)

## <a name="customer_controller"></a>![Class: ](https://apidocs.io/img/class.png ".CustomerController") CustomerController

### Get controller instance

An instance of the ``` CustomerController ``` class can be accessed from the API Client.

```python
 customer_controller_client = client.customer_controller
```

### <a name="get_using_get_2"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.get_using_get_2") get_using_get_2

> *Tags:*  ``` Skips Authentication ``` 

> Show your account

```python
def get_using_get_2(self,
                        x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'

result = customer_controller_client.get_using_get_2(x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_from_fields_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.get_from_fields_using_get") get_from_fields_using_get

> *Tags:*  ``` Skips Authentication ``` 

> Get your personnalized sender IDs

```python
def get_from_fields_using_get(self,
                                  x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'

result = customer_controller_client.get_from_fields_using_get(x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="update_delete_sender_using_put"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.update_delete_sender_using_put") update_delete_sender_using_put

> *Tags:*  ``` Skips Authentication ``` 

> Remove sender ID

```python
def update_delete_sender_using_put(self,
                                       x_auth_token,
                                       sender_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| senderID |  ``` Required ```  | senderID |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'
sender_id = 'senderID'

result = customer_controller_client.update_delete_sender_using_put(x_auth_token, sender_id)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="add_sender_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.add_sender_using_post") add_sender_using_post

> *Tags:*  ``` Skips Authentication ``` 

> Add personnalized sender ID

```python
def add_sender_using_post(self,
                              x_auth_token,
                              sender_id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| senderID |  ``` Required ```  | senderID |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'
sender_id = 'senderID'

result = customer_controller_client.add_sender_using_post(x_auth_token, sender_id)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_using_get_3"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.list_using_get_3") list_using_get_3

> *Tags:*  ``` Skips Authentication ``` 

> View a list of your subaccounts

```python
def list_using_get_3(self,
                         x_auth_token,
                         limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'
limit = 217

result = customer_controller_client.list_using_get_3(x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get_3"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.list_page_using_get_3") list_page_using_get_3

> *Tags:*  ``` Skips Authentication ``` 

> View a list of your subaccounts by page

```python
def list_page_using_get_3(self,
                              page,
                              x_auth_token,
                              limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
page = 217
x_auth_token = 'X-Auth-Token'
limit = 217

result = customer_controller_client.list_page_using_get_3(page, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="group_controller"></a>![Class: ](https://apidocs.io/img/class.png ".GroupController") GroupController

### Get controller instance

An instance of the ``` GroupController ``` class can be accessed from the API Client.

```python
 group_controller_client = client.group_controller
```

### <a name="list_using_get_4"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.list_using_get_4") list_using_get_4

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups

```python
def list_using_get_4(self,
                         x_auth_token,
                         limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'
limit = 217

result = group_controller_client.list_using_get_4(x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="add_using_post_2"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.add_using_post_2") add_using_post_2

> *Tags:*  ``` Skips Authentication ``` 

> Add a group

```python
def add_using_post_2(self,
                         resource,
                         x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
resource = GroupResourceModel()
x_auth_token = 'X-Auth-Token'

result = group_controller_client.add_using_post_2(resource, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_delete_list_using_post_1"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.create_delete_list_using_post_1") create_delete_list_using_post_1

> *Tags:*  ``` Skips Authentication ``` 

> Delete a list of groups

```python
def create_delete_list_using_post_1(self,
                                        id_list,
                                        x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| idList |  ``` Required ```  ``` Collection ```  | idList |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
id_list = [217]
x_auth_token = 'X-Auth-Token'

result = group_controller_client.create_delete_list_using_post_1(id_list, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get_4"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.list_page_using_get_4") list_page_using_get_4

> *Tags:*  ``` Skips Authentication ``` 

> listPage

```python
def list_page_using_get_4(self,
                              page,
                              x_auth_token,
                              limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
page = 217
x_auth_token = 'X-Auth-Token'
limit = 217

result = group_controller_client.list_page_using_get_4(page, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="search_using_get_2"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.search_using_get_2") search_using_get_2

> *Tags:*  ``` Skips Authentication ``` 

> search

```python
def search_using_get_2(self,
                           name,
                           x_auth_token,
                           limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
name = 'name'
x_auth_token = 'X-Auth-Token'
limit = 217

result = group_controller_client.search_using_get_2(name, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_using_get_4"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.get_using_get_4") get_using_get_4

> *Tags:*  ``` Skips Authentication ``` 

> Show a group

```python
def get_using_get_4(self,
                        id,
                        x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
id = 217
x_auth_token = 'X-Auth-Token'

result = group_controller_client.get_using_get_4(id, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="update_using_put_2"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.update_using_put_2") update_using_put_2

> *Tags:*  ``` Skips Authentication ``` 

> Update a group

```python
def update_using_put_2(self,
                           id,
                           resource,
                           x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
id = 217
resource = GroupResourceModel()
x_auth_token = 'X-Auth-Token'

result = group_controller_client.update_using_put_2(id, resource, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="delete_using_delete_3"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.delete_using_delete_3") delete_using_delete_3

> *Tags:*  ``` Skips Authentication ``` 

> Delete a group

```python
def delete_using_delete_3(self,
                              id,
                              x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
id = 217
x_auth_token = 'X-Auth-Token'

result = group_controller_client.delete_using_delete_3(id, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |




### <a name="get_contacts_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.get_contacts_using_get") get_contacts_using_get

> *Tags:*  ``` Skips Authentication ``` 

> Show a list of contacts for a group

```python
def get_contacts_using_get(self,
                               id,
                               page,
                               x_auth_token,
                               limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
id = 217
page = 217
x_auth_token = 'X-Auth-Token'
limit = 217

result = group_controller_client.get_contacts_using_get(id, page, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="campaign_controller"></a>![Class: ](https://apidocs.io/img/class.png ".CampaignController") CampaignController

### Get controller instance

An instance of the ``` CampaignController ``` class can be accessed from the API Client.

```python
 campaign_controller_client = client.campaign_controller
```

### <a name="list_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.list_using_get") list_using_get

> *Tags:*  ``` Skips Authentication ``` 

> list

```python
def list_using_get(self,
                       x_auth_token,
                       limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'
limit = 217

result = campaign_controller_client.list_using_get(x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_send_to_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.create_send_to_list_using_post") create_send_to_list_using_post

> *Tags:*  ``` Skips Authentication ``` 

> sendToList

```python
def create_send_to_list_using_post(self,
                                       resource,
                                       x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
resource = CampaignInputResourceModel()
x_auth_token = 'X-Auth-Token'

result = campaign_controller_client.create_send_to_list_using_post(resource, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.list_page_using_get") list_page_using_get

> *Tags:*  ``` Skips Authentication ``` 

> listPage

```python
def list_page_using_get(self,
                            page,
                            x_auth_token,
                            limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
page = 217
x_auth_token = 'X-Auth-Token'
limit = 217

result = campaign_controller_client.list_page_using_get(page, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="search_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.search_using_get") search_using_get

> *Tags:*  ``` Skips Authentication ``` 

> search

```python
def search_using_get(self,
                         name,
                         x_auth_token,
                         limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
name = 'name'
x_auth_token = 'X-Auth-Token'
limit = 217

result = campaign_controller_client.search_using_get(name, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="delete_using_delete"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.delete_using_delete") delete_using_delete

> *Tags:*  ``` Skips Authentication ``` 

> delete

```python
def delete_using_delete(self,
                            messsage_id,
                            x_auth_token,
                            id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsageId |  ``` Required ```  | messsageId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| id |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
messsage_id = 'messsageId'
x_auth_token = 'X-Auth-Token'
id = 'id'

result = campaign_controller_client.delete_using_delete(messsage_id, x_auth_token, id)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |




[Back to List of Controllers](#list_of_controllers)

## <a name="transfer_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TransferController") TransferController

### Get controller instance

An instance of the ``` TransferController ``` class can be accessed from the API Client.

```python
 transfer_controller_client = client.transfer_controller
```

### <a name="list_using_get_9"></a>![Method: ](https://apidocs.io/img/method.png ".TransferController.list_using_get_9") list_using_get_9

> *Tags:*  ``` Skips Authentication ``` 

> View a list of transferts

```python
def list_using_get_9(self,
                         x_auth_token,
                         limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'
limit = 217

result = transfer_controller_client.list_using_get_9(x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get_9"></a>![Method: ](https://apidocs.io/img/method.png ".TransferController.list_page_using_get_9") list_page_using_get_9

> *Tags:*  ``` Skips Authentication ``` 

> listPage

```python
def list_page_using_get_9(self,
                              page,
                              x_auth_token,
                              limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
page = 217
x_auth_token = 'X-Auth-Token'
limit = 217

result = transfer_controller_client.list_page_using_get_9(page, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_using_get_9"></a>![Method: ](https://apidocs.io/img/method.png ".TransferController.get_using_get_9") get_using_get_9

> *Tags:*  ``` Skips Authentication ``` 

> Show a transfet

```python
def get_using_get_9(self,
                        id,
                        x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
id = 217
x_auth_token = 'X-Auth-Token'

result = transfer_controller_client.get_using_get_9(id, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="email_api_configuration_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EmailApiConfigurationController") EmailApiConfigurationController

### Get controller instance

An instance of the ``` EmailApiConfigurationController ``` class can be accessed from the API Client.

```python
 email_api_configuration_controller_client = client.email_api_configuration_controller
```

### <a name="get_using_get_3"></a>![Method: ](https://apidocs.io/img/method.png ".EmailApiConfigurationController.get_using_get_3") get_using_get_3

> *Tags:*  ``` Skips Authentication ``` 

> Show your configuration

```python
def get_using_get_3(self,
                        x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'

result = email_api_configuration_controller_client.get_using_get_3(x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="update_using_put_1"></a>![Method: ](https://apidocs.io/img/method.png ".EmailApiConfigurationController.update_using_put_1") update_using_put_1

> *Tags:*  ``` Skips Authentication ``` 

> Update your configuration

```python
def update_using_put_1(self,
                           resource,
                           x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
resource = EmailAPIConfigurationResourceModel()
x_auth_token = 'X-Auth-Token'

result = email_api_configuration_controller_client.update_using_put_1(resource, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="add_using_post_1"></a>![Method: ](https://apidocs.io/img/method.png ".EmailApiConfigurationController.add_using_post_1") add_using_post_1

> *Tags:*  ``` Skips Authentication ``` 

> Create your configuration

```python
def add_using_post_1(self,
                         resource,
                         x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
resource = EmailAPIConfigurationResourceModel()
x_auth_token = 'X-Auth-Token'

result = email_api_configuration_controller_client.add_using_post_1(resource, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="delete_using_delete_2"></a>![Method: ](https://apidocs.io/img/method.png ".EmailApiConfigurationController.delete_using_delete_2") delete_using_delete_2

> *Tags:*  ``` Skips Authentication ``` 

> Delete your configuration

```python
def delete_using_delete_2(self,
                              x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'

result = email_api_configuration_controller_client.delete_using_delete_2(x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |




[Back to List of Controllers](#list_of_controllers)

## <a name="message_controller"></a>![Class: ](https://apidocs.io/img/class.png ".MessageController") MessageController

### Get controller instance

An instance of the ``` MessageController ``` class can be accessed from the API Client.

```python
 message_controller_client = client.message_controller
```

### <a name="list_using_get_6"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.list_using_get_6") list_using_get_6

> *Tags:*  ``` Skips Authentication ``` 

> list

```python
def list_using_get_6(self,
                         x_auth_token,
                         limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'
limit = 53

result = message_controller_client.list_using_get_6(x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get_6"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.list_page_using_get_6") list_page_using_get_6

> *Tags:*  ``` Skips Authentication ``` 

> listPage

```python
def list_page_using_get_6(self,
                              page,
                              x_auth_token,
                              limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
page = 53
x_auth_token = 'X-Auth-Token'
limit = 53

result = message_controller_client.list_page_using_get_6(page, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_responses_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.list_responses_using_get") list_responses_using_get

> *Tags:*  ``` Skips Authentication ``` 

> listResponses

```python
def list_responses_using_get(self,
                                 x_auth_token,
                                 limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'
limit = 53

result = message_controller_client.list_responses_using_get(x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_responses_page_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.list_responses_page_using_get") list_responses_page_using_get

> *Tags:*  ``` Skips Authentication ``` 

> listResponsesPage

```python
def list_responses_page_using_get(self,
                                      page,
                                      x_auth_token,
                                      limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
page = 53
x_auth_token = 'X-Auth-Token'
limit = 53

result = message_controller_client.list_responses_page_using_get(page, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_scheduled_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.list_scheduled_using_get") list_scheduled_using_get

> *Tags:*  ``` Skips Authentication ``` 

> listScheduled

```python
def list_scheduled_using_get(self,
                                 x_auth_token,
                                 limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'
limit = 53

result = message_controller_client.list_scheduled_using_get(x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_scheduled_page_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.list_scheduled_page_using_get") list_scheduled_page_using_get

> *Tags:*  ``` Skips Authentication ``` 

> listScheduledPage

```python
def list_scheduled_page_using_get(self,
                                      page,
                                      x_auth_token,
                                      limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
page = 53
x_auth_token = 'X-Auth-Token'
limit = 53

result = message_controller_client.list_scheduled_page_using_get(page, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="search_using_get_3"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.search_using_get_3") search_using_get_3

> *Tags:*  ``` Skips Authentication ``` 

> search

```python
def search_using_get_3(self,
                           id,
                           x_auth_token,
                           limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
id = 'id'
x_auth_token = 'X-Auth-Token'
limit = 53

result = message_controller_client.search_using_get_3(id, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_send_to_list_using_post_1"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.create_send_to_list_using_post_1") create_send_to_list_using_post_1

> *Tags:*  ``` Skips Authentication ``` 

> sendToList

```python
def create_send_to_list_using_post_1(self,
                                         resource,
                                         x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
resource = MessageInputMixedResourceModel()
x_auth_token = 'X-Auth-Token'

result = message_controller_client.create_send_to_list_using_post_1(resource, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_send_to_contact_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.create_send_to_contact_list_using_post") create_send_to_contact_list_using_post

> *Tags:*  ``` Skips Authentication ``` 

> sendToContactList

```python
def create_send_to_contact_list_using_post(self,
                                               resource,
                                               x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
resource = MessageInputContactResourceModel()
x_auth_token = 'X-Auth-Token'

message_controller_client.create_send_to_contact_list_using_post(resource, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_send_to_group_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.create_send_to_group_list_using_post") create_send_to_group_list_using_post

> *Tags:*  ``` Skips Authentication ``` 

> sendToGroupList

```python
def create_send_to_group_list_using_post(self,
                                             resource,
                                             x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
resource = MessageInputGroupResourceModel()
x_auth_token = 'X-Auth-Token'

message_controller_client.create_send_to_group_list_using_post(resource, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_send_to_number_list_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.create_send_to_number_list_using_post") create_send_to_number_list_using_post

> *Tags:*  ``` Skips Authentication ``` 

> sendToNumberList

```python
def create_send_to_number_list_using_post(self,
                                              resource,
                                              x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
resource = MessageInputResourceModel()
x_auth_token = 'X-Auth-Token'

result = message_controller_client.create_send_to_number_list_using_post(resource, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="delete_using_delete_4"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.delete_using_delete_4") delete_using_delete_4

> *Tags:*  ``` Skips Authentication ``` 

> delete

```python
def delete_using_delete_4(self,
                              messsage_id,
                              x_auth_token,
                              id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsageId |  ``` Required ```  | messsageId |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| id |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
messsage_id = 'messsageId'
x_auth_token = 'X-Auth-Token'
id = 'id'

message_controller_client.delete_using_delete_4(messsage_id, x_auth_token, id)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |




[Back to List of Controllers](#list_of_controllers)

## <a name="register_controler_controller"></a>![Class: ](https://apidocs.io/img/class.png ".RegisterControlerController") RegisterControlerController

### Get controller instance

An instance of the ``` RegisterControlerController ``` class can be accessed from the API Client.

```python
 register_controler_client = client.register_controler
```

### <a name="create_register_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".RegisterControlerController.create_register_using_post") create_register_using_post

> *Tags:*  ``` Skips Authentication ``` 

> register

```python
def create_register_using_post(self,
                                   resource)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |



#### Example Usage

```python
resource = RegisterResourceModel()

result = register_controler_client.create_register_using_post(resource)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_refresh_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".RegisterControlerController.create_refresh_using_post") create_refresh_using_post

> *Tags:*  ``` Skips Authentication ``` 

> refresh

```python
def create_refresh_using_post(self,
                                  resource)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |



#### Example Usage

```python
resource = SimpleEmailResourceModel()

result = register_controler_client.create_refresh_using_post(resource)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_activate_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".RegisterControlerController.get_activate_using_get") get_activate_using_get

> *Tags:*  ``` Skips Authentication ``` 

> activate

```python
def get_activate_using_get(self,
                               token,
                               id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| token |  ``` Required ```  | token |
| id |  ``` Required ```  | id |



#### Example Usage

```python
token = 'token'
id = 53

result = register_controler_client.get_activate_using_get(token, id)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="credit_consumption_controller"></a>![Class: ](https://apidocs.io/img/class.png ".CreditConsumptionController") CreditConsumptionController

### Get controller instance

An instance of the ``` CreditConsumptionController ``` class can be accessed from the API Client.

```python
 credit_consumption_controller_client = client.credit_consumption_controller
```

### <a name="list_using_get_2"></a>![Method: ](https://apidocs.io/img/method.png ".CreditConsumptionController.list_using_get_2") list_using_get_2

> *Tags:*  ``` Skips Authentication ``` 

> Get the consumption of the last months

```python
def list_using_get_2(self,
                         x_auth_token,
                         limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'
limit = 53

result = credit_consumption_controller_client.list_using_get_2(x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get_2"></a>![Method: ](https://apidocs.io/img/method.png ".CreditConsumptionController.list_page_using_get_2") list_page_using_get_2

> *Tags:*  ``` Skips Authentication ``` 

> Get pageable consumption of the last months

```python
def list_page_using_get_2(self,
                              page,
                              x_auth_token,
                              limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
page = 53
x_auth_token = 'X-Auth-Token'
limit = 53

result = credit_consumption_controller_client.list_page_using_get_2(page, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_using_get_1"></a>![Method: ](https://apidocs.io/img/method.png ".CreditConsumptionController.get_using_get_1") get_using_get_1

> *Tags:*  ``` Skips Authentication ``` 

> Get specific consumption by id 

```python
def get_using_get_1(self,
                        id,
                        x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
id = 53
x_auth_token = 'X-Auth-Token'

result = credit_consumption_controller_client.get_using_get_1(id, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="pricing_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PricingController") PricingController

### Get controller instance

An instance of the ``` PricingController ``` class can be accessed from the API Client.

```python
 pricing_controller_client = client.pricing_controller
```

### <a name="get_using_get_7"></a>![Method: ](https://apidocs.io/img/method.png ".PricingController.get_using_get_7") get_using_get_7

> *Tags:*  ``` Skips Authentication ``` 

> get

```python
def get_using_get_7(self,
                        x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'

result = pricing_controller_client.get_using_get_7(x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)

## <a name="message_model_controller"></a>![Class: ](https://apidocs.io/img/class.png ".MessageModelController") MessageModelController

### Get controller instance

An instance of the ``` MessageModelController ``` class can be accessed from the API Client.

```python
 message_model_controller_client = client.message_model_controller
```

### <a name="list_using_get_7"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.list_using_get_7") list_using_get_7

> *Tags:*  ``` Skips Authentication ``` 

> list

```python
def list_using_get_7(self,
                         x_auth_token,
                         size=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| size |  ``` Optional ```  | size |



#### Example Usage

```python
x_auth_token = 'X-Auth-Token'
size = 53

result = message_model_controller_client.list_using_get_7(x_auth_token, size)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="add_using_post_3"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.add_using_post_3") add_using_post_3

> *Tags:*  ``` Skips Authentication ``` 

> add

```python
def add_using_post_3(self,
                         resource,
                         x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
resource = MessageModelInputResourceModel()
x_auth_token = 'X-Auth-Token'

result = message_model_controller_client.add_using_post_3(resource, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="create_delete_multiple_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.create_delete_multiple_using_post") create_delete_multiple_using_post

> *Tags:*  ``` Skips Authentication ``` 

> deleteMultiple

```python
def create_delete_multiple_using_post(self,
                                          ids,
                                          x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ids |  ``` Required ```  ``` Collection ```  | ids |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
ids = ['ids']
x_auth_token = 'X-Auth-Token'

result = message_model_controller_client.create_delete_multiple_using_post(ids, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="list_page_using_get_7"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.list_page_using_get_7") list_page_using_get_7

> *Tags:*  ``` Skips Authentication ``` 

> listPage

```python
def list_page_using_get_7(self,
                              page,
                              x_auth_token,
                              limit=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| xAuthToken |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |



#### Example Usage

```python
page = 53
x_auth_token = 'X-Auth-Token'
limit = 53

result = message_model_controller_client.list_page_using_get_7(page, x_auth_token, limit)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_using_get_6"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.get_using_get_6") get_using_get_6

> *Tags:*  ``` Skips Authentication ``` 

> get

```python
def get_using_get_6(self,
                        id,
                        x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
id = 'id'
x_auth_token = 'X-Auth-Token'

result = message_model_controller_client.get_using_get_6(id, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="update_using_put_3"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.update_using_put_3") update_using_put_3

> *Tags:*  ``` Skips Authentication ``` 

> update

```python
def update_using_put_3(self,
                           id,
                           resource,
                           x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
id = 'id'
resource = MessageModelInputResourceModel()
x_auth_token = 'X-Auth-Token'

message_model_controller_client.update_using_put_3(id, resource, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="delete_using_delete_5"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.delete_using_delete_5") delete_using_delete_5

> *Tags:*  ``` Skips Authentication ``` 

> delete

```python
def delete_using_delete_5(self,
                              id,
                              x_auth_token)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| xAuthToken |  ``` Required ```  | X-Auth-Token |



#### Example Usage

```python
id = 'id'
x_auth_token = 'X-Auth-Token'

message_model_controller_client.delete_using_delete_5(id, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |




[Back to List of Controllers](#list_of_controllers)

## <a name="societe_info_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SocieteInfoController") SocieteInfoController

### Get controller instance

An instance of the ``` SocieteInfoController ``` class can be accessed from the API Client.

```python
 societe_info_controller_client = client.societe_info_controller
```

### <a name="create_research_company_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".SocieteInfoController.create_research_company_using_post") create_research_company_using_post

> *Tags:*  ``` Skips Authentication ``` 

> researchCompany

```python
def create_research_company_using_post(self,
                                           research)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| research |  ``` Required ```  | research |



#### Example Usage

```python
research = SocieteInfoResearchResourceModel()

result = societe_info_controller_client.create_research_company_using_post(research)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




### <a name="get_details_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".SocieteInfoController.get_details_using_get") get_details_using_get

> *Tags:*  ``` Skips Authentication ``` 

> getDetails

```python
def get_details_using_get(self,
                              id)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |



#### Example Usage

```python
id = 'id'

result = societe_info_controller_client.get_details_using_get(id)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |




[Back to List of Controllers](#list_of_controllers)



