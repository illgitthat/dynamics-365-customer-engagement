---
title: "Detect duplicate data for Dynamics 365 for Customer Engagement apps | MicrosoftDocs"
ms.custom: 
ms.date: 09/30/2017
ms.reviewer: 
ms.service: crm-online
ms.suite: 
ms.tgt_pltfrm: 
ms.topic: article
applies_to: 
  - Dynamics 365 for Customer Engagement  (online)
  - Dynamics 365 for Customer Engagement  Version 9.x
author: jimholtz
ms.assetid: 4bfccb7c-c29d-4a33-900e-3b3665fa4cf4
caps.latest.revision: 34
ms.author: jimholtz
manager: kvivek
search.audienceType: 
  - admin
search.app: 
  - D365CE
  - Powerplatform
---
# Detect duplicate data so you can fix or remove it

*This content also applies to the on-premises version.*

To determine whether a record is a potential duplicate, [!INCLUDE[pn_microsoftcrm](../includes/pn-dynamics-crm.md)] apps uses duplicate detection rules. When publishing a duplicate detection rule, a matchcode is created for each existing record. A matchcode is also created when a record is created or updated. When a record is in the process of being created or updated, its matchcode can be checked automatically against the matchcodes of existing records. By default, [!INCLUDE[pn_microsoftcrm](../includes/pn-dynamics-crm.md)] apps has simple duplicate detection rules for accounts, contacts, and leads. For example, you detect duplicates by matching the record fields, such as email address, first name, and last name.  
  
 Duplicate detection works by comparing generated match codes of existing records with each new record being created. These match codes are created as each new record is created. Therefore, there is potential for one or more duplicate records to be created if they are processed at the exact same moment. In addition to detecting duplicates as they are created, you should schedule duplicate detection jobs to check for other potential duplicate records.  
  
> [!NOTE]
>  Duplicate detection works with [!INCLUDE[pn_moca_full](../includes/pn-moca-full.md)], but isn't available for [!INCLUDE[pn_Mobile_Express_short](../includes/pn-mobile-express-short.md)].  
> 
> [!IMPORTANT]
>  You have to be a system administrator or a system customizer to create, enable, and publish duplicate detection rules for your organization.  
> 
>  After publishing a duplicate detection rule, increasing the length of fields that are included in the duplicate detection criteria goes undetected. The field length could exceed the matchcode length limit and not be verified. This may result in duplicates not being detected.  
> 
>  You can create multiple detection rules for the same entity type. However, you can publish a maximum of five duplicate detection rules per entity type at one time.  
  
 You can detect duplicates:  
  
- When you create or update records for entities that enabled for duplicate detection. This includes records created with [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)] and tracked in [!INCLUDE[pn_microsoftcrm](../includes/pn-dynamics-crm.md)] apps web application. The duplicate detection dialog is only displayed for the records created or updated in the [!INCLUDE [pn-crm-shortest](../includes/pn-crm-shortest.md)] apps user interface (UI). For example, for records created by a workflow, the duplicate detection dialog is not displayed.  
  
  > [!NOTE]
  > [!INCLUDE[pn_microsoftcrm](../includes/pn-dynamics-crm.md)] apps has the ability to detect duplicates for the updated UI entities when you create or update records using entity forms or grid views in the [!INCLUDE [pn-crm-shortest](../includes/pn-crm-shortest.md)] apps web application.  
  
- When [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)] goes from offline to online.  
  
- During data import. You can specify whether or not to check for duplicates during the import.  
  
  > [!NOTE]
  >  Duplicates can’t be detected when a user merges two records, converts a lead, or saves an activity as completed. Duplicates also aren’t detected when a user changes the status of a record, such as activating or reactivating it.  
  
To check for duplicates in the web application, you can use **Detect Duplicates** capability provided in **More Commands** (![More commands button](../admin/media/not-available.gif "More commands button")) on the nav bar in the grid. The duplicate records are also detected when you import data programmatically or through Import Data Wizard. In addition, you can check for duplicates by running scheduled duplicate detection jobs. For step-by-step instructions on how to set up the duplicate detection job, see [Run system jobs to detect duplicates](run-bulk-system-jobs-detect-duplicate-records.md).  
  
A duplicate detection job runs in the background while you do other things in [!INCLUDE[pn_microsoftcrm](../includes/pn-dynamics-crm.md)] apps . You can request email notification from [!INCLUDE [pn-crm-shortest](../includes/pn-crm-shortest.md)] apps upon the completion of a duplicate detection job.  
  
### See also  
 [Import data (all record types)](../admin/import-data-all-record-types.md)   
 [Check for duplicates](set-up-duplicate-detection-rules-keep-data-clean.md)   
 [Set up duplicate detection rules](set-up-duplicate-detection-rules-keep-data-clean.md)   
 [Run system jobs to detect duplicates](run-bulk-system-jobs-detect-duplicate-records.md)   
 [Delete bulk records](../admin/delete-bulk-records.md)
