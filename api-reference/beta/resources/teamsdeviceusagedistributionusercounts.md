---
title: tipo de recurso teamsDeviceUsageDistributionUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6b5a4a09c96c5b3691c4cbcc285ac947c903ce50
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046479"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="12521-103">tipo de recurso teamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="12521-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="12521-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12521-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="12521-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12521-105">Properties</span></span>

| <span data-ttu-id="12521-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12521-106">Property</span></span>          | <span data-ttu-id="12521-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="12521-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="12521-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="12521-108">reportRefreshDate</span></span> | <span data-ttu-id="12521-109">Data</span><span class="sxs-lookup"><span data-stu-id="12521-109">Date</span></span>   |
| <span data-ttu-id="12521-110">web</span><span class="sxs-lookup"><span data-stu-id="12521-110">web</span></span>               | <span data-ttu-id="12521-111">Int64</span><span class="sxs-lookup"><span data-stu-id="12521-111">Int64</span></span>  |
| <span data-ttu-id="12521-112">Windowsphonee</span><span class="sxs-lookup"><span data-stu-id="12521-112">windowsPhone</span></span>      | <span data-ttu-id="12521-113">Int64</span><span class="sxs-lookup"><span data-stu-id="12521-113">Int64</span></span>  |
| <span data-ttu-id="12521-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="12521-114">androidPhone</span></span>      | <span data-ttu-id="12521-115">Int64</span><span class="sxs-lookup"><span data-stu-id="12521-115">Int64</span></span>  |
| <span data-ttu-id="12521-116">emiti</span><span class="sxs-lookup"><span data-stu-id="12521-116">ios</span></span>               | <span data-ttu-id="12521-117">Int64</span><span class="sxs-lookup"><span data-stu-id="12521-117">Int64</span></span>  |
| <span data-ttu-id="12521-118">mac</span><span class="sxs-lookup"><span data-stu-id="12521-118">mac</span></span>               | <span data-ttu-id="12521-119">Int64</span><span class="sxs-lookup"><span data-stu-id="12521-119">Int64</span></span>  |
| <span data-ttu-id="12521-120">Windows</span><span class="sxs-lookup"><span data-stu-id="12521-120">windows</span></span>           | <span data-ttu-id="12521-121">Int64</span><span class="sxs-lookup"><span data-stu-id="12521-121">Int64</span></span>  |
| <span data-ttu-id="12521-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="12521-122">reportPeriod</span></span>      | <span data-ttu-id="12521-123">String</span><span class="sxs-lookup"><span data-stu-id="12521-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="12521-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12521-124">JSON representation</span></span>

<span data-ttu-id="12521-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12521-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
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
  "reportPeriod": "String"
}
```


