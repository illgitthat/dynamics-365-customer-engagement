---
title: "Generate segments based on customer journey results (Dynamics 365 for Marketing) | Microsoft Docs"
description: "Explains how to automatically generate an interaction segment that finds all contacts who did a particular thing during a specific customer journey"
keywords:
ms.date: 06/07/2019
ms.service: dynamics-365-marketing
ms.custom: 
  - dyn365-marketing
ms.topic: get-started-article
applies_to: 
  - Dynamics 365 for Customer Engagement (online)
ms.assetid: 901bf6af-5884-46ae-9852-1acb2bb19cd9
author: kamaybac
ms.author: kamaybac
manager: shellyha
ms.reviewer:
topic-status: Drafting
search.audienceType: 
  - admin
  - customizer
  - enduser
search.app: 
  - D365CE
  - D365Mktg
---

# Generate dynamic interaction segments from customer journey results

After going live with a customer journey, you'll be able to [monitor the progress of contacts](insights.md#journey-insights) through the journey pipeline. You can use many of these results to automatically generate [interaction segments](segments-interaction.md) that find all contacts that are being counted by a given result. This provides a handy way to find all contacts that did certain things in a particular journey. Because interaction segments are dynamic, they will continue to grow as the journey processes more contacts.

> [!TIP]
> You might use this to split long, complex journeys into shorter, easier to manage journeys. For example, you might create a standard demographic segment to target the initial journey, and then create auto-generated segments that find contacts that ended on a particular tile or did a particular thing in that journey. Finally, you'd create follow-up journeys that target the appropriate segments that were auto-generated based on what each contact did on the initial journey.

To generate a dynamic segment from customer journey results:

1. Go to **Marketing** > **Marketing execution** > **Customer journeys** and open a journey from the list. The journey must already be live for the required data to be available.

1. Select a tile from the journey pipeline and inspect the **Data** panel, which shows how many contacts that tile has processed and, sometimes, more other information about what they did there. Here’s the **Data** panel for an email tile:

    ![Data panel for an email tile](media/customer-journey-data-panel.png "Data panel for an email tile")

1. Identify the type of information you'd like to use in your new segment and select the floppy-disk button ![Save-as-segment button](media/floppy-disk-button.png "Save-as-segment button")  for that value. For example:
    - **Processed**: Nearly all types of tiles provide this value and a floppy-disk button for it. This will find all contacts who were successfully processed by this tile in this journey.
    - **Unique clicks**: This is only shown for email tiles. This will find all contacts that clicked on this email when sent by this journey.
    - **Hard bounces**: This is only shown for email tiles. This will find all contacts that produced a hard bounce after this email was sent by this journey.

1. A quick-create flyout slides in from the side of the screen. Use it to assign a **Name** and **Description** of the segment you are creating.

1. Select **Save and Close** at the bottom of the quick-create flyout to create the segment. You'll now be able to find it under **Marketing** > **Customers** > **Segments**. If you're fast, you can open the new segment right away by selecting **View record** in the pop-up announcement.

    ![Changes saved pop-up announcement](media/popup-changes-saved.png "Changes saved pop-up announcement")

> [!NOTE]
> The segments you create using this procedure are initially saved in the draft state. You must [go live](go-live.md) with each segment before you can use it to target a journey.

> [!TIP]
> You'll be able to see and edit the full logic for each segment created in this way, so you can also use this technique to get started creating custom segments, or to learn how to create segmentation logic for use in other contexts.

### See also

[Design interaction-based dynamic segments](segments-interaction.md)  
[Use customer journeys to create automated campaigns](customer-journeys-create-automated-campaigns.md)  
[Analyze results to gain insights from your marketing activities](insights.md)
