---
title: tipo de recurso emailAppUsageAppsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: fb06e9dfe56edb0e7882d0cdce8ee4564375ed93
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440559"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="86d86-103">tipo de recurso emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="86d86-103">emailAppUsageAppsUserCounts resource type</span></span>

<span data-ttu-id="86d86-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86d86-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="86d86-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86d86-105">Properties</span></span>

| <span data-ttu-id="86d86-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86d86-106">Property</span></span>          | <span data-ttu-id="86d86-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="86d86-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="86d86-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="86d86-108">reportRefreshDate</span></span> | <span data-ttu-id="86d86-109">Data</span><span class="sxs-lookup"><span data-stu-id="86d86-109">Date</span></span>   |
| <span data-ttu-id="86d86-110">mailForMac</span><span class="sxs-lookup"><span data-stu-id="86d86-110">mailForMac</span></span>        | <span data-ttu-id="86d86-111">Int64</span><span class="sxs-lookup"><span data-stu-id="86d86-111">Int64</span></span>  |
| <span data-ttu-id="86d86-112">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="86d86-112">outlookForMac</span></span>     | <span data-ttu-id="86d86-113">Int64</span><span class="sxs-lookup"><span data-stu-id="86d86-113">Int64</span></span>  |
| <span data-ttu-id="86d86-114">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="86d86-114">outlookForWindows</span></span> | <span data-ttu-id="86d86-115">Int64</span><span class="sxs-lookup"><span data-stu-id="86d86-115">Int64</span></span>  |
| <span data-ttu-id="86d86-116">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="86d86-116">outlookForMobile</span></span>  | <span data-ttu-id="86d86-117">Int64</span><span class="sxs-lookup"><span data-stu-id="86d86-117">Int64</span></span>  |
| <span data-ttu-id="86d86-118">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="86d86-118">otherForMobile</span></span>    | <span data-ttu-id="86d86-119">Int64</span><span class="sxs-lookup"><span data-stu-id="86d86-119">Int64</span></span>  |
| <span data-ttu-id="86d86-120">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="86d86-120">outlookForWeb</span></span>     | <span data-ttu-id="86d86-121">Int64</span><span class="sxs-lookup"><span data-stu-id="86d86-121">Int64</span></span>  |
| <span data-ttu-id="86d86-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="86d86-122">pop3App</span></span>           | <span data-ttu-id="86d86-123">Int64</span><span class="sxs-lookup"><span data-stu-id="86d86-123">Int64</span></span>  |
| <span data-ttu-id="86d86-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="86d86-124">imap4App</span></span>          | <span data-ttu-id="86d86-125">Int64</span><span class="sxs-lookup"><span data-stu-id="86d86-125">Int64</span></span>  |
| <span data-ttu-id="86d86-126">smtpApp</span><span class="sxs-lookup"><span data-stu-id="86d86-126">smtpApp</span></span>           | <span data-ttu-id="86d86-127">Int64</span><span class="sxs-lookup"><span data-stu-id="86d86-127">Int64</span></span>  |
| <span data-ttu-id="86d86-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="86d86-128">reportPeriod</span></span>      | <span data-ttu-id="86d86-129">String</span><span class="sxs-lookup"><span data-stu-id="86d86-129">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="86d86-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86d86-130">JSON representation</span></span>

<span data-ttu-id="86d86-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86d86-131">The following is a JSON representation of the resource.</span></span>

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
