---
title: "Add products an opportunity (Dynamics 365 for Sales) | MicrosoftDocs"
description: "Develop your opportunity by defining the products your customers are interested in purchasing."
keywords: "opportunity, deal, develop, propose, nurture sales"
ms.date: 08/01/2019
ms.service: dynamics-365-sales
ms.custom: dyn365-sales
ms.topic: article
applies_to: Dynamics 365 for Customer Engagement
ms.assetid: 36b834d9-7b37-49f7-a110-efcaee8dea04
author: shubhadaj
ms.author: shujoshi
manager: annbe
ms.reviewer: 
ms.suite: 
ms.tgt_pltfrm: 
caps.latest.revision: 58
---

# Add products to an opportunity (Sales Hub)

A way that might help you increase your sales is to add all products that your customer might need. You can add product bundles or product families to make it easier for you to choose products for upsell and cross-sell. The product can be an existing product in the [!INCLUDE[pn-dyn-365-sales](../includes/pn-dyn-365-sales.md)] product catalog or an ad hoc product that you add as a write-in product. Any products added to an opportunity are automatically associated with quotes generated from the opportunity.


1. From the list of opportunities, open the opportunity to which you want to add products.

2. Go to the **Product Line Items** tab.

3. Select a **Price List**. The price list determines the cost of the product. 
  
    > [!NOTE]
    > By default, selecting a price list is required to be able to add products to an opportunity; however, your administrator can change your organization settings to make the Price List field optional.The capability to make the Price List field optional is in preview. To learn about enabling preview features in the 2019 release wave 2, see [How do I enable the 2019 release wave 2 updates](/power-platform/admin/preview-october-2019-updates#when-will-the-2019-release-wave-2-features-be-enabled)

4. If you want the estimated revenue of the opportunity to be calculated based on the total amount of products, set **Revenue** to **System Calculated**. If you want to use a custom estimated revenue, set it to **User Provided**.

5. In the **Product Line Items** grid, select **Add New Opportunity Product**.

6. In the **New Opportunity Product** form, do the following:  

    1.  **Select Product**: Set the switch to choose whether you want to add an existing product or create a new one:
    
        -  To use an existing product, select **Lookup** to search for and add a product.

            
            > [!NOTE]
            > - When a price list is selected for the opportunity, the products listed in the **Existing Product** field are filtered by the price list. This means that only the product associated with the selected price list are shown in this field. 
            > - When a price list isn't selected, the **Existing product** field shows all active products (not filtered by the price list). You can change the view to look for other products by selecting the **Change View** icon. 
            > - By default, the product lookup will show the most recently used products. The most recently used products are not filtered based on the selected price list. 
            > - If a price list is selected, and you select a product that isn’t associated with the price list, you'll see an error. Select a product that's associated with the selected price list.

            > [!IMPORTANT]
            > The capability to make the selection of a price list optional is a preview feature. [What are Preview features and how do I enable them?](../admin/what-are-preview-features-how-do-i-enable-them.md)


        -  To create a product, select **Write-In**, and then enter the name of the product.
    
    2.  **Pricing**: Select the pricing option. By default, this is the per unit price that is listed in the product catalog. To override the catalog price, select **Override Price**: When you override the price, you can specify a price that you want to charge for each unit of the product.   

    3.  **Quantity**: Enter the quantity of the product or service that will be included.  

    4.  **Manual Discount**: If you want to offer a discount to the product price, enter it here.  
    
    5.  **Tax**: If required, enter the appropriate tax amount.  
   
7. To save this product, and add more products, select **Save and New**.

The **Product Line Items** grid shows all the products that are associated with the opportunity. If you added an existing product from the product catalog, you can change the quantity and discount of the product inline in the **Product Line Items** grid. If you added a write-in product, you can also change the price of the product in addition to the quantity and discount.

The icon for each product line item shows whether it is a product, product bundle, or a product family. 

Here are the actions you can take on the products added to the **Product Line Items** grid:

|To                                    |Do This                                                       |
|--------------------------------------|--------------------------------------------------------------|
|Edit properties of a product  |Select a product, and on the command bar, select **Edit Properties**. You can change details, such as the price, quantity, or discount of the added products. <br/> You can also open the opportunity product record and view or change the properties of the product inline on the **Product Properties** tab. |
|Delete a product associated with the opportunity |Select the product, and on the command bar, select **Delete Opportunity Product**. |
|View products within a bundle | Select the **Chevron** icon ![Chevron icon](media/chevron-icon.png "Chevron icon") for the product bundle. You’ll see all the products that are included in the bundle. |
|See and add related products for cross-selling or upselling or to select an accessory or substitute product | Select a product, and on the command bar, select **Suggestions**. The Suggestions pane shows all the products that are defined as related products for the current product. Select the related products that you want to add, and then select **OK**. |
|See specific records together by moving a record up or down in the grid | Select a record, and on the command bar, use the **Up** or **Down** button. |


### See also  

[Create or edit an opportunity](../sales-enterprise/create-edit-opportunity-sales.md)  
[Nurture sales from lead to order](../sales-enterprise/nurture-sales-from-lead-order-sales.md)   
[Print leads, quotes, and other records](../basics/print-leads-quotes-other-records.md)  
[Dynamics 365 for Sales troubleshooting guide for administrators](troubleshooting-admin.md)  
