---
title: tipo de recurso emailAppUsageAppsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d4dd1bc6a84b1d3e5f1b412986de686c9e6f5312
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979473"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="ada69-103">tipo de recurso emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="ada69-103">emailAppUsageAppsUserCounts resource type</span></span>

<span data-ttu-id="ada69-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ada69-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="ada69-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ada69-105">Properties</span></span>

| <span data-ttu-id="ada69-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ada69-106">Property</span></span>          | <span data-ttu-id="ada69-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ada69-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="ada69-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ada69-108">reportRefreshDate</span></span> | <span data-ttu-id="ada69-109">Data</span><span class="sxs-lookup"><span data-stu-id="ada69-109">Date</span></span>   |
| <span data-ttu-id="ada69-110">mailForMac</span><span class="sxs-lookup"><span data-stu-id="ada69-110">mailForMac</span></span>        | <span data-ttu-id="ada69-111">Int64</span><span class="sxs-lookup"><span data-stu-id="ada69-111">Int64</span></span>  |
| <span data-ttu-id="ada69-112">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="ada69-112">outlookForMac</span></span>     | <span data-ttu-id="ada69-113">Int64</span><span class="sxs-lookup"><span data-stu-id="ada69-113">Int64</span></span>  |
| <span data-ttu-id="ada69-114">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="ada69-114">outlookForWindows</span></span> | <span data-ttu-id="ada69-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ada69-115">Int64</span></span>  |
| <span data-ttu-id="ada69-116">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="ada69-116">outlookForMobile</span></span>  | <span data-ttu-id="ada69-117">Int64</span><span class="sxs-lookup"><span data-stu-id="ada69-117">Int64</span></span>  |
| <span data-ttu-id="ada69-118">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="ada69-118">otherForMobile</span></span>    | <span data-ttu-id="ada69-119">Int64</span><span class="sxs-lookup"><span data-stu-id="ada69-119">Int64</span></span>  |
| <span data-ttu-id="ada69-120">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="ada69-120">outlookForWeb</span></span>     | <span data-ttu-id="ada69-121">Int64</span><span class="sxs-lookup"><span data-stu-id="ada69-121">Int64</span></span>  |
| <span data-ttu-id="ada69-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="ada69-122">pop3App</span></span>           | <span data-ttu-id="ada69-123">Int64</span><span class="sxs-lookup"><span data-stu-id="ada69-123">Int64</span></span>  |
| <span data-ttu-id="ada69-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="ada69-124">imap4App</span></span>          | <span data-ttu-id="ada69-125">Int64</span><span class="sxs-lookup"><span data-stu-id="ada69-125">Int64</span></span>  |
| <span data-ttu-id="ada69-126">smtpApp</span><span class="sxs-lookup"><span data-stu-id="ada69-126">smtpApp</span></span>           | <span data-ttu-id="ada69-127">Int64</span><span class="sxs-lookup"><span data-stu-id="ada69-127">Int64</span></span>  |
| <span data-ttu-id="ada69-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ada69-128">reportPeriod</span></span>      | <span data-ttu-id="ada69-129">String</span><span class="sxs-lookup"><span data-stu-id="ada69-129">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ada69-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ada69-130">JSON representation</span></span>

<span data-ttu-id="ada69-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ada69-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageAppsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailForMac": 1024, 
  "outlookForMac": 1024, 
  "outlookForWindows": 1024, 
  "outlookForMobile": 1024, 
  "otherForMobile": 1024, 
  "outlookForWeb": 1024, 
  "pop3App": 1024, 
  "imap4App": 1024, 
  "smtpApp": 1024, 
  "reportPeriod": "String"
}
```


