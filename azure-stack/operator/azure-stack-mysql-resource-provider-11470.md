---
title: Azure Stack MySQL resource provider 1.1.47.0 release notes | Microsoft Docs
description: View the release notes to see what's new in the Azure Stack MySQL resource provider 1.1.47.0 update.
services: azure-stack
documentationcenter: ''
author: justinha
manager: femila
editor: ''

ms.assetid:  
ms.service: azure-stack
ms.workload: na
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: article
ms.date: 11/26/2019
ms.author: justinha
ms.reviewer: jiahan
ms.lastreviewed: 11/26/2019
---

# MySQL resource provider 1.1.47.0 release notes

*Applies to: Azure Stack integrated systems and Azure Stack Development Kit*

These release notes describe the improvements and known issues in MySQL resource provider version 1.1.47.0.

## Build reference
Download the MySQL resource provider binary and then run the self-extractor to extract the contents to a temporary directory. The resource provider has a minimum corresponding Azure Stack build. The minimum Azure Stack release version required to install this version of the MySQL resource provider is listed below:

> |Minimum Azure Stack version|MySQL resource provider version|
> |-----|-----|
> |Version 1808 (1.1808.0.97)|[MySQL RP version 1.1.33.0](https://aka.ms/azurestackmysqlrp11330)|  
> |     |     |

> [!IMPORTANT]
> Apply the minimum supported Azure Stack update to your Azure Stack integrated system or deploy the latest Azure Stack Development Kit (ASDK) before deploying the latest version of the MySQL resource provider.

## New features and fixes
This version of the Azure Stack MySQL resource provider includes the following improvements and fixes:

### Fixes

- **MySQL resource provider portal extension might choose the wrong subscription**. The MySQL resource provider uses Azure Resource Manager calls to determine the first service admin subscription to use, which might not be the *Default Provider Subscription*. If that happens, the MySQL resource provider doesn't work normally.

## Known issues

- **MySQL SKUs can take up to an hour to be visible in the portal**. It can take up to an hour for newly created SKUs to be visible for use when creating new MySQL databases. 

    **Workaround**: None.


### Known issues for Cloud Admins operating Azure Stack
Refer to the documentation in the [Azure Stack Release Notes](azure-stack-servicing-policy.md).

## Next steps
[Learn more about the MySQL resource provider](azure-stack-mysql-resource-provider.md).

[Prepare to deploy the MySQL resource provider](azure-stack-mysql-resource-provider-deploy.md#prerequisites).

[Upgrade the MySQL resource provider from a previous version](azure-stack-mysql-resource-provider-update.md). 