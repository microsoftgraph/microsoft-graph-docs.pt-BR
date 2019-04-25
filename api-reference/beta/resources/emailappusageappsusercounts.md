---
title: tipo de recurso emailAppUsageAppsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 220770fab755c0e345af23f3fc3113732af63ff0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542808"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="e8111-103">tipo de recurso emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="e8111-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e8111-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8111-104">Properties</span></span>

| <span data-ttu-id="e8111-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8111-105">Property</span></span>          | <span data-ttu-id="e8111-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8111-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e8111-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e8111-107">reportRefreshDate</span></span> | <span data-ttu-id="e8111-108">Data</span><span class="sxs-lookup"><span data-stu-id="e8111-108">Date</span></span>   |
| <span data-ttu-id="e8111-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="e8111-109">mailForMac</span></span>        | <span data-ttu-id="e8111-110">Int64</span><span class="sxs-lookup"><span data-stu-id="e8111-110">Int64</span></span>  |
| <span data-ttu-id="e8111-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="e8111-111">outlookForMac</span></span>     | <span data-ttu-id="e8111-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e8111-112">Int64</span></span>  |
| <span data-ttu-id="e8111-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="e8111-113">outlookForWindows</span></span> | <span data-ttu-id="e8111-114">Int64</span><span class="sxs-lookup"><span data-stu-id="e8111-114">Int64</span></span>  |
| <span data-ttu-id="e8111-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="e8111-115">outlookForMobile</span></span>  | <span data-ttu-id="e8111-116">Int64</span><span class="sxs-lookup"><span data-stu-id="e8111-116">Int64</span></span>  |
| <span data-ttu-id="e8111-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="e8111-117">otherForMobile</span></span>    | <span data-ttu-id="e8111-118">Int64</span><span class="sxs-lookup"><span data-stu-id="e8111-118">Int64</span></span>  |
| <span data-ttu-id="e8111-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="e8111-119">outlookForWeb</span></span>     | <span data-ttu-id="e8111-120">Int64</span><span class="sxs-lookup"><span data-stu-id="e8111-120">Int64</span></span>  |
| <span data-ttu-id="e8111-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="e8111-121">pop3App</span></span>           | <span data-ttu-id="e8111-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e8111-122">Int64</span></span>  |
| <span data-ttu-id="e8111-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="e8111-123">imap4App</span></span>          | <span data-ttu-id="e8111-124">Int64</span><span class="sxs-lookup"><span data-stu-id="e8111-124">Int64</span></span>  |
| <span data-ttu-id="e8111-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="e8111-125">smtpApp</span></span>           | <span data-ttu-id="e8111-126">Int64</span><span class="sxs-lookup"><span data-stu-id="e8111-126">Int64</span></span>  |
| <span data-ttu-id="e8111-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e8111-127">reportPeriod</span></span>      | <span data-ttu-id="e8111-128">String</span><span class="sxs-lookup"><span data-stu-id="e8111-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e8111-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8111-129">JSON representation</span></span>

<span data-ttu-id="e8111-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8111-130">The following is a JSON representation of the resource.</span></span>

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
