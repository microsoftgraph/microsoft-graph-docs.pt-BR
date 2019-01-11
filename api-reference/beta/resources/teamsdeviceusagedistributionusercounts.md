---
title: tipo de recurso de teamsDeviceUsageDistributionUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: a02dfa5a5036d67a624656d715c0fb0d3c8194ef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868695"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="ad490-103">tipo de recurso de teamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="ad490-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ad490-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad490-104">Properties</span></span>

| <span data-ttu-id="ad490-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad490-105">Property</span></span>          | <span data-ttu-id="ad490-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad490-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="ad490-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ad490-107">reportRefreshDate</span></span> | <span data-ttu-id="ad490-108">Data</span><span class="sxs-lookup"><span data-stu-id="ad490-108">Date</span></span>   |
| <span data-ttu-id="ad490-109">web</span><span class="sxs-lookup"><span data-stu-id="ad490-109">web</span></span>               | <span data-ttu-id="ad490-110">Int64</span><span class="sxs-lookup"><span data-stu-id="ad490-110">Int64</span></span>  |
| <span data-ttu-id="ad490-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="ad490-111">windowsPhone</span></span>      | <span data-ttu-id="ad490-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ad490-112">Int64</span></span>  |
| <span data-ttu-id="ad490-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="ad490-113">androidPhone</span></span>      | <span data-ttu-id="ad490-114">Int64</span><span class="sxs-lookup"><span data-stu-id="ad490-114">Int64</span></span>  |
| <span data-ttu-id="ad490-115">IOS</span><span class="sxs-lookup"><span data-stu-id="ad490-115">ios</span></span>               | <span data-ttu-id="ad490-116">Int64</span><span class="sxs-lookup"><span data-stu-id="ad490-116">Int64</span></span>  |
| <span data-ttu-id="ad490-117">mac</span><span class="sxs-lookup"><span data-stu-id="ad490-117">mac</span></span>               | <span data-ttu-id="ad490-118">Int64</span><span class="sxs-lookup"><span data-stu-id="ad490-118">Int64</span></span>  |
| <span data-ttu-id="ad490-119">Windows</span><span class="sxs-lookup"><span data-stu-id="ad490-119">windows</span></span>           | <span data-ttu-id="ad490-120">Int64</span><span class="sxs-lookup"><span data-stu-id="ad490-120">Int64</span></span>  |
| <span data-ttu-id="ad490-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ad490-121">reportPeriod</span></span>      | <span data-ttu-id="ad490-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad490-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ad490-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad490-123">JSON representation</span></span>

<span data-ttu-id="ad490-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ad490-124">The following is a JSON representation of the resource.</span></span>

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
