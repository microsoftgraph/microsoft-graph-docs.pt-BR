---
title: tipo de recurso de teamsDeviceUsageDistributionUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d398782cef79cdf92bc56502f7c6cbf1bcdee99d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979282"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="2b1cb-103">tipo de recurso de teamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="2b1cb-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2b1cb-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b1cb-104">Properties</span></span>

| <span data-ttu-id="2b1cb-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b1cb-105">Property</span></span>          | <span data-ttu-id="2b1cb-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b1cb-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="2b1cb-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2b1cb-107">reportRefreshDate</span></span> | <span data-ttu-id="2b1cb-108">Data</span><span class="sxs-lookup"><span data-stu-id="2b1cb-108">Date</span></span>   |
| <span data-ttu-id="2b1cb-109">web</span><span class="sxs-lookup"><span data-stu-id="2b1cb-109">web</span></span>               | <span data-ttu-id="2b1cb-110">Int64</span><span class="sxs-lookup"><span data-stu-id="2b1cb-110">Int64</span></span>  |
| <span data-ttu-id="2b1cb-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="2b1cb-111">windowsPhone</span></span>      | <span data-ttu-id="2b1cb-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2b1cb-112">Int64</span></span>  |
| <span data-ttu-id="2b1cb-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="2b1cb-113">androidPhone</span></span>      | <span data-ttu-id="2b1cb-114">Int64</span><span class="sxs-lookup"><span data-stu-id="2b1cb-114">Int64</span></span>  |
| <span data-ttu-id="2b1cb-115">IOS</span><span class="sxs-lookup"><span data-stu-id="2b1cb-115">ios</span></span>               | <span data-ttu-id="2b1cb-116">Int64</span><span class="sxs-lookup"><span data-stu-id="2b1cb-116">Int64</span></span>  |
| <span data-ttu-id="2b1cb-117">mac</span><span class="sxs-lookup"><span data-stu-id="2b1cb-117">mac</span></span>               | <span data-ttu-id="2b1cb-118">Int64</span><span class="sxs-lookup"><span data-stu-id="2b1cb-118">Int64</span></span>  |
| <span data-ttu-id="2b1cb-119">Windows</span><span class="sxs-lookup"><span data-stu-id="2b1cb-119">windows</span></span>           | <span data-ttu-id="2b1cb-120">Int64</span><span class="sxs-lookup"><span data-stu-id="2b1cb-120">Int64</span></span>  |
| <span data-ttu-id="2b1cb-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2b1cb-121">reportPeriod</span></span>      | <span data-ttu-id="2b1cb-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b1cb-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2b1cb-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b1cb-123">JSON representation</span></span>

<span data-ttu-id="2b1cb-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b1cb-124">The following is a JSON representation of the resource.</span></span>

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
