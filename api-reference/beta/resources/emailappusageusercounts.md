---
title: tipo de recurso emailAppUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d8af9e9337c68fcd4434514b85fa9217c79add26
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972170"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="acbba-103">tipo de recurso emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="acbba-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="acbba-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="acbba-104">Properties</span></span>

| <span data-ttu-id="acbba-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acbba-105">Property</span></span>          | <span data-ttu-id="acbba-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="acbba-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="acbba-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="acbba-107">reportRefreshDate</span></span> | <span data-ttu-id="acbba-108">Data</span><span class="sxs-lookup"><span data-stu-id="acbba-108">Date</span></span>   |
| <span data-ttu-id="acbba-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="acbba-109">mailForMac</span></span>        | <span data-ttu-id="acbba-110">Int64</span><span class="sxs-lookup"><span data-stu-id="acbba-110">Int64</span></span>  |
| <span data-ttu-id="acbba-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="acbba-111">outlookForMac</span></span>     | <span data-ttu-id="acbba-112">Int64</span><span class="sxs-lookup"><span data-stu-id="acbba-112">Int64</span></span>  |
| <span data-ttu-id="acbba-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="acbba-113">outlookForWindows</span></span> | <span data-ttu-id="acbba-114">Int64</span><span class="sxs-lookup"><span data-stu-id="acbba-114">Int64</span></span>  |
| <span data-ttu-id="acbba-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="acbba-115">outlookForMobile</span></span>  | <span data-ttu-id="acbba-116">Int64</span><span class="sxs-lookup"><span data-stu-id="acbba-116">Int64</span></span>  |
| <span data-ttu-id="acbba-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="acbba-117">otherForMobile</span></span>    | <span data-ttu-id="acbba-118">Int64</span><span class="sxs-lookup"><span data-stu-id="acbba-118">Int64</span></span>  |
| <span data-ttu-id="acbba-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="acbba-119">outlookForWeb</span></span>     | <span data-ttu-id="acbba-120">Int64</span><span class="sxs-lookup"><span data-stu-id="acbba-120">Int64</span></span>  |
| <span data-ttu-id="acbba-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="acbba-121">pop3App</span></span>           | <span data-ttu-id="acbba-122">Int64</span><span class="sxs-lookup"><span data-stu-id="acbba-122">Int64</span></span>  |
| <span data-ttu-id="acbba-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="acbba-123">imap4App</span></span>          | <span data-ttu-id="acbba-124">Int64</span><span class="sxs-lookup"><span data-stu-id="acbba-124">Int64</span></span>  |
| <span data-ttu-id="acbba-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="acbba-125">smtpApp</span></span>           | <span data-ttu-id="acbba-126">Int64</span><span class="sxs-lookup"><span data-stu-id="acbba-126">Int64</span></span>  |
| <span data-ttu-id="acbba-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="acbba-127">reportDate</span></span>        | <span data-ttu-id="acbba-128">Data</span><span class="sxs-lookup"><span data-stu-id="acbba-128">Date</span></span>   |
| <span data-ttu-id="acbba-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="acbba-129">reportPeriod</span></span>      | <span data-ttu-id="acbba-130">String</span><span class="sxs-lookup"><span data-stu-id="acbba-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="acbba-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="acbba-131">JSON representation</span></span>

<span data-ttu-id="acbba-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="acbba-132">The following is a JSON representation of the resource.</span></span>

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
