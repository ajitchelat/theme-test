<properties
	pageTitle="Microsoft Azure Subscription and Service Limits, Quotas, and Constraints"
	description="Provides a list of common Azure subscription and service limits, quotas, and constraints. This includes information on how to increase limits along with maximum values."
	services=""
	documentationCenter=""
	authors="rothja"
	manager="jeffreyg"
	editor=""
	tags="billing"
	/>

<tags
	ms.service="billing"
	ms.workload="na"
	ms.tgt_pltfrm="na"
	ms.devlang="na"
	ms.topic="article"
	ms.date="08/18/2016"
	ms.author="btardif"/>

# Azure subscription and service limits, quotas, and constraints

## Overview

This document specifies some of the most common Microsoft Azure limits. This does not currently cover all Azure services. Over time, these limits will be expanded and updated to cover more of the platform.

> [AZURE.NOTE] If you want to raise the limit above the **Default Limit**, you can [open an online customer support request at no charge](https://azure.microsoft.com/blog/2014/06/04/azure-limits-quotas-increase-requests/). The limits cannot be raised above the **Maximum Limit** value in the tables below. If there is no **Maximum Limit** column, then the specified resource does not have adjustable limits.

## Limits and the Azure Resource Manager

It is now possible to combine multiple Azure resources in to a single Azure Resource Group. When using Resource Groups, limits that once were global become managed at a regional level with the Azure Resource Manager. For more information about Azure Resource Groups, see [Azure Resource Manager overview]().

In the limits below, a new table has been added to reflect any differences in limits when using the Azure Resource Manager. For example, there is a **Subscription Limits** table and a **Subscription Limits - Azure Resource Manager** table. When a limit applies to both scenarios, it is only shown in the first table. Unless otherwise indicated, limits are global across all regions.

> [AZURE.NOTE] It is important to emphasize that quotas for resources in Azure Resource Groups are per-region accessible by your subscription, and are not per-subscription, as the service management quotas are. Let's use core quotas as an example. If you need to request a quota increase with support for cores, you need to decide how many cores you want to use in which regions, and then make a specific request for Azure Resource Group core quotas for the amounts and regions that you want. Therefore, if you need to use 30 cores in West Europe to run your application there; you should specifically request 30 cores in West Europe. But you will not have a core quota increase in any other region -- only West Europe will have the 30-core quota.
<!-- -->
As a result, you may find it useful to consider deciding what your Azure Resource Group quotas need to be for your workload in any one region, and request that amount in each region into which you are considering deployment. See [troubleshooting deployment issues]() for more help discovering your current quotas for specific regions.


## Service-specific limits

- [Active Directory]()
- [API Management]()
- [App Service]()
- [Application Insights]()
- [Automation]()
- [Azure Redis Cache]()
- [Azure RemoteApp]()
- [Backup]()
- [Batch]()
- [BizTalk Services]()
- [CDN]()
- [Cloud Services]()
- [Data Factory]()
- [Data Lake Analytics]()
- [DNS]()
- [DocumentDB]()
- [Event Hubs]()
- [IoT Hub]()
- [Key Vault]()
- [Media Services]()
- [Mobile Engagement]()
- [Mobile Services]()
- [Multi-Factor Authentication]()
- [Networking]()
- [Notification Hub Service]()
- [Operational Insights]()
- [Resource Group]()
- [Scheduler]()
- [Search]()
- [Service Bus]()
- [Site Recovery]()
- [SQL Database]()
- [Storage]()
- [StorSimple System]()
- [Stream Analytics]()
- [Subscription]()
- [Traffic Manager]()
- [Virtual Machines]()
- [Virtual Machine Scale Sets]()


### Subscription limits
#### Subscription limits
[AZURE.INCLUDE [azure-subscription-limits]()]

#### Subscription limits - Azure Resource Manager

The following limits apply when using the Azure Resource Manager and Azure Resource Groups. Limits that have not changed with the Azure Resource Manager are not listed below. Please refer to the previous table for those limits.

[AZURE.INCLUDE [azure-subscription-limits-azure-resource-manager]()]


### Resource Group limits

[AZURE.INCLUDE [azure-resource-groups-limits]()]

### Virtual Machines limits
#### Virtual Machine limits
[AZURE.INCLUDE [azure-virtual-machines-limits]()]


#### Virtual Machines limits - Azure Resource Manager

The following limits apply when using the Azure Resource Manager and Azure Resource Groups. Limits that have not changed with the Azure Resource Manager are not listed below. Please refer to the previous table for those limits.

[AZURE.INCLUDE [azure-virtual-machines-limits-azure-resource-manager]()]

### Virtual Machine Scale Sets limits

[AZURE.INCLUDE [virtual-machine-scale-sets-limits]()]

### Networking limits

[AZURE.INCLUDE [expressroute-limits]()]

#### Networking limits
[AZURE.INCLUDE [azure-virtual-network-limits]()]

#### Traffic Manager limits

[AZURE.INCLUDE [traffic-manager-limits]()]

#### DNS limits

[AZURE.INCLUDE [dns-limits]()]

### Storage limits

For additional details on storage account limits, see [Azure Storage Scalability and Performance Targets]()).

#### Storage Service limits

[AZURE.INCLUDE [azure-storage-limits]()]

#### Virtual Machine disk limits

[AZURE.INCLUDE [azure-storage-limits-vm-disks]()]

See [Virtual machine sizes]() for additional details.

**Standard storage accounts**

[AZURE.INCLUDE [azure-storage-limits-vm-disks-standard]()]

**Premium storage accounts**

[AZURE.INCLUDE [azure-storage-limits-vm-disks-premium]()]

#### Storage Resource Provider limits

[AZURE.INCLUDE [azure-storage-limits-azure-resource-manager]()]


### Cloud Services limits

[AZURE.INCLUDE [azure-cloud-services-limits]()]


### App Service limits
The following App Service limits include limits for Web Apps, Mobile Apps, API Apps, and Logic Apps.

[AZURE.INCLUDE [azure-websites-limits]()]

### Scheduler limits

[AZURE.INCLUDE [scheduler-limits-table]()]

### Batch limits

[AZURE.INCLUDE [azure-batch-limits]())]

###BizTalk Services limits
The following table shows the limits for Azure Biztalk Services.

[AZURE.INCLUDE [biztalk-services-service-limits]()]


### DocumentDB limits

[AZURE.INCLUDE [azure-documentdb-limits]()]

Quotas listed with an asterisk (*) [can be adjusted by contacting Azure support]().

### Mobile Engagement limits

[AZURE.INCLUDE [azure-mobile-engagement-limits]()]


### Search limits

Pricing tiers determine the capacity and limits of your search service. Tiers include:

- *Free* multi-tenant service, shared with other Azure subscribers, intended for evaluation and small development projects.
- *Basic* provides dedicated computing resources for production workloads at a smaller scale, with up to three replicas for highly available query workloads.
- *Standard (S1, S2, S3, S3 High Density)* is for larger production workloads. Multiple levels exist within the standard tier so that you can choose a resource configuration for specific scenarios.

**Limits per subscription**

[AZURE.INCLUDE [azure-search-limits-per-subscription]()]

**Limits per search service**

[AZURE.INCLUDE [azure-search-limits-per-service]()]

For more granular information about other limits, including document size, queries per second, keys, requests, and responses, see [Service limits in Azure Search]().

### Media Services limits

[AZURE.INCLUDE [azure-mediaservices-limits]()]

### CDN limits

[AZURE.INCLUDE [cdn-limits]()]

### Mobile Services limits

[AZURE.INCLUDE [mobile-services-limits]()]

### Notification Hub Service limits

[AZURE.INCLUDE [notification-hub-limits]()]

### Event Hubs limits

[AZURE.INCLUDE [azure-servicebus-limits]()]

### Service Bus limits

[AZURE.INCLUDE [azure-servicebus-limits]()]

### IoT Hub limits

[AZURE.INCLUDE [azure-iothub-limits]()]

### Data Factory limits

[AZURE.INCLUDE [azure-data-factory-limits]()]

### Data Lake Analytics Limits
[AZURE.INCLUDE [azure-data-lake-analytics-limits]()]

### Stream Analytics limits
[AZURE.INCLUDE [stream-analytics-limits-table]()]

### Active Directory limits

[AZURE.INCLUDE [AAD-service-limits]()]


### Azure RemoteApp limits

[AZURE.INCLUDE [azure-remoteapp-limits]()]

### StorSimple System limits

[AZURE.INCLUDE [storsimple-limits-table]()]


### Operational Insights limits

[AZURE.INCLUDE [operational-insights-limits]()]

### Backup limits

[AZURE.INCLUDE [azure-backup-limits]()]

### Site Recovery limits

[AZURE.INCLUDE [site-recovery-limits]()]

### Application Insights limits

[AZURE.INCLUDE [application-insights-limits]()]

### API Management limits

[AZURE.INCLUDE [api-management-service-limits]()]

### Azure Redis Cache limits

[AZURE.INCLUDE [redis-cache-service-limits]()]

### Key Vault limits

[AZURE.INCLUDE [key-vault-limits]()]

### Multi-Factor Authentication
[AZURE.INCLUDE [azure-mfa-service-limits]())]

### Automation limits
[AZURE.INCLUDE [automation-limits]()]

### SQL Database limits

For SQL Database limits, see [SQL Database Resource Limits]().

## See also

[Understanding Azure Limits and Increases](https://azure.microsoft.com/blog/2014/06/04/azure-limits-quotas-increase-requests/)

[Virtual Machine and Cloud Service Sizes for Azure]()

[Sizes for Cloud Services]()
