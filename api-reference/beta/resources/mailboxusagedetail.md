---
title: tipo de recurso mailboxUsageDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 63b4b997a0ae559338fffd2acfabaa35dcc306e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581265"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="52578-103">tipo de recurso mailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="52578-103">mailboxUsageDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="52578-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52578-104">Properties</span></span>

| <span data-ttu-id="52578-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52578-105">Property</span></span>                        | <span data-ttu-id="52578-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="52578-106">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="52578-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="52578-107">reportRefreshDate</span></span>               | <span data-ttu-id="52578-108">Data</span><span class="sxs-lookup"><span data-stu-id="52578-108">Date</span></span>    |
| <span data-ttu-id="52578-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="52578-109">userPrincipalName</span></span>               | <span data-ttu-id="52578-110">String</span><span class="sxs-lookup"><span data-stu-id="52578-110">String</span></span>  |
| <span data-ttu-id="52578-111">displayName</span><span class="sxs-lookup"><span data-stu-id="52578-111">displayName</span></span>                     | <span data-ttu-id="52578-112">String</span><span class="sxs-lookup"><span data-stu-id="52578-112">String</span></span>  |
| <span data-ttu-id="52578-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="52578-113">isDeleted</span></span>                       | <span data-ttu-id="52578-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="52578-114">Boolean</span></span> |
| <span data-ttu-id="52578-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="52578-115">deletedDate</span></span>                     | <span data-ttu-id="52578-116">Data</span><span class="sxs-lookup"><span data-stu-id="52578-116">Date</span></span>    |
| <span data-ttu-id="52578-117">createdDate</span><span class="sxs-lookup"><span data-stu-id="52578-117">createdDate</span></span>                     | <span data-ttu-id="52578-118">Data</span><span class="sxs-lookup"><span data-stu-id="52578-118">Date</span></span>    |
| <span data-ttu-id="52578-119">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="52578-119">lastActivityDate</span></span>                | <span data-ttu-id="52578-120">Data</span><span class="sxs-lookup"><span data-stu-id="52578-120">Date</span></span>    |
| <span data-ttu-id="52578-121">itemCount</span><span class="sxs-lookup"><span data-stu-id="52578-121">itemCount</span></span>                       | <span data-ttu-id="52578-122">Int64</span><span class="sxs-lookup"><span data-stu-id="52578-122">Int64</span></span>   |
| <span data-ttu-id="52578-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="52578-123">storageUsedInBytes</span></span>              | <span data-ttu-id="52578-124">Int64</span><span class="sxs-lookup"><span data-stu-id="52578-124">Int64</span></span>   |
| <span data-ttu-id="52578-125">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="52578-125">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="52578-126">Int64</span><span class="sxs-lookup"><span data-stu-id="52578-126">Int64</span></span>   |
| <span data-ttu-id="52578-127">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="52578-127">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="52578-128">Int64</span><span class="sxs-lookup"><span data-stu-id="52578-128">Int64</span></span>   |
| <span data-ttu-id="52578-129">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="52578-129">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="52578-130">Int64</span><span class="sxs-lookup"><span data-stu-id="52578-130">Int64</span></span>   |
| <span data-ttu-id="52578-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="52578-131">reportPeriod</span></span>                    | <span data-ttu-id="52578-132">String</span><span class="sxs-lookup"><span data-stu-id="52578-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="52578-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52578-133">JSON representation</span></span>

<span data-ttu-id="52578-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52578-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "createdDate": "Date", 
  "lastActivityDate": "Date", 
  "itemCount": 1024, 
  "storageUsedInBytes": 1024, 
  "issueWarningQuotaInBytes": 1024, 
  "prohibitSendQuotaInBytes": 1024, 
  "prohibitSendReceiveQuotaInBytes": 1024, 
  "reportPeriod": "String"
}
```
