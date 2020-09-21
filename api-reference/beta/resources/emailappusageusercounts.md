---
title: tipo de recurso emailAppUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 29f8e9b4ae1a559415bcd826aa1507836492d99a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979438"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="3f959-103">tipo de recurso emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="3f959-103">emailAppUsageUserCounts resource type</span></span>

<span data-ttu-id="3f959-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f959-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="3f959-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f959-105">Properties</span></span>

| <span data-ttu-id="3f959-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f959-106">Property</span></span>          | <span data-ttu-id="3f959-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f959-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="3f959-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3f959-108">reportRefreshDate</span></span> | <span data-ttu-id="3f959-109">Data</span><span class="sxs-lookup"><span data-stu-id="3f959-109">Date</span></span>   |
| <span data-ttu-id="3f959-110">mailForMac</span><span class="sxs-lookup"><span data-stu-id="3f959-110">mailForMac</span></span>        | <span data-ttu-id="3f959-111">Int64</span><span class="sxs-lookup"><span data-stu-id="3f959-111">Int64</span></span>  |
| <span data-ttu-id="3f959-112">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="3f959-112">outlookForMac</span></span>     | <span data-ttu-id="3f959-113">Int64</span><span class="sxs-lookup"><span data-stu-id="3f959-113">Int64</span></span>  |
| <span data-ttu-id="3f959-114">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="3f959-114">outlookForWindows</span></span> | <span data-ttu-id="3f959-115">Int64</span><span class="sxs-lookup"><span data-stu-id="3f959-115">Int64</span></span>  |
| <span data-ttu-id="3f959-116">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="3f959-116">outlookForMobile</span></span>  | <span data-ttu-id="3f959-117">Int64</span><span class="sxs-lookup"><span data-stu-id="3f959-117">Int64</span></span>  |
| <span data-ttu-id="3f959-118">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="3f959-118">otherForMobile</span></span>    | <span data-ttu-id="3f959-119">Int64</span><span class="sxs-lookup"><span data-stu-id="3f959-119">Int64</span></span>  |
| <span data-ttu-id="3f959-120">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="3f959-120">outlookForWeb</span></span>     | <span data-ttu-id="3f959-121">Int64</span><span class="sxs-lookup"><span data-stu-id="3f959-121">Int64</span></span>  |
| <span data-ttu-id="3f959-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="3f959-122">pop3App</span></span>           | <span data-ttu-id="3f959-123">Int64</span><span class="sxs-lookup"><span data-stu-id="3f959-123">Int64</span></span>  |
| <span data-ttu-id="3f959-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="3f959-124">imap4App</span></span>          | <span data-ttu-id="3f959-125">Int64</span><span class="sxs-lookup"><span data-stu-id="3f959-125">Int64</span></span>  |
| <span data-ttu-id="3f959-126">smtpApp</span><span class="sxs-lookup"><span data-stu-id="3f959-126">smtpApp</span></span>           | <span data-ttu-id="3f959-127">Int64</span><span class="sxs-lookup"><span data-stu-id="3f959-127">Int64</span></span>  |
| <span data-ttu-id="3f959-128">reportDate</span><span class="sxs-lookup"><span data-stu-id="3f959-128">reportDate</span></span>        | <span data-ttu-id="3f959-129">Data</span><span class="sxs-lookup"><span data-stu-id="3f959-129">Date</span></span>   |
| <span data-ttu-id="3f959-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3f959-130">reportPeriod</span></span>      | <span data-ttu-id="3f959-131">String</span><span class="sxs-lookup"><span data-stu-id="3f959-131">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3f959-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f959-132">JSON representation</span></span>

<span data-ttu-id="3f959-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f959-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
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
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


