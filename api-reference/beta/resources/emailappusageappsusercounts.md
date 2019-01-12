---
title: tipo de recurso de emailAppUsageAppsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 220770fab755c0e345af23f3fc3113732af63ff0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970378"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="407c3-103">tipo de recurso de emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="407c3-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="407c3-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="407c3-104">Properties</span></span>

| <span data-ttu-id="407c3-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="407c3-105">Property</span></span>          | <span data-ttu-id="407c3-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="407c3-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="407c3-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="407c3-107">reportRefreshDate</span></span> | <span data-ttu-id="407c3-108">Data</span><span class="sxs-lookup"><span data-stu-id="407c3-108">Date</span></span>   |
| <span data-ttu-id="407c3-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="407c3-109">mailForMac</span></span>        | <span data-ttu-id="407c3-110">Int64</span><span class="sxs-lookup"><span data-stu-id="407c3-110">Int64</span></span>  |
| <span data-ttu-id="407c3-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="407c3-111">outlookForMac</span></span>     | <span data-ttu-id="407c3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="407c3-112">Int64</span></span>  |
| <span data-ttu-id="407c3-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="407c3-113">outlookForWindows</span></span> | <span data-ttu-id="407c3-114">Int64</span><span class="sxs-lookup"><span data-stu-id="407c3-114">Int64</span></span>  |
| <span data-ttu-id="407c3-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="407c3-115">outlookForMobile</span></span>  | <span data-ttu-id="407c3-116">Int64</span><span class="sxs-lookup"><span data-stu-id="407c3-116">Int64</span></span>  |
| <span data-ttu-id="407c3-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="407c3-117">otherForMobile</span></span>    | <span data-ttu-id="407c3-118">Int64</span><span class="sxs-lookup"><span data-stu-id="407c3-118">Int64</span></span>  |
| <span data-ttu-id="407c3-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="407c3-119">outlookForWeb</span></span>     | <span data-ttu-id="407c3-120">Int64</span><span class="sxs-lookup"><span data-stu-id="407c3-120">Int64</span></span>  |
| <span data-ttu-id="407c3-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="407c3-121">pop3App</span></span>           | <span data-ttu-id="407c3-122">Int64</span><span class="sxs-lookup"><span data-stu-id="407c3-122">Int64</span></span>  |
| <span data-ttu-id="407c3-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="407c3-123">imap4App</span></span>          | <span data-ttu-id="407c3-124">Int64</span><span class="sxs-lookup"><span data-stu-id="407c3-124">Int64</span></span>  |
| <span data-ttu-id="407c3-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="407c3-125">smtpApp</span></span>           | <span data-ttu-id="407c3-126">Int64</span><span class="sxs-lookup"><span data-stu-id="407c3-126">Int64</span></span>  |
| <span data-ttu-id="407c3-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="407c3-127">reportPeriod</span></span>      | <span data-ttu-id="407c3-128">String</span><span class="sxs-lookup"><span data-stu-id="407c3-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="407c3-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="407c3-129">JSON representation</span></span>

<span data-ttu-id="407c3-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="407c3-130">The following is a JSON representation of the resource.</span></span>

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
