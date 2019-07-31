---
title: tipo de recurso emailAppUsageAppsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0ca694c5d416dcc062984ba03a3521a39a010a87
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972177"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="11291-103">tipo de recurso emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="11291-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="11291-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11291-104">Properties</span></span>

| <span data-ttu-id="11291-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11291-105">Property</span></span>          | <span data-ttu-id="11291-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="11291-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="11291-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="11291-107">reportRefreshDate</span></span> | <span data-ttu-id="11291-108">Data</span><span class="sxs-lookup"><span data-stu-id="11291-108">Date</span></span>   |
| <span data-ttu-id="11291-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="11291-109">mailForMac</span></span>        | <span data-ttu-id="11291-110">Int64</span><span class="sxs-lookup"><span data-stu-id="11291-110">Int64</span></span>  |
| <span data-ttu-id="11291-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="11291-111">outlookForMac</span></span>     | <span data-ttu-id="11291-112">Int64</span><span class="sxs-lookup"><span data-stu-id="11291-112">Int64</span></span>  |
| <span data-ttu-id="11291-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="11291-113">outlookForWindows</span></span> | <span data-ttu-id="11291-114">Int64</span><span class="sxs-lookup"><span data-stu-id="11291-114">Int64</span></span>  |
| <span data-ttu-id="11291-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="11291-115">outlookForMobile</span></span>  | <span data-ttu-id="11291-116">Int64</span><span class="sxs-lookup"><span data-stu-id="11291-116">Int64</span></span>  |
| <span data-ttu-id="11291-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="11291-117">otherForMobile</span></span>    | <span data-ttu-id="11291-118">Int64</span><span class="sxs-lookup"><span data-stu-id="11291-118">Int64</span></span>  |
| <span data-ttu-id="11291-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="11291-119">outlookForWeb</span></span>     | <span data-ttu-id="11291-120">Int64</span><span class="sxs-lookup"><span data-stu-id="11291-120">Int64</span></span>  |
| <span data-ttu-id="11291-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="11291-121">pop3App</span></span>           | <span data-ttu-id="11291-122">Int64</span><span class="sxs-lookup"><span data-stu-id="11291-122">Int64</span></span>  |
| <span data-ttu-id="11291-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="11291-123">imap4App</span></span>          | <span data-ttu-id="11291-124">Int64</span><span class="sxs-lookup"><span data-stu-id="11291-124">Int64</span></span>  |
| <span data-ttu-id="11291-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="11291-125">smtpApp</span></span>           | <span data-ttu-id="11291-126">Int64</span><span class="sxs-lookup"><span data-stu-id="11291-126">Int64</span></span>  |
| <span data-ttu-id="11291-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="11291-127">reportPeriod</span></span>      | <span data-ttu-id="11291-128">String</span><span class="sxs-lookup"><span data-stu-id="11291-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="11291-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11291-129">JSON representation</span></span>

<span data-ttu-id="11291-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11291-130">The following is a JSON representation of the resource.</span></span>

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
