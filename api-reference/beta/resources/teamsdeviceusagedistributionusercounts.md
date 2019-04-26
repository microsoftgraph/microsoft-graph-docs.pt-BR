---
title: tipo de recurso teamsDeviceUsageDistributionUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d398782cef79cdf92bc56502f7c6cbf1bcdee99d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553607"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="78960-103">tipo de recurso teamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="78960-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="78960-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78960-104">Properties</span></span>

| <span data-ttu-id="78960-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78960-105">Property</span></span>          | <span data-ttu-id="78960-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="78960-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="78960-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="78960-107">reportRefreshDate</span></span> | <span data-ttu-id="78960-108">Data</span><span class="sxs-lookup"><span data-stu-id="78960-108">Date</span></span>   |
| <span data-ttu-id="78960-109">web</span><span class="sxs-lookup"><span data-stu-id="78960-109">web</span></span>               | <span data-ttu-id="78960-110">Int64</span><span class="sxs-lookup"><span data-stu-id="78960-110">Int64</span></span>  |
| <span data-ttu-id="78960-111">Windowsphonee</span><span class="sxs-lookup"><span data-stu-id="78960-111">windowsPhone</span></span>      | <span data-ttu-id="78960-112">Int64</span><span class="sxs-lookup"><span data-stu-id="78960-112">Int64</span></span>  |
| <span data-ttu-id="78960-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="78960-113">androidPhone</span></span>      | <span data-ttu-id="78960-114">Int64</span><span class="sxs-lookup"><span data-stu-id="78960-114">Int64</span></span>  |
| <span data-ttu-id="78960-115">emiti</span><span class="sxs-lookup"><span data-stu-id="78960-115">ios</span></span>               | <span data-ttu-id="78960-116">Int64</span><span class="sxs-lookup"><span data-stu-id="78960-116">Int64</span></span>  |
| <span data-ttu-id="78960-117">mac</span><span class="sxs-lookup"><span data-stu-id="78960-117">mac</span></span>               | <span data-ttu-id="78960-118">Int64</span><span class="sxs-lookup"><span data-stu-id="78960-118">Int64</span></span>  |
| <span data-ttu-id="78960-119">Windows</span><span class="sxs-lookup"><span data-stu-id="78960-119">windows</span></span>           | <span data-ttu-id="78960-120">Int64</span><span class="sxs-lookup"><span data-stu-id="78960-120">Int64</span></span>  |
| <span data-ttu-id="78960-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="78960-121">reportPeriod</span></span>      | <span data-ttu-id="78960-122">String</span><span class="sxs-lookup"><span data-stu-id="78960-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="78960-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78960-123">JSON representation</span></span>

<span data-ttu-id="78960-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="78960-124">The following is a JSON representation of the resource.</span></span>

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
