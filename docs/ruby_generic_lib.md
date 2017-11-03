# Getting started

sMsMode API-REST Documentation

## How to Build

This client library is a Ruby gem which can be compiled and used in your Ruby and Ruby on Rails project. This library requires a few gems from the RubyGems repository.

1. Open the command line interface or the terminal and navigate to the folder containing the source code.
2. Run ``` gem build s_msmode_apirest.gemspec ``` to build the gem.
3. Once built, the gem can be installed on the current work environment using ``` gem install s_msmode_apirest-2.25.1.gem ```

![Building Gem](https://apidocs.io/illustration/ruby?step=buildSDK&workspaceFolder=sMsmode%20API-REST-Ruby&workspaceName=sMsmode%20API-REST-Ruby&projectName=s_msmode_apirest&gemName=s_msmode_apirest&gemVer=2.25.1)

## How to Use

The following section explains how to use the SMsmodeApirest Ruby Gem in a new Rails project using RubyMine&trade;. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.

### 1. Starting a new project

Close any existing projects in RubyMine&trade; by selecting ``` File -> Close Project ```. Next, click on ``` Create New Project ``` to create a new project from scratch.

![Create a new project in RubyMine](https://apidocs.io/illustration/ruby?step=createNewProject0&workspaceFolder=sMsmode%20API-REST-Ruby&workspaceName=SMsmodeApirest&projectName=s_msmode_apirest&gemName=s_msmode_apirest&gemVer=2.25.1)

Next, provide ``` TestApp ``` as the project name, choose ``` Rails Application ``` as the project type, and click ``` OK ```.

![Create a new Rails Application in RubyMine - step 1](https://apidocs.io/illustration/ruby?step=createNewProject1&workspaceFolder=sMsmode%20API-REST-Ruby&workspaceName=SMsmodeApirest&projectName=s_msmode_apirest&gemName=s_msmode_apirest&gemVer=2.25.1)

In the next dialog make sure that correct *Ruby SDK* is being used (minimum 2.0.0) and click ``` OK ```.

![Create a new Rails Application in RubyMine - step 2](https://apidocs.io/illustration/ruby?step=createNewProject2&workspaceFolder=sMsmode%20API-REST-Ruby&workspaceName=SMsmodeApirest&projectName=s_msmode_apirest&gemName=s_msmode_apirest&gemVer=2.25.1)

This will create a new Rails Application project with an existing set of files and folder.

### 2. Add reference of the gem

In order to use the SMsmodeApirest gem in the new project we must add a gem reference. Locate the ```Gemfile``` in the *Project Explorer* window under the ``` TestApp ``` project node. The file contains references to all gems being used in the project. Here, add the reference to the library gem by adding the following line: ``` gem 's_msmode_apirest', '~> 2.25.1' ```

![Add references of the Gemfile](https://apidocs.io/illustration/ruby?step=addReference&workspaceFolder=sMsmode%20API-REST-Ruby&workspaceName=SMsmodeApirest&projectName=s_msmode_apirest&gemName=s_msmode_apirest&gemVer=2.25.1)

### 3. Adding a new Rails Controller

Once the ``` TestApp ``` project is created, a folder named ``` controllers ``` will be visible in the *Project Explorer* under the following path: ``` TestApp > app > controllers ```. Right click on this folder and select ``` New -> Run Rails Generator... ```.

![Run Rails Generator on Controllers Folder](https://apidocs.io/illustration/ruby?step=addCode0&workspaceFolder=sMsmode%20API-REST-Ruby&workspaceName=SMsmodeApirest&projectName=s_msmode_apirest&gemName=s_msmode_apirest&gemVer=2.25.1)

Selecting the said option will popup a small window where the generator names are displayed. Here, select the ``` controller ``` template.

![Create a new Controller](https://apidocs.io/illustration/ruby?step=addCode1&workspaceFolder=sMsmode%20API-REST-Ruby&workspaceName=SMsmodeApirest&projectName=s_msmode_apirest&gemName=s_msmode_apirest&gemVer=2.25.1)

Next, a popup window will ask you for a Controller name and included Actions. For controller name provide ``` Hello ``` and include an action named ``` Index ``` and click ``` OK ```.

![Add a new Controller](https://apidocs.io/illustration/ruby?step=addCode2&workspaceFolder=sMsmode%20API-REST-Ruby&workspaceName=SMsmodeApirest&projectName=s_msmode_apirest&gemName=s_msmode_apirest&gemVer=2.25.1)

A new controller class anmed ``` HelloController ``` will be created in a file named ``` hello_controller.rb ``` containing a method named ``` Index ```. In this method, add code for initialization and a sample for its usage.

![Initialize the library](https://apidocs.io/illustration/ruby?step=addCode3&workspaceFolder=sMsmode%20API-REST-Ruby&workspaceName=SMsmodeApirest&projectName=s_msmode_apirest&gemName=s_msmode_apirest&gemVer=2.25.1)

## How to Test

You can test the generated SDK and the server with automatically generated test
cases as follows:

  1. From terminal/cmd navigate to the root directory of the SDK.
  2. Invoke: `bundle exec rake`

## Initialization

### 

API client can be initialized as following.

```ruby

client = SMsmodeApirest::SMsmodeApirestClient.new
```

The added initlization code can be debugged by putting a breakpoint in the ``` Index ``` method and running the project in debug mode by selecting ``` Run -> Debug 'Development: TestApp' ```.

![Debug the TestApp](https://apidocs.io/illustration/ruby?step=addCode4&workspaceFolder=sMsmode%20API-REST-Ruby&workspaceName=SMsmodeApirest&projectName=s_msmode_apirest&gemName=s_msmode_apirest&gemVer=2.25.1&initLine=client%2520%253D%2520SMsmodeApirestClient.new)



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

```ruby
reportController = client.report_controller
```

### <a name="list_using_get_8"></a>![Method: ](https://apidocs.io/img/method.png ".ReportController.list_using_get_8") list_using_get_8

> *Tags:*  ``` Skips Authentication ``` 

> list


```ruby
def list_using_get_8(x_auth_token,
                         limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'
limit = 153

result = reportController.list_using_get_8(x_auth_token, limit)

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


```ruby
def list_page_using_get_8(page,
                              x_auth_token,
                              limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
page = 153
x_auth_token = 'X-Auth-Token'
limit = 153

result = reportController.list_page_using_get_8(page, x_auth_token, limit)

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


```ruby
def get_using_get_8(message_ref,
                        x_auth_token,
                        limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| message_ref |  ``` Required ```  | messageRef |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
message_ref = 'messageRef'
x_auth_token = 'X-Auth-Token'
limit = 153

result = reportController.get_using_get_8(message_ref, x_auth_token, limit)

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


```ruby
def get_page_using_get(message_ref,
                           page,
                           x_auth_token,
                           limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| message_ref |  ``` Required ```  | messageRef |
| page |  ``` Required ```  | page |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
message_ref = 'messageRef'
page = 153
x_auth_token = 'X-Auth-Token'
limit = 153

result = reportController.get_page_using_get(message_ref, page, x_auth_token, limit)

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


```ruby
def find_using_get(message_ref,
                       destinataire,
                       x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| message_ref |  ``` Required ```  | messageRef |
| destinataire |  ``` Required ```  | destinataire |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
message_ref = 'messageRef'
destinataire = 'destinataire'
x_auth_token = 'X-Auth-Token'

result = reportController.find_using_get(message_ref, destinataire, x_auth_token)

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

```ruby
invoiceController = client.invoice_controller
```

### <a name="list_using_get_5"></a>![Method: ](https://apidocs.io/img/method.png ".InvoiceController.list_using_get_5") list_using_get_5

> *Tags:*  ``` Skips Authentication ``` 

> View a list of invoices


```ruby
def list_using_get_5(x_auth_token,
                         limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'
limit = 153

result = invoiceController.list_using_get_5(x_auth_token, limit)

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


```ruby
def list_page_using_get_5(page,
                              x_auth_token,
                              limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
page = 153
x_auth_token = 'X-Auth-Token'
limit = 153

result = invoiceController.list_page_using_get_5(page, x_auth_token, limit)

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


```ruby
def get_pdf_using_get(id,
                          x_auth_token,
                          base64); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| base64 |  ``` Required ```  | base64 |


#### Example Usage

```ruby
id = 153
x_auth_token = 'X-Auth-Token'
base64 = true

result = invoiceController.get_pdf_using_get(id, x_auth_token, base64)

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


```ruby
def get_using_get_5(id,
                        x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
id = 153
x_auth_token = 'X-Auth-Token'

result = invoiceController.get_using_get_5(id, x_auth_token)

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

```ruby
authenticationController = client.authentication_controller
```

### <a name="create_get_token_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".AuthenticationController.create_get_token_using_post") create_get_token_using_post

> *Tags:*  ``` Skips Authentication ``` 

> Generate the OAuth Token


```ruby
def create_get_token_using_post(request); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| request |  ``` Required ```  | request |


#### Example Usage

```ruby
request = AuthenticationResourceModel.new

result = authenticationController.create_get_token_using_post(request)

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

```ruby
contactController = client.contact_controller
```

### <a name="list_using_get_1"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.list_using_get_1") list_using_get_1

> *Tags:*  ``` Skips Authentication ``` 

> View a list of contacts


```ruby
def list_using_get_1(x_auth_token,
                         limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'
limit = 153

result = contactController.list_using_get_1(x_auth_token, limit)

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


```ruby
def add_using_post(resource,
                       x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
resource = ContactResourceModel.new
x_auth_token = 'X-Auth-Token'

result = contactController.add_using_post(resource, x_auth_token)

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


```ruby
def delete_book_using_delete(x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'

result = contactController.delete_book_using_delete(x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



### <a name="get_customer_info_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.get_customer_info_using_get") get_customer_info_using_get

> *Tags:*  ``` Skips Authentication ``` 

> Show contact info of customer


```ruby
def get_customer_info_using_get(x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'

result = contactController.get_customer_info_using_get(x_auth_token)

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


```ruby
def update_edit_customer_using_put(x_auth_token,
                                       resource); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| resource |  ``` Required ```  | resource |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'
resource = ContactResourceModel.new

result = contactController.update_edit_customer_using_put(x_auth_token, resource)

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


```ruby
def create_delete_list_using_post(id_list,
                                      x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id_list |  ``` Required ```  ``` Collection ```  | idList |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
id_list = [153]
x_auth_token = 'X-Auth-Token'

result = contactController.create_delete_list_using_post(id_list, x_auth_token)

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


```ruby
def create_export_contacts_using_post(fields,
                                          x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| fields |  ``` Required ```  ``` Collection ```  | fields |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
fields = ['fields']
x_auth_token = 'X-Auth-Token'

result = contactController.create_export_contacts_using_post(fields, x_auth_token)

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


```ruby
def upload_blocking_using_post(file,
                                   model,
                                   x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | file |
| model |  ``` Required ```  | model |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
file = Faraday::UploadIO.new('PathToFile', 'application/octet-stream')
model = 'model'
x_auth_token = 'X-Auth-Token'

result = contactController.upload_blocking_using_post(file, model, x_auth_token)

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


```ruby
def list_page_using_get_1(page,
                              x_auth_token,
                              limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
page = 153
x_auth_token = 'X-Auth-Token'
limit = 153

result = contactController.list_page_using_get_1(page, x_auth_token, limit)

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


```ruby
def search_using_get_1(name,
                           x_auth_token,
                           limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
name = 'name'
x_auth_token = 'X-Auth-Token'
limit = 153

result = contactController.search_using_get_1(name, x_auth_token, limit)

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


```ruby
def get_using_get(id,
                      x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
id = 153
x_auth_token = 'X-Auth-Token'

result = contactController.get_using_get(id, x_auth_token)

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


```ruby
def update_using_put(id,
                         resource,
                         x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
id = 153
resource = ContactResourceModel.new
x_auth_token = 'X-Auth-Token'

result = contactController.update_using_put(id, resource, x_auth_token)

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


```ruby
def delete_using_delete_1(id,
                              x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
id = 153
x_auth_token = 'X-Auth-Token'

result = contactController.delete_using_delete_1(id, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



### <a name="add_group_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".ContactController.add_group_using_post") add_group_using_post

> *Tags:*  ``` Skips Authentication ``` 

> Add a contact in a group


```ruby
def add_group_using_post(id,
                             group_id,
                             x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| group_id |  ``` Required ```  | groupId |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
id = 153
group_id = 153
x_auth_token = 'X-Auth-Token'

result = contactController.add_group_using_post(id, group_id, x_auth_token)

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


```ruby
def get_groups_using_get(id,
                             page,
                             x_auth_token,
                             limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| page |  ``` Required ```  | page |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
id = 153
page = 153
x_auth_token = 'X-Auth-Token'
limit = 153

result = contactController.get_groups_using_get(id, page, x_auth_token, limit)

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


```ruby
def delete_group_using_delete(id,
                                  group_id,
                                  x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| group_id |  ``` Required ```  | groupId |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
id = 153
group_id = 153
x_auth_token = 'X-Auth-Token'

result = contactController.delete_group_using_delete(id, group_id, x_auth_token)

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

```ruby
customerController = client.customer_controller
```

### <a name="get_using_get_2"></a>![Method: ](https://apidocs.io/img/method.png ".CustomerController.get_using_get_2") get_using_get_2

> *Tags:*  ``` Skips Authentication ``` 

> Show your account


```ruby
def get_using_get_2(x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'

result = customerController.get_using_get_2(x_auth_token)

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


```ruby
def get_from_fields_using_get(x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'

result = customerController.get_from_fields_using_get(x_auth_token)

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


```ruby
def update_delete_sender_using_put(x_auth_token,
                                       sender_id); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| sender_id |  ``` Required ```  | senderID |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'
sender_id = 'senderID'

result = customerController.update_delete_sender_using_put(x_auth_token, sender_id)

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


```ruby
def add_sender_using_post(x_auth_token,
                              sender_id); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| sender_id |  ``` Required ```  | senderID |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'
sender_id = 'senderID'

result = customerController.add_sender_using_post(x_auth_token, sender_id)

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


```ruby
def list_using_get_3(x_auth_token,
                         limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'
limit = 244

result = customerController.list_using_get_3(x_auth_token, limit)

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


```ruby
def list_page_using_get_3(page,
                              x_auth_token,
                              limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
page = 244
x_auth_token = 'X-Auth-Token'
limit = 244

result = customerController.list_page_using_get_3(page, x_auth_token, limit)

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

```ruby
groupController = client.group_controller
```

### <a name="list_using_get_4"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.list_using_get_4") list_using_get_4

> *Tags:*  ``` Skips Authentication ``` 

> View a list of groups


```ruby
def list_using_get_4(x_auth_token,
                         limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'
limit = 244

result = groupController.list_using_get_4(x_auth_token, limit)

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


```ruby
def add_using_post_2(resource,
                         x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
resource = GroupResourceModel.new
x_auth_token = 'X-Auth-Token'

result = groupController.add_using_post_2(resource, x_auth_token)

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


```ruby
def create_delete_list_using_post_1(id_list,
                                        x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id_list |  ``` Required ```  ``` Collection ```  | idList |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
id_list = [244]
x_auth_token = 'X-Auth-Token'

result = groupController.create_delete_list_using_post_1(id_list, x_auth_token)

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


```ruby
def list_page_using_get_4(page,
                              x_auth_token,
                              limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
page = 244
x_auth_token = 'X-Auth-Token'
limit = 244

result = groupController.list_page_using_get_4(page, x_auth_token, limit)

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


```ruby
def search_using_get_2(name,
                           x_auth_token,
                           limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
name = 'name'
x_auth_token = 'X-Auth-Token'
limit = 244

result = groupController.search_using_get_2(name, x_auth_token, limit)

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


```ruby
def get_using_get_4(id,
                        x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
id = 244
x_auth_token = 'X-Auth-Token'

result = groupController.get_using_get_4(id, x_auth_token)

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


```ruby
def update_using_put_2(id,
                           resource,
                           x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
id = 244
resource = GroupResourceModel.new
x_auth_token = 'X-Auth-Token'

result = groupController.update_using_put_2(id, resource, x_auth_token)

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


```ruby
def delete_using_delete_3(id,
                              x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
id = 244
x_auth_token = 'X-Auth-Token'

result = groupController.delete_using_delete_3(id, x_auth_token)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |



### <a name="get_contacts_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".GroupController.get_contacts_using_get") get_contacts_using_get

> *Tags:*  ``` Skips Authentication ``` 

> Show a list of contacts for a group


```ruby
def get_contacts_using_get(id,
                               page,
                               x_auth_token,
                               limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| page |  ``` Required ```  | page |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
id = 244
page = 244
x_auth_token = 'X-Auth-Token'
limit = 244

result = groupController.get_contacts_using_get(id, page, x_auth_token, limit)

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

```ruby
campaignController = client.campaign_controller
```

### <a name="list_using_get"></a>![Method: ](https://apidocs.io/img/method.png ".CampaignController.list_using_get") list_using_get

> *Tags:*  ``` Skips Authentication ``` 

> list


```ruby
def list_using_get(x_auth_token,
                       limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'
limit = 244

result = campaignController.list_using_get(x_auth_token, limit)

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


```ruby
def create_send_to_list_using_post(resource,
                                       x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
resource = CampaignInputResourceModel.new
x_auth_token = 'X-Auth-Token'

result = campaignController.create_send_to_list_using_post(resource, x_auth_token)

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


```ruby
def list_page_using_get(page,
                            x_auth_token,
                            limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
page = 244
x_auth_token = 'X-Auth-Token'
limit = 244

result = campaignController.list_page_using_get(page, x_auth_token, limit)

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


```ruby
def search_using_get(name,
                         x_auth_token,
                         limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| name |  ``` Required ```  | name |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
name = 'name'
x_auth_token = 'X-Auth-Token'
limit = 244

result = campaignController.search_using_get(name, x_auth_token, limit)

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


```ruby
def delete_using_delete(messsage_id,
                            x_auth_token,
                            id); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsage_id |  ``` Required ```  | messsageId |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| id |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
messsage_id = 'messsageId'
x_auth_token = 'X-Auth-Token'
id = 'id'

result = campaignController.delete_using_delete(messsage_id, x_auth_token, id)

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

```ruby
transferController = client.transfer_controller
```

### <a name="list_using_get_9"></a>![Method: ](https://apidocs.io/img/method.png ".TransferController.list_using_get_9") list_using_get_9

> *Tags:*  ``` Skips Authentication ``` 

> View a list of transferts


```ruby
def list_using_get_9(x_auth_token,
                         limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'
limit = 244

result = transferController.list_using_get_9(x_auth_token, limit)

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


```ruby
def list_page_using_get_9(page,
                              x_auth_token,
                              limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
page = 244
x_auth_token = 'X-Auth-Token'
limit = 244

result = transferController.list_page_using_get_9(page, x_auth_token, limit)

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


```ruby
def get_using_get_9(id,
                        x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
id = 244
x_auth_token = 'X-Auth-Token'

result = transferController.get_using_get_9(id, x_auth_token)

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

```ruby
emailApiConfigurationController = client.email_api_configuration_controller
```

### <a name="get_using_get_3"></a>![Method: ](https://apidocs.io/img/method.png ".EmailApiConfigurationController.get_using_get_3") get_using_get_3

> *Tags:*  ``` Skips Authentication ``` 

> Show your configuration


```ruby
def get_using_get_3(x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'

result = emailApiConfigurationController.get_using_get_3(x_auth_token)

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


```ruby
def update_using_put_1(resource,
                           x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
resource = EmailAPIConfigurationResourceModel.new
x_auth_token = 'X-Auth-Token'

result = emailApiConfigurationController.update_using_put_1(resource, x_auth_token)

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


```ruby
def add_using_post_1(resource,
                         x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
resource = EmailAPIConfigurationResourceModel.new
x_auth_token = 'X-Auth-Token'

result = emailApiConfigurationController.add_using_post_1(resource, x_auth_token)

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


```ruby
def delete_using_delete_2(x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'

result = emailApiConfigurationController.delete_using_delete_2(x_auth_token)

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

```ruby
messageController = client.message_controller
```

### <a name="list_using_get_6"></a>![Method: ](https://apidocs.io/img/method.png ".MessageController.list_using_get_6") list_using_get_6

> *Tags:*  ``` Skips Authentication ``` 

> list


```ruby
def list_using_get_6(x_auth_token,
                         limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'
limit = 244

result = messageController.list_using_get_6(x_auth_token, limit)

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


```ruby
def list_page_using_get_6(page,
                              x_auth_token,
                              limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
page = 244
x_auth_token = 'X-Auth-Token'
limit = 244

result = messageController.list_page_using_get_6(page, x_auth_token, limit)

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


```ruby
def list_responses_using_get(x_auth_token,
                                 limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'
limit = 244

result = messageController.list_responses_using_get(x_auth_token, limit)

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


```ruby
def list_responses_page_using_get(page,
                                      x_auth_token,
                                      limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
page = 244
x_auth_token = 'X-Auth-Token'
limit = 244

result = messageController.list_responses_page_using_get(page, x_auth_token, limit)

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


```ruby
def list_scheduled_using_get(x_auth_token,
                                 limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'
limit = 244

result = messageController.list_scheduled_using_get(x_auth_token, limit)

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


```ruby
def list_scheduled_page_using_get(page,
                                      x_auth_token,
                                      limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
page = 244
x_auth_token = 'X-Auth-Token'
limit = 244

result = messageController.list_scheduled_page_using_get(page, x_auth_token, limit)

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


```ruby
def search_using_get_3(id,
                           x_auth_token,
                           limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
id = 'id'
x_auth_token = 'X-Auth-Token'
limit = 244

result = messageController.search_using_get_3(id, x_auth_token, limit)

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


```ruby
def create_send_to_list_using_post_1(resource,
                                         x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
resource = MessageInputMixedResourceModel.new
x_auth_token = 'X-Auth-Token'

result = messageController.create_send_to_list_using_post_1(resource, x_auth_token)

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


```ruby
def create_send_to_contact_list_using_post(resource,
                                               x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
resource = MessageInputContactResourceModel.new
x_auth_token = 'X-Auth-Token'

messageController.create_send_to_contact_list_using_post(resource, x_auth_token)

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


```ruby
def create_send_to_group_list_using_post(resource,
                                             x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
resource = MessageInputGroupResourceModel.new
x_auth_token = 'X-Auth-Token'

messageController.create_send_to_group_list_using_post(resource, x_auth_token)

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


```ruby
def create_send_to_number_list_using_post(resource,
                                              x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
resource = MessageInputResourceModel.new
x_auth_token = 'X-Auth-Token'

result = messageController.create_send_to_number_list_using_post(resource, x_auth_token)

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


```ruby
def delete_using_delete_4(messsage_id,
                              x_auth_token,
                              id); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| messsage_id |  ``` Required ```  | messsageId |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| id |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
messsage_id = 'messsageId'
x_auth_token = 'X-Auth-Token'
id = 'id'

messageController.delete_using_delete_4(messsage_id, x_auth_token, id)

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

```ruby
registerControler = client.register_controler
```

### <a name="create_register_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".RegisterControlerController.create_register_using_post") create_register_using_post

> *Tags:*  ``` Skips Authentication ``` 

> register


```ruby
def create_register_using_post(resource); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |


#### Example Usage

```ruby
resource = RegisterResourceModel.new

result = registerControler.create_register_using_post(resource)

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


```ruby
def create_refresh_using_post(resource); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |


#### Example Usage

```ruby
resource = SimpleEmailResourceModel.new

result = registerControler.create_refresh_using_post(resource)

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


```ruby
def get_activate_using_get(token,
                               id); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| token |  ``` Required ```  | token |
| id |  ``` Required ```  | id |


#### Example Usage

```ruby
token = 'token'
id = 244

result = registerControler.get_activate_using_get(token, id)

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

```ruby
creditConsumptionController = client.credit_consumption_controller
```

### <a name="list_using_get_2"></a>![Method: ](https://apidocs.io/img/method.png ".CreditConsumptionController.list_using_get_2") list_using_get_2

> *Tags:*  ``` Skips Authentication ``` 

> Get the consumption of the last months


```ruby
def list_using_get_2(x_auth_token,
                         limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'
limit = 244

result = creditConsumptionController.list_using_get_2(x_auth_token, limit)

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


```ruby
def list_page_using_get_2(page,
                              x_auth_token,
                              limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
page = 244
x_auth_token = 'X-Auth-Token'
limit = 244

result = creditConsumptionController.list_page_using_get_2(page, x_auth_token, limit)

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


```ruby
def get_using_get_1(id,
                        x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
id = 244
x_auth_token = 'X-Auth-Token'

result = creditConsumptionController.get_using_get_1(id, x_auth_token)

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

```ruby
pricingController = client.pricing_controller
```

### <a name="get_using_get_7"></a>![Method: ](https://apidocs.io/img/method.png ".PricingController.get_using_get_7") get_using_get_7

> *Tags:*  ``` Skips Authentication ``` 

> get


```ruby
def get_using_get_7(x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'

result = pricingController.get_using_get_7(x_auth_token)

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

```ruby
messageModelController = client.message_model_controller
```

### <a name="list_using_get_7"></a>![Method: ](https://apidocs.io/img/method.png ".MessageModelController.list_using_get_7") list_using_get_7

> *Tags:*  ``` Skips Authentication ``` 

> list


```ruby
def list_using_get_7(x_auth_token,
                         size = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| size |  ``` Optional ```  | size |


#### Example Usage

```ruby
x_auth_token = 'X-Auth-Token'
size = 244

result = messageModelController.list_using_get_7(x_auth_token, size)

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


```ruby
def add_using_post_3(resource,
                         x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| resource |  ``` Required ```  | resource |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
resource = MessageModelInputResourceModel.new
x_auth_token = 'X-Auth-Token'

result = messageModelController.add_using_post_3(resource, x_auth_token)

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


```ruby
def create_delete_multiple_using_post(ids,
                                          x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| ids |  ``` Required ```  ``` Collection ```  | ids |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
ids = ['ids']
x_auth_token = 'X-Auth-Token'

result = messageModelController.create_delete_multiple_using_post(ids, x_auth_token)

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


```ruby
def list_page_using_get_7(page,
                              x_auth_token,
                              limit = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| page |  ``` Required ```  | page |
| x_auth_token |  ``` Required ```  | X-Auth-Token |
| limit |  ``` Optional ```  | limit |


#### Example Usage

```ruby
page = 81
x_auth_token = 'X-Auth-Token'
limit = 81

result = messageModelController.list_page_using_get_7(page, x_auth_token, limit)

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


```ruby
def get_using_get_6(id,
                        x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
id = 'id'
x_auth_token = 'X-Auth-Token'

result = messageModelController.get_using_get_6(id, x_auth_token)

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


```ruby
def update_using_put_3(id,
                           resource,
                           x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| resource |  ``` Required ```  | resource |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
id = 'id'
resource = MessageModelInputResourceModel.new
x_auth_token = 'X-Auth-Token'

messageModelController.update_using_put_3(id, resource, x_auth_token)

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


```ruby
def delete_using_delete_5(id,
                              x_auth_token); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |
| x_auth_token |  ``` Required ```  | X-Auth-Token |


#### Example Usage

```ruby
id = 'id'
x_auth_token = 'X-Auth-Token'

messageModelController.delete_using_delete_5(id, x_auth_token)

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

```ruby
societeInfoController = client.societe_info_controller
```

### <a name="create_research_company_using_post"></a>![Method: ](https://apidocs.io/img/method.png ".SocieteInfoController.create_research_company_using_post") create_research_company_using_post

> *Tags:*  ``` Skips Authentication ``` 

> researchCompany


```ruby
def create_research_company_using_post(research); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| research |  ``` Required ```  | research |


#### Example Usage

```ruby
research = SocieteInfoResearchResourceModel.new

result = societeInfoController.create_research_company_using_post(research)

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


```ruby
def get_details_using_get(id); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| id |  ``` Required ```  | id |


#### Example Usage

```ruby
id = 'id'

result = societeInfoController.get_details_using_get(id)

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |



[Back to List of Controllers](#list_of_controllers)



