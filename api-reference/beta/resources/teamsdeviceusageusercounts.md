---
title: tipo de recurso teamsDeviceUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: af62b0bf6d11c256252b2c6c6f16f4e3b5ba2354
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046465"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="dfdb0-103">tipo de recurso teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="dfdb0-103">teamsDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="dfdb0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfdb0-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="dfdb0-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dfdb0-105">Properties</span></span>

| <span data-ttu-id="dfdb0-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dfdb0-106">Property</span></span>          | <span data-ttu-id="dfdb0-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfdb0-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="dfdb0-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="dfdb0-108">reportRefreshDate</span></span> | <span data-ttu-id="dfdb0-109">Data</span><span class="sxs-lookup"><span data-stu-id="dfdb0-109">Date</span></span>   |
| <span data-ttu-id="dfdb0-110">web</span><span class="sxs-lookup"><span data-stu-id="dfdb0-110">web</span></span>               | <span data-ttu-id="dfdb0-111">Int64</span><span class="sxs-lookup"><span data-stu-id="dfdb0-111">Int64</span></span>  |
| <span data-ttu-id="dfdb0-112">Windowsphonee</span><span class="sxs-lookup"><span data-stu-id="dfdb0-112">windowsPhone</span></span>      | <span data-ttu-id="dfdb0-113">Int64</span><span class="sxs-lookup"><span data-stu-id="dfdb0-113">Int64</span></span>  |
| <span data-ttu-id="dfdb0-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="dfdb0-114">androidPhone</span></span>      | <span data-ttu-id="dfdb0-115">Int64</span><span class="sxs-lookup"><span data-stu-id="dfdb0-115">Int64</span></span>  |
| <span data-ttu-id="dfdb0-116">emiti</span><span class="sxs-lookup"><span data-stu-id="dfdb0-116">ios</span></span>               | <span data-ttu-id="dfdb0-117">Int64</span><span class="sxs-lookup"><span data-stu-id="dfdb0-117">Int64</span></span>  |
| <span data-ttu-id="dfdb0-118">mac</span><span class="sxs-lookup"><span data-stu-id="dfdb0-118">mac</span></span>               | <span data-ttu-id="dfdb0-119">Int64</span><span class="sxs-lookup"><span data-stu-id="dfdb0-119">Int64</span></span>  |
| <span data-ttu-id="dfdb0-120">Windows</span><span class="sxs-lookup"><span data-stu-id="dfdb0-120">windows</span></span>           | <span data-ttu-id="dfdb0-121">Int64</span><span class="sxs-lookup"><span data-stu-id="dfdb0-121">Int64</span></span>  |
| <span data-ttu-id="dfdb0-122">reportDate</span><span class="sxs-lookup"><span data-stu-id="dfdb0-122">reportDate</span></span>        | <span data-ttu-id="dfdb0-123">Data</span><span class="sxs-lookup"><span data-stu-id="dfdb0-123">Date</span></span>   |
| <span data-ttu-id="dfdb0-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="dfdb0-124">reportPeriod</span></span>      | <span data-ttu-id="dfdb0-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dfdb0-125">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dfdb0-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dfdb0-126">JSON representation</span></span>

<span data-ttu-id="dfdb0-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dfdb0-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


