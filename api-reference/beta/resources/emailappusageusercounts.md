---
title: tipo de recurso emailAppUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 18ce0629bbb2a700d873587de6d3e5244304bcb0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499488"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="934b9-103">tipo de recurso emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="934b9-103">emailAppUsageUserCounts resource type</span></span>

<span data-ttu-id="934b9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="934b9-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="934b9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="934b9-105">Properties</span></span>

| <span data-ttu-id="934b9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="934b9-106">Property</span></span>          | <span data-ttu-id="934b9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="934b9-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="934b9-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="934b9-108">reportRefreshDate</span></span> | <span data-ttu-id="934b9-109">Data</span><span class="sxs-lookup"><span data-stu-id="934b9-109">Date</span></span>   |
| <span data-ttu-id="934b9-110">mailForMac</span><span class="sxs-lookup"><span data-stu-id="934b9-110">mailForMac</span></span>        | <span data-ttu-id="934b9-111">Int64</span><span class="sxs-lookup"><span data-stu-id="934b9-111">Int64</span></span>  |
| <span data-ttu-id="934b9-112">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="934b9-112">outlookForMac</span></span>     | <span data-ttu-id="934b9-113">Int64</span><span class="sxs-lookup"><span data-stu-id="934b9-113">Int64</span></span>  |
| <span data-ttu-id="934b9-114">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="934b9-114">outlookForWindows</span></span> | <span data-ttu-id="934b9-115">Int64</span><span class="sxs-lookup"><span data-stu-id="934b9-115">Int64</span></span>  |
| <span data-ttu-id="934b9-116">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="934b9-116">outlookForMobile</span></span>  | <span data-ttu-id="934b9-117">Int64</span><span class="sxs-lookup"><span data-stu-id="934b9-117">Int64</span></span>  |
| <span data-ttu-id="934b9-118">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="934b9-118">otherForMobile</span></span>    | <span data-ttu-id="934b9-119">Int64</span><span class="sxs-lookup"><span data-stu-id="934b9-119">Int64</span></span>  |
| <span data-ttu-id="934b9-120">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="934b9-120">outlookForWeb</span></span>     | <span data-ttu-id="934b9-121">Int64</span><span class="sxs-lookup"><span data-stu-id="934b9-121">Int64</span></span>  |
| <span data-ttu-id="934b9-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="934b9-122">pop3App</span></span>           | <span data-ttu-id="934b9-123">Int64</span><span class="sxs-lookup"><span data-stu-id="934b9-123">Int64</span></span>  |
| <span data-ttu-id="934b9-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="934b9-124">imap4App</span></span>          | <span data-ttu-id="934b9-125">Int64</span><span class="sxs-lookup"><span data-stu-id="934b9-125">Int64</span></span>  |
| <span data-ttu-id="934b9-126">smtpApp</span><span class="sxs-lookup"><span data-stu-id="934b9-126">smtpApp</span></span>           | <span data-ttu-id="934b9-127">Int64</span><span class="sxs-lookup"><span data-stu-id="934b9-127">Int64</span></span>  |
| <span data-ttu-id="934b9-128">reportDate</span><span class="sxs-lookup"><span data-stu-id="934b9-128">reportDate</span></span>        | <span data-ttu-id="934b9-129">Data</span><span class="sxs-lookup"><span data-stu-id="934b9-129">Date</span></span>   |
| <span data-ttu-id="934b9-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="934b9-130">reportPeriod</span></span>      | <span data-ttu-id="934b9-131">String</span><span class="sxs-lookup"><span data-stu-id="934b9-131">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="934b9-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="934b9-132">JSON representation</span></span>

<span data-ttu-id="934b9-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="934b9-133">The following is a JSON representation of the resource.</span></span>

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
