---
title: "Close an opportunity as won or lost (Dynamics 365 for Sales) | MicrosoftDocs"
description: "Close the opportunity to indicate whether it was won or lost."
keywords: "Close, Won, Lost, opportunity, proposal"
ms.date: 04/12/2019
ms.service: dynamics-365-sales
ms.custom: dyn365-sales
ms.topic: article
applies_to: Dynamics 365 for Customer Engagement
ms.assetid: be3ff5e6-019b-4c07-aebb-e5792af19b4d
author: shubhadaj
ms.author: shujoshi
manager: annbe
ms.reviewer: 
ms.suite: 
ms.tgt_pltfrm: 
caps.latest.revision: 13
---

# Close an opportunity as won or lost (Sales and Sales Hub)

If your customer has accepted your proposal, congratulations! However, whether your customer accepted or declined your proposal, it's now time to close that opportunity.  
  
1. If you're using the Sales Hub app, in the site map, select **Opportunities**. 
   
   OR

   In the Sales module, go to **Sales** > **Opportunities**.
  
2. Open the opportunity you want to edit.  
  
3. At the top of the **Opportunity** form, do one of the following:  

   - To close your opportunity as won, select **Close as Won**.  
 
   - To close your opportunity as lost, select **Close as Lost**.

      ![Close as Won and Close as Lost options on the Opportunity form](media/close-opportunity.png "Close as Won and Close as Lost options on the Opportunity form")

4. When you close the opportunity as **Won**, in the **Close Opportunity** dialog box, do the following, and select **OK**:

    - In **Actual Revenue**, Verify the amount, and make changes, if necessary.
    
    - In **Description**, enter details about what contributed to winning this opportunity. 

      ![Close Opportunity dialog box when the opportunity is won](media/close-as-won.png "Close Opportunity dialog box when the opportunity is won")

    When you close the opportunity as **Lost**, in the **Close Opportunity** dialog box, do the following, and select **OK**:
  
    -  In **Competitor**, select a competitor you lost this opportunity to.
    
    -  In **Description**, add more details around why the opportunity was lost.

        ![Close Opportunity dialog box when the opportunity is lost](media/close-as-lost.png "Close Opportunity dialog box when the opportunity is lost")

    > [!IMPORTANT]
    > - If your system administrator has enabled custom fields on the Opportunity Close form, you may be required to fill in data in other fields as defined by your organization. The capability to enable custom fields on the Opportunity Close form is in preview.  [What are Preview features and how do I enable them?](../admin/what-are-preview-features-how-do-i-enable-them.md). 
    > - To learn about enabling preview features in the 2019 release wave 2, see [How do I enable the 2019 release wave 2 updates](/power-platform/admin/preview-october-2019-updates#when-will-the-2019-release-wave-2-features-be-enabled)


For information on how to resolve the common errors that you may see while closing an opportunity, see the [troubleshooting guide](troubleshooting.md).

## Reopen a closed opportunity

If you've closed an opportunity as lost, but would like to start discussions about a potential sale, you may want to reopen a closed opportunity.

1. If you're using the Sales Hub app, in the site map, select **Opportunities**. 
   
   OR

    In the Sales module, go to **Sales** > **Opportunities**.

2. To see all the closed opportunities, in the view selector, select the **Closed Opportunities** view.  

    ![Closed Opportunities view in the view selector](media/select-closed-opportunities-view.png "Closed Opportunities view in the view selector")

3. Select the opportunity that you want to repoen, and on the command bar, select **Reopen Opportunity**. The reopened opportunities start appearing in the open opportunities list.
  
### See also  
 [Nurture sales from lead to order](../sales-enterprise/nurture-sales-from-lead-order-sales.md)   
 [Print leads, quotes, and other records](../basics/print-leads-quotes-other-records.md)  
 [Dynamics 365 for Sales troubleshooting guide for administrators](troubleshooting-admin.md)  
