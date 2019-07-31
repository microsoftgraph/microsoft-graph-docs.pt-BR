---
title: tipo de recurso teamsDeviceUsageDistributionUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1842d2edc9e527d577b6a44e61443018f8309c17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007610"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="4049b-103">tipo de recurso teamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="4049b-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4049b-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4049b-104">Properties</span></span>

| <span data-ttu-id="4049b-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4049b-105">Property</span></span>          | <span data-ttu-id="4049b-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="4049b-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4049b-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4049b-107">reportRefreshDate</span></span> | <span data-ttu-id="4049b-108">Data</span><span class="sxs-lookup"><span data-stu-id="4049b-108">Date</span></span>   |
| <span data-ttu-id="4049b-109">web</span><span class="sxs-lookup"><span data-stu-id="4049b-109">web</span></span>               | <span data-ttu-id="4049b-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4049b-110">Int64</span></span>  |
| <span data-ttu-id="4049b-111">Windowsphonee</span><span class="sxs-lookup"><span data-stu-id="4049b-111">windowsPhone</span></span>      | <span data-ttu-id="4049b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4049b-112">Int64</span></span>  |
| <span data-ttu-id="4049b-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="4049b-113">androidPhone</span></span>      | <span data-ttu-id="4049b-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4049b-114">Int64</span></span>  |
| <span data-ttu-id="4049b-115">emiti</span><span class="sxs-lookup"><span data-stu-id="4049b-115">ios</span></span>               | <span data-ttu-id="4049b-116">Int64</span><span class="sxs-lookup"><span data-stu-id="4049b-116">Int64</span></span>  |
| <span data-ttu-id="4049b-117">mac</span><span class="sxs-lookup"><span data-stu-id="4049b-117">mac</span></span>               | <span data-ttu-id="4049b-118">Int64</span><span class="sxs-lookup"><span data-stu-id="4049b-118">Int64</span></span>  |
| <span data-ttu-id="4049b-119">Windows</span><span class="sxs-lookup"><span data-stu-id="4049b-119">windows</span></span>           | <span data-ttu-id="4049b-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4049b-120">Int64</span></span>  |
| <span data-ttu-id="4049b-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4049b-121">reportPeriod</span></span>      | <span data-ttu-id="4049b-122">String</span><span class="sxs-lookup"><span data-stu-id="4049b-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4049b-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4049b-123">JSON representation</span></span>

<span data-ttu-id="4049b-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4049b-124">The following is a JSON representation of the resource.</span></span>

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
