# Custom Stock Status User Guide

## Overview


Custom Stock Status will help admin install additional stock statuses for the products. Information about the product's stock status is displayed at the frontend more accurately and clearly, giving customers better shopping experience and increasing the ability to buy from them. In particular, admins can custom stock status automatically or manually with image and text to quickly attract customers' attention with appealing status. That's the feature of [Mageplaza Custom Stock Status](https://www.mageplaza.com/magento-2-custom-stock-status/) extension.

## How to download and install 

- [Download Mageplaza Custom Stock Status](https://www.mageplaza.com/magento-2-custom-stock-status/)
- [Install Custom Stock Status](https://www.mageplaza.com/install-magento-2-extension/)

## How to use

Custom Stock Status apply for the followign product types:

- Simple Product

![Imgur](https://i.imgur.com/7Dc7N7i.png)

- Bundle Product: Can apply for child products of Bundle products

![Imgur](https://i.imgur.com/hWVisBa.png)

- Group Product: Can apply for child products of Bundle products

![Imgur](https://i.imgur.com/GdHFzkq.png)

- Configurable Product: With this product type, you can configure the Custom Stock Status by size and color of products

![Imgur](https://i.imgur.com/CRmRC4F.gif)

## How to configure

### 1. Configuration

Login to the **Admin Magento**, choose `Stores> Custom Stock Status> Configuration`.

![Imgur](https://i.imgur.com/arLBQ5Q.png)

#### 1.1. General configuration

![Imgur](https://i.imgur.com/0JUZZGZ.png)

- **Enable**: Select `Yes` to turn on the module
- **Apply for Products**: Choose to apply **Custom Stock Status** to products:
  - **Instock**: only instock products will be applied **Custom Stock Status**.
  - **Out of stock**: only out of stock products are applied **Custom Stock Status**.
  - **Both**: apply custom stock status to all products.
- **Status format**: Choose to display the status of the product in **Frontend** with:
  - Image + Text: Show by the order of image then text
  
  ![Imgur](https://i.imgur.com/wSXuNsY.png)
  
  - Image Only: Only show Custom Stock Status with image
  
  ![Imgur](https://i.imgur.com/FVSXLYF.png)
  
  - Text only: Only show Custom Stock Status with text
  
  ![Imgur](https://i.imgur.com/Hv5nOfh.png)
  
  - Text + Image: Show by the order of text then image
  
  ![Imgur](https://i.imgur.com/0Jkk4Mq.png)
  
  
- **Display On**: Choose to display the **Custom Stock Status** on the page below. You can choose to apply to multiple pages at the same time. Those not selected will not be applied:
  - Product Listing Page:
  
  ![Imgur](https://i.imgur.com/5q577ZY.png)
  
  
  - Product View Page
  
  ![Imgur](https://i.imgur.com/Jf1uKVo.png)
  
  - Shopping Cart Page
  
  ![Imgur](https://i.imgur.com/IRw72Hm.png)
  
  
  - Mageplaza One Step Checkout: This option only displays **Custom Stock Status** when you install the [Mageplaza's One Step Checkout](https://www.mageplaza.com/magento-2-one-step-checkout-extension/) extension. With this extension integration, you can summarize 6 payment steps in just one page to make it easier for customers to shorten the payment process.
  
  ![Imgur](https://i.imgur.com/amI1oMI.png)
  
- **Apply with Child Configurable Product Options**:
  - Selecting "Yes" to display the **Custom Stock Status** on options such as size, color, ... with the **Configurable Product** and the **sub-products** of **Group Product, Bundle Product**.
  - Selecting "No" will not display the **Custom Stock Status** at any child product type.
  
- **Enable Automatic Stock Status based on Dynamic Quantity Ranges**:
  - Select `Yes`, it will enable **Automatic Stock Status based on Dynamic Quantity Ranges**. If the product satisfies Dynamic Group, it will apply Stock Status with Group Name group. Dynamic Group applies only to Simple Group.
  - If "No" is selected, it will not apply **Dynamic Groups**.
  - In case both the **Custom Stock Status** and **Dynamic Groups** are selected and enable, it will prioritize the information in the previous **Dynamic Groups** field. You can access  Store> Attributes> Product` to search with 2 attributes to create additional options for **Custom Stock Status** and **Dynamic Groups**.
  
**Note**:
- If you want the inventory status to become clear and notify the email to the customer when the product comes back to the warehouse or change the product price, with [Mageplaza's Product Alerts](https://www.mageplaza.com/magento-2-product-alerts/) extension, it will help you do that and it is completely compatible with **Custom Stock Status** extension.
- Or customers can pre-order and order later if you don't currently have enough products, with [Mageplaza's Pre Order](https://www.mageplaza.com/magento-2-pre-order/) extension, it will help you solve that problem and it is also fully compatible with **Custom Stock Status** extension.

### 2. Manage Custom Stock Status
Login to the Magento Admin, choose `Stores > Custom Stock Status > Manage Custom Stock Status`. Or you can access to `Store > Attributes > Product`, find `mp_stock_status` at Attributes Code.

![Imgur](https://i.imgur.com/wbATrcL.png)

In this section, configure the option of attributes for the Custom Stock Status field when accessing `Catalog> Product`, edit a product.

#### 2.1. Properties
##### 2.1.1. Attribute Properties

![Imgur](https://i.imgur.com/i8Cmk1D.png)


- Default Label:
  - You can change the name for attributes, the names of these attributes will be displayed in the `Catalog> Product` section, edit a product.
  - This is a required field.
  
- Catalog Input Type for Store Owner: Select the input type. Include options:
  - Visual Swatch: Create an option of attributes Custom Stock Status in Manage Swatch (Values of Your Attribute) with label and image. You can upload image with .gif, .jpg, .png format. You can enter the option replacement name of attributes Custom Stock  Status for each store. Here, we support adding the variable in status to the Quantity label of the product. For example: Only {{qty}} in stock, Will be available tomorrow, {{attribute_code}}
  
  ![Imgur](https://i.imgur.com/BzgUBzD.png)
  
  Note: If you select the Visual Swatch, you can display both the label and image outside the Frontend for Custom Stock Status, depending on the selection of the Status format field at Configuration.
With Admin is the price you must enter and for each store you can replace the option name of attributes. If the names of the stores are left blank, they will default to Admin values.
Values Required: If "yes" is selected, attributes will be set to the default values required to select an option of attributes.
2.1.2. Advanced Attribute Properties
This section you can configure the display position design of attributes. With the Attribute Code field and the Validation Input for Store Owner the default value.


2.2. Manage Labels
Fill Titles to replace Attributes Custom Stock Status shows which store you want. The title will display replacing the Attributes name. If left blank, it will default to the Attributes name you set in the Default Label field. Example: Custom Stock Status

2.3. Storefront Properties
Select Storefront Properties information to display Attributes in the store location you want.

3. Manage Dynamic Groups
Login to the Magento Admin, choose Stores> Custom Stock Status> Manage Dynamic Quantity Groups. Or you can visit Store> Attributes> Product, search in Attributes Code field with mp_dynamic_groups.
For Dynamic Group, it only applies to Simple Product and if the product satisfies Dynamic Group, it will give priority to consider or apply Dynamic Group first.
3.1. Properties
3.1.1. Attribute Properties


Default Label:
You can change the name for attributes, the names of these attributes will be displayed in the Catalog> Product section, edit a product. For example: Dynamic Group, ...
The required field must not be blank. Leave the "This is a required field" message blank.
Catalog Input Type for Store Owner: In this field, the default input type is Multiple Select.
Multiple Select: create a name for Dynamic Group in Manage Options (Values ​​of Your Attribute). If Simple Product satisfies each Dynamic group, then it will apply Stock Status with Dynamic group selected.
3.1.2. Advanced Attribute Properties
This section is similar to the Custom Stock Status section, you can configure the design of the display location of attributes. With the Attribute Code field and the Validation Input for Store Owner the default value.
With Manage Labels and Storefront Properties is exactly the same as the ones above we have guided.

3.2. Dynamic Quantity Groups Properties

In this section, selecting the Dynamic Group based on qty will apply the selected Stock Status if the field Enable Automatic Stock Status based on Dynamic Quantity Ranges at Configuration is enabled and Dynamic Group applies only to Simple Product.
For example, with Group Name Available, select Stock Status as Coming Soon2 (get Stock Status from the Custom Stock Status option you created above) with Quantity From = 0, Quantity To = 3. If the Simple product has Quantity within About on will be applied Dynamic Group
Note: When your product has a satisfactory Quantity to apply Dynamic Group, you must also consider that product meets the condition that you have configured at Configuration and you will apply Dynamic Group. If the product selects all Dynamic Group groups then the priority will be considered from top to bottom.

4. Edit Product
4.1. Edit Product
Login to the Magento Admin, choose Catalog> Products.
In the Edit product section, these two fields are added when installing the Custom Stock Status extension of Mageplaza. With the Option of these two fields, you have created options attributes in Manage Custom Stock Status and Manage Dynamic Groups


Note:
In case if both Custom Stock Status and Dynamic Groups to be selected, then priority will be given to Dynamic group first. If the product is not satisfied Dynamic group will continue to consider applying Custom Stock Status. And if you continue to Custom Custom Status, the default Stock Status will be applied by magento.
4.2. Product Grid
You can edit products for multiple products at the same time to save time. Go to Catalog> Products, on the product page select the products you want to edit the Custom Stock Status and select Actions> Update Attributes.



Attention
When you want to remove the extension, you should use composer to run the command: "bin / magento module: uninstall Mageplaza_ProductAlerts"
If you delete the extension manually, you need to delete the mp_dynamic_groups and mp_stock_status attributes in the database or in the backend.
Method 1: Go to the backend: From the Admin Panel, go to Stores> Attributes> Product. In the Attribute Code column, find the attribute mp_dynamic_groups and mp_stock_status, click and delete

Method 2: Go to the database to delete: Access to eav_attribute table. In the attribute_code column, you find and delete the attribute mp_dynamic_groups and mp_stock_status


Mageplaza Extension compatible
You can install some Mageplaza extensions, it is fully compatible with Custom Stock Status.
Product Slider: allows you to easily create many sliders such as featured products, bestselling products, new products, etc. If you install Product Slider products that apply Custom Stock Status on sliders with image or text or both.
Automatic Related Products: with this extension you can design for related products, can display on slider and display image and text of Custom Stock Status on that slider.
Who Viewed This Also Viewed: Customers are more likely to make a purchase decision when they see a product that other customers have seen. By smart algorithms, the most viewed products will be automatically updated and proposed to customers.
  
