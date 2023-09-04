# Magento_Prepraton
You added 3 product to the cart. What is the price will be final?
BasePrice - 50 SpecialPrice - 60 TierPrice for 2 products and more - 57 CatalogPrice Rule applied for 10% discount

Answer: 
50 x 3 x 0.9 = 135

***

A customer wants to change the 404 pages completely How to perform it?

Answer:
Add item for MagentoFrameworkAppRouterNoRouteHandlerList in the di.xml

*** 

A customer wants to change the 404 pages content What is the easiest way to do it?

Answer:
Create new cms_page and assign it in the system config

***

What is Magento vault?

Answer:
Storage for payment Token

***

To create a new configuration type(Choos 4):

Answer:
Create your XSD file.
Define a reader by extending MagentoFrameworkConfigReaderFilesystem
Create your XML file
Define your configuration object in your di.xml

***

The store owner has custom system of rewards for the customer. They want to add Balance with reward points to the Customer Account Dashboard. How do you customize it?

Answer:
Add block and template to customer_account_index.xml

***

An order has the additional attribute "Extended Guarantee Period". You want to show it as a column inside order history in Account Dashboard. How to add it?

Answer:
Add a child block to container inside sales_order_history.xml layout.

***

You want to sell a set of furniture. It is possible to order a table with adjustable size and color, change amounts and color of chairs. Which is the product type you choose?

Answer:
Bundle

***

You added a configurable product to the cart. You see configurable thumbnails image in cart. How to change it?

Answer:
Change config to Sales -> Checkout -> Shopping Cart -> Configurable Product Image -> Product Thumbnail Itself.

***

You added a grouped product to the cart. You see simple thumbnails image in cart. However want to see the same image for each option. How to change it?

Answer:
Change config to Sales -> Checkout -> Shopping Cart -> Grouped Product Image -> Parent Product Thumbnail.

***

What the requirement for adding an extension attribute to an entity?

Answer:
Entity has to implements MagentoFrameworkApiExtensibleDataInterface

***

You created a plugin for some method. Your business logic require doesn't call the original callable(proceed) method. What happened? (choose 2)

Answer:
"Subject" method won't be called
It will prevent the execution of all the plugins next in the chain and the original method call

***

Where are the locations of a template in Magento 2? (Choose 2)

Answer:
/view/frontend/templates/
/_/templates/

***

How templates are initiated?

Answer:
Templates are initiated in layout files, and each layout block has an associated template

***

Which products attributes are static? (choose 2)

Answer:
media_gallery
attribute_set_id

***

Where Magento 2 storing category name?

Answer:
catalog_category_entity_varchar

***

In your module, you use constant MagentoCatalogModelProductType::TYPE_SIMPLE. Which type of dependency you should set in composer.json

Answer:
Require

***

You inherited a class from 3rd party module. Which type of dependency you should set in composer.json?

Answer:
Require

***

You extended layout of 3rd party module. Which type of dependency you should set in composer.json?

Answer:
Suggest

***

You use the method from the 3rd party module. But you check if module enabled. Which type of dependency you should set in composer.json?

Answer:
Suggest

***

You created a plugin for ProductRepositroyInterface. Which type of dependency you should set in composer.json?

Answer:
Suggest

***

How to upgrade Magento 2 CE for specific version locally(in developer mode) (Choose 2)

Answer:
composer require magento/product-community-edition:
bin/magento setup:upgrade

***

What is different between entitytype_save_after and entitytype_save_commit_after? (Choose 2)

Answer:
If _save_after fails, data will not be persisted in DB.
If _save_commit_after fails, data will be persisted in DB anyway.

***

You want to prevent the collection loading in the specific method. You have some condition(for example Customer Groupe) What is the best way to customize it

public function loadingFoo($bar)
{
    return $this->collection->load();
}
Answer:
Around Plugin

***

You want to add your custom data to MagentoCheckoutModelCompositeConfigProvider:getSerializedCheckoutConfig. What is the best way to customize it?

Answer:
Add new item for configProviders in di.xml

***

What are GDPR and CCPA?

Answer:
Legislation that regulates data protection and privacy in the European Union and in the US California

***

How to create a Custom Order Status? (choose 2)

Answer:
Create new status in admin Stores -> Order Status -> Create New Status.
Assign Status to State in admin Stores -> Order Status -> Assignment Information.

***

You have form input in UI component form. How to add validation?

Answer:
Add node validation and add rule in the node

***

How to add a custom shipping carrier?(choose 2)

Answer:
Create default config in "config.xml" file
Create the carrier model that extends AbstractCarrier and implemets CarrierInterface

***

How to provide data from backend to UI component?

Answer:
Implement DataProviderInterface and declare inside node in ui_component config

***

How can you restrict access to extension attributes?

Answer:
You can utilize magneto ACL. Add inside extension_attributes.xml

***

What do extension attributes allow? (choose 2)

Answer:
Auto data hinting
Clear declaration via XML

***

What do extension attributes allow? (choose 2)

Answer:
Auto generating getters and setters for extension attributes
Use join directive for add attributes to a collection

***

You creating customer address custom attributes. Which config you should add that allows you to edit the attribute in admin? (choose 2)

Answer:
used_in_forms = 'admin'
s_system=0

***

You want to filter data from ProductRepository::getItems() What will you do?

Answer:
Utilize SearchCriteriaBuilder

***

By default you have product url: Example: http://mystore.com/helena-hooded-fleece.html

You have requirement including category path for all products Example: http://mystore.com/clotheth/hooded/helena-hooded-fleece.html

Answer:
Change Stores > Settings > Configuration > Categories Path for Product URLs

***

What does FrontController do in Magento2?

Answer:
Composite that searches through a list of router according to order

***

How to add a custom router?(choose 2)

Answer:
Implement RouterInterface
Add you route via di.xml to RouterList

***

What is the first argument in plugins?

Answer:
$subject (e. g. Instance of plugged class)

***

How to get original arguments in After Plugin?

Answer:
Generated code pass it automatically, since from 3rd argument

***

Magento area types are(choose 3):

Answer:
adminhtml, crontab, graphql
base, webapi_rest
webapi_soap, frontend

***

What pattern are you use each time when you adding something to di.xml

Answer:
dependency injection

***

A customer wants to add an extra block to product detailed page after SKU

Answer:
Add custom layout container to catalog_product_view.xml after sku block


***

How to create a new indexer?(choose 3)

Answer:
MagentoFrameworkIndexerActionInterface and MagentoFrameworkMviewActionInterface
Add etc/indexer.xml in your module
Add etc/ mview.xml in your module

***

How to use a Content Delivery Network for Media Files?

Answer:
Configure via Configuration/General/Web/Base URLs/ Base URL for User Media Files

***

What is the difference between varchar and static attributes?

Answer:
Static attribute is saved to _entity tables

***

What minimum requirements for creating a custom block?

Answer:
Implements MagentoFrameworkViewElementBlockInterface

***

Where do you set default config values for system configs?

Answer:
config.xml

***

How to reduce a performance impact for classes with a big amount of dependencies in a 3rd party modules?

Answer:
Add config for use proxy pattern via di.xml

***

Preferable way customizing Magento_Checkout/js/view/shipping in Magento checkout

Answer:
Create mixing

***

You want to convert data to lower case before an EAV attribute for ProductEntity saves. What will you choose?

Answer:
Create backend model

***

You want to validate data before an EAV attribute for CategoryEntity saves.

Answer:
Create backend model

***


What steps you should perform for adding viewModel to the block.(choose 2)

Answer:
Add via Layout
Create class that implements MagentoFrameworkViewElementBlockArgumentInterface

***

You need access to some data in myTemplate.phtml. What is the recommended approach?

Answer:
viewModel

***

How to get viewModel in a template?

Answer:
$block->getViewModel()

***

You added to default.xml

<referenceBlock name="content">
 <block name="myHeavyBlock" cacheable="false" template="havyBlocks/template.phtml"/>
</referenceBlock>
All pages become very slow. What happened?

Answer:
All pages become uncacheable

***

You want to add a discount when customers order more than 3 products. How to do it?

Answer:
Use Tired price via admin

***

Differences between developer and production mode? (choose 3)

Answer:
Developer - Shows errors on the frontend.
Production - Serves static view files from cache only.
Production - Does not allow you to enable or disable cache types in Magento Admin.

***


How to ship an item to a different location?

Answer:
Native feature Stores > Settings > Configuration > Sales > Multishipping Settings

***

Does Magento 2 use cookies out of the box?

Answer:
Yes

***

Can Magento 2 work without cookies?

Answer:
Yes, Magento 2 support cookie restricted mode.

***

What kind of Catalog Input Type for Store Owner must you set to make the attributes filterable in Layered Navigation? (Choose 2)

Answer:
Dropdown
Multiple Select

***

What kind of Catalog Input Type for Store Owner must you set to make the attributes filterable in Layered Navigation? (Choose 3)

Answer:
Dropdown
Price
Multiple Select

***

Advantages of using EAV for a merchant

Answer:
Changing attributes without altering DB schema

***

What interface should implement Each Action class?

Answer:
MagentoFrameworkAppActionInterface

***

A merchant asks you to create a module that is able to process URLs with a custom structure that can contain any combination of a product type code, a partial name, and a 4-digit year in any order.

The request path will look like this: /product/:type-code/:name-part/:year

Which layer in the Magento request processing flow is suited for this kind of customization?

Answer:
Router

***

While integrating a merchant’s product information management system with Magento, you create a module MyCompany_MerchantPim that adds a catalog product EAV attribute pim_entity_idprogrammatically.

In which type of setup script do you create the EAV attribute?

Answer:
Setup/UpgradeData.php

***

You are facing a bug, which is supposedly caused by the customization of MagentoCatalogApiProductRepositoryInterface::save().

To resolve the issue, you decide to find all logic which customizes this method. Which two places do you search for customization declarations? (Choose 2)

Answer:
*/di.xml
*/events.xml

***

You are implementing customization of the sales management within a module MyCompany_MySalesProcess. You have created several event observers to add custom functionality. Each observer is a separate class, but they require some common functionality.

How do you implement the common functionality in the event observers, keeping maintainability and testability in mind?

Answer:
You create a regular class implementing the common functionality as public methods and use constructor injection to make them available to the observers.

***

You are creating a new module to extend the functionality of the Magento application. What files are required?

Answer:
etc/module.xml, registration.php

***

A customer asked you to add the VAT number field to the shipping address form on checkout. What steps should you perform to achieve this? (choose 3)

Answer:
Add your field to JS layout via plugin MagentoCheckoutBlockCheckoutLayoutProcessor::process
Add a JS mixin for Magento_Checkout/js/action/set-shipping-information to modify data submission
Create extension attribute and add logic for process you field

***

Which Magento 2 products are composite? (choose 3)

Answer:
Bundle
Grouped
Configurable

***

The existing page layout does not meet your requirements. You created a new page layout 3-columns-double-footer. Should you do something else to get your page in the layouts list?

Answer:
Create view/frontend/layouts.xml with a node

***


How to add and display a category attribute? (choose 2)

Answer:
Add attribute using MagentoEavSetupEavSetup::addAttribute via data patch.
Creating a category_form.xml file in the view/adminhtml/ui_component directory in your module.

***

Keeping maintainability in mind, how do you add a new link to the customer account sidebar?

Answer:
Create customer_account.xml and add a block to the customer_account_navigation

***

What ways are possible to wrap a block with an HTML tag?

Answer:
Add a custom Layout XML container.
Add the tag to the template.

***


Keeping maintainability in mind, how do you customize the format of addresses in emails?

Answer:
Stores > Configuration > Customers > Customer Configuration > Address Templates.

***

What is the purpose of the getFlatColumns method in an EAV's Source model?

Answer:
It returns columns that will be added to the EAV model's flat table.

***


What only happens in the Production deploy mode?

Answer:
Errors are only logged, not shown to the user

***

You are configuring a new entry in etc/adminhtml/system.xml that is a select / dropdown type. What must the class for the source model extend or implement?

Answer:
MagentoFrameworkDataOptionSourceInterface

***

Magento uses the concept of service contracts to create a blueprint for modules to communicate with each other. Where are these service contracts stored in a module?

Answer:
Api

***

You need to add a fee (additional to tax and shipping) to every order placed. In what file do you specify the new total?

Answer:
etc/sales.xml

***

UpgradeSchema.php only provides one method: upgrade. What method do you use to determine what code to execute for what method?

Answer:
Use PHP's version_compare method to compare the $context->getVersion() with the required version.

***

You are customizing a third-party module and need to prevent an event handler from triggering. Keeping upgradeability in mind, how do you do this?

Answer:
Create an observer in events.xml with the same name and specify the disabled="true" attribute

***

What additional tools are available in the backend and not in frontend? (choose 3)

Answer:
Global records search
URL secret keys
ACL

***

You have created a custom theme and need to customize the view/frontend/templates/product/list.phtml file in the Magento_Catalog module. Where do you place this file inside your theme?

Answer:
Magento_Catalog/templates/product/list.phtml

***

What category path is the category that is the closest to the top of the tree, but still is visible on Layered Navigation?

Answer:
1/2/8

***

How do you create a new cache type?

Answer:
Create etc/cache.xml and specify a

***

You are tasked with installed a new 3-party module to show product promotions to a customer. What two steps do you take to make the module active? (choose 2)

Answer:
php bin/magento setup:upgrade
php bin/magento module:enable MyCompany_MyModule

***

What files are required for a new custom theme? (choose 2)

Answer:
registration.php
theme.xml

***

You performing a code review on an existing module. You see some interesting files in the Setup/ folder. What files in the Setup/ does Magento understand? (choose 3)

Answer:
Setup/UpgradeSchema.php
Setup/InstallSchema.php
Setup/Recurring.php

***

You need to create a custom price calculator for simple products. You have already creates the new price model. Keeping simplicity in mind, what additional steps do you take to implement this? (choose 2)

Answer:
In your product_types.xml, reference the simple product type, and set a value for the priceModel attribute.
Make your new price model extend MagentoCatalogModelProductTypePrice

***

You need to programatically create a new customer attribute that would be editable in admin panel. What steps are required to do this? (choose 2)

Answer:
Specify the used_in_forms data for the attribute
Create the attribute with MagentoCustomerSetupCustomerSetup::addAttribute

***

You are adding an extension attribute to the CustomerInterface class. You have specified data for the extension attribute, but when you check the database, nothing has been saved. Why is that?

Answer:
Extension attribute data is not automatically persisted to the database.

***


What Magento layout XML instructions instruct Magento to render HTML output?

Answer:
block

***

As you create a controller in Magento's adminhtml area, you must configure it to respond appropriately to the ACL. Keeping simplicity in mind, what steps do you take to implement this?

Answer:
Set the value of the ADMIN_RESOURCE constant of your class to be the ACL resource

***

When setData (' some', 'value') is called on an EAV entity and the entity is saved to the database?

Answer:
The 'value' of the attribute named ' some' is saved in one of the entity's tables depending on its datatype (for example, entityname_varchar)

***


Applying the shopping cart rule's action affects the quote item by setting the quote item's...

Answer:
base_discount_amount and discount_amount with the discount applied to original price

***

How to make attributes be able to be used in catalog price rules?

Answer:
Edit attributes to allow display in catalog condition


***

As you are assessing a 3rd-party module, you see this file: /Setup/InstallSchema.php. What is the intended purpose of this file?

Answer:
Installs schema-related entities (tables, columns) into the database.

***

Which of the following operations is most impacted (in time required) by a large number of products and stores?

Answer:
adding new attributes to be used in flat catalog

***

How do you enable customer comments on orders in Magento 2?

Answer:
Customer comments require a custom extension

***

Assume you have saved a product in the Catalog. Will your last changes be taken into account for rule-based related products?

Answer:
Yes, it will be done automatically by an observer on the catalog_product_save_after event.

***

Does Magento 2 have a “Saved Credit Card" payment method?"

Answer:
Customer can save their credit cards tokens in 'Saved Payment Methods' which are available only for payment methods such as Braintree, that offer a secure vault.


***

https://m2exam.decimadigital.com/magento-2-certification-question-list
