---
title: "Enable the Project Web App site collection features in Project Server 2016"
ms.author: efrene
author: efrene
manager: scotv
ms.date: 12/20/2016
ms.audience: ITPro
ms.topic: article
ms.prod: project-server-itpro
localization_priority: Normal
ms.collection:
- IT_ProjectAdmin
- IT_ProjectAdmin_Top
ms.assetid: b9c4dff2-4812-4131-8b20-4b7766d93233
description: "Summary: Enable the Project Web App site collection features to allow the import of SharePoint list projects into Project Web App."
---

# Enable the Project Web App site collection features in Project Server 2016
 
 **Summary:** Enable the Project Web App site collection features to allow the import of SharePoint list projects into Project Web App.<br/>
**Applies to:** Project Server 2016
  
Enabling the Project Web App site collection features adds additional functionality to the site collection that allows you to import SharePoint list projects into Project Web App.
  
## Enable the Project Web App site collection features
<a name="EnableTheProjectWebAppSiteCollectionFeatures"> </a>

The Project Web App site collection features are enabled by using the **Enable-SPFeature** PowerShell cmdlet. Use the following PowerShell script to enable the Project Web App site collection features.
  
```
Enable-SPFeature pwasite -URL SiteCollectionURL
```

For example:
  
```
Enable-SPFeature pwasite -URL http://contoso-appsrv1/sites/ContosoProjects

```

After the Project Web App site collection features have been activated for the site collection, you can add a Project Center web part and begin importing SharePoint list projects into Project Web App.
  
If you want to add a Project Web App site to the site collection, see [Create a PWA site in an existing site collection](create-a-pwa-site-in-an-existing-site-collection.md).
  
## See also
<a name="EnableTheProjectWebAppSiteCollectionFeatures"> </a>

#### 

[New-SPProjectDatabase](http://technet.microsoft.com/library/6eca666c-cbe8-41aa-94c5-4a8a3419fc96.aspx)
  
[Enable-SPFeature](http://technet.microsoft.com/library/9b68c192-b640-4cb8-8a92-a98008169b27.aspx)
  
[Get-SPWeb](http://technet.microsoft.com/library/9bf9284f-e3b9-439d-8a5f-74020e1eccaf.aspx)
  
[Project forums](https://social.technet.microsoft.com/Forums/en-US/category/project)

