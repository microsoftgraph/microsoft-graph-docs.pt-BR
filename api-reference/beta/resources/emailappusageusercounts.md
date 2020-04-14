---
title: tipo de recurso emailAppUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a9878e2f98ca1beff51e6bd9ea803e8cbebeb390
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440552"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="e5863-103">tipo de recurso emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="e5863-103">emailAppUsageUserCounts resource type</span></span>

<span data-ttu-id="e5863-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5863-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="e5863-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5863-105">Properties</span></span>

| <span data-ttu-id="e5863-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5863-106">Property</span></span>          | <span data-ttu-id="e5863-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5863-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e5863-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e5863-108">reportRefreshDate</span></span> | <span data-ttu-id="e5863-109">Data</span><span class="sxs-lookup"><span data-stu-id="e5863-109">Date</span></span>   |
| <span data-ttu-id="e5863-110">mailForMac</span><span class="sxs-lookup"><span data-stu-id="e5863-110">mailForMac</span></span>        | <span data-ttu-id="e5863-111">Int64</span><span class="sxs-lookup"><span data-stu-id="e5863-111">Int64</span></span>  |
| <span data-ttu-id="e5863-112">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="e5863-112">outlookForMac</span></span>     | <span data-ttu-id="e5863-113">Int64</span><span class="sxs-lookup"><span data-stu-id="e5863-113">Int64</span></span>  |
| <span data-ttu-id="e5863-114">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="e5863-114">outlookForWindows</span></span> | <span data-ttu-id="e5863-115">Int64</span><span class="sxs-lookup"><span data-stu-id="e5863-115">Int64</span></span>  |
| <span data-ttu-id="e5863-116">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="e5863-116">outlookForMobile</span></span>  | <span data-ttu-id="e5863-117">Int64</span><span class="sxs-lookup"><span data-stu-id="e5863-117">Int64</span></span>  |
| <span data-ttu-id="e5863-118">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="e5863-118">otherForMobile</span></span>    | <span data-ttu-id="e5863-119">Int64</span><span class="sxs-lookup"><span data-stu-id="e5863-119">Int64</span></span>  |
| <span data-ttu-id="e5863-120">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="e5863-120">outlookForWeb</span></span>     | <span data-ttu-id="e5863-121">Int64</span><span class="sxs-lookup"><span data-stu-id="e5863-121">Int64</span></span>  |
| <span data-ttu-id="e5863-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="e5863-122">pop3App</span></span>           | <span data-ttu-id="e5863-123">Int64</span><span class="sxs-lookup"><span data-stu-id="e5863-123">Int64</span></span>  |
| <span data-ttu-id="e5863-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="e5863-124">imap4App</span></span>          | <span data-ttu-id="e5863-125">Int64</span><span class="sxs-lookup"><span data-stu-id="e5863-125">Int64</span></span>  |
| <span data-ttu-id="e5863-126">smtpApp</span><span class="sxs-lookup"><span data-stu-id="e5863-126">smtpApp</span></span>           | <span data-ttu-id="e5863-127">Int64</span><span class="sxs-lookup"><span data-stu-id="e5863-127">Int64</span></span>  |
| <span data-ttu-id="e5863-128">reportDate</span><span class="sxs-lookup"><span data-stu-id="e5863-128">reportDate</span></span>        | <span data-ttu-id="e5863-129">Data</span><span class="sxs-lookup"><span data-stu-id="e5863-129">Date</span></span>   |
| <span data-ttu-id="e5863-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e5863-130">reportPeriod</span></span>      | <span data-ttu-id="e5863-131">String</span><span class="sxs-lookup"><span data-stu-id="e5863-131">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e5863-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5863-132">JSON representation</span></span>

<span data-ttu-id="e5863-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5863-133">The following is a JSON representation of the resource.</span></span>

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
