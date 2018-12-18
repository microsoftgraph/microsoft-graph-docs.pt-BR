---
title: tipo de recurso de teamsDeviceUsageDistributionUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
ms.openlocfilehash: 01b9f67f30a7b2f13aac65cbcd4795792ee0aaa0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345847"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="ba9ee-103">tipo de recurso de teamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="ba9ee-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ba9ee-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba9ee-104">Properties</span></span>

| <span data-ttu-id="ba9ee-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba9ee-105">Property</span></span>          | <span data-ttu-id="ba9ee-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba9ee-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="ba9ee-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ba9ee-107">reportRefreshDate</span></span> | <span data-ttu-id="ba9ee-108">Data</span><span class="sxs-lookup"><span data-stu-id="ba9ee-108">Date</span></span>   |
| <span data-ttu-id="ba9ee-109">web</span><span class="sxs-lookup"><span data-stu-id="ba9ee-109">web</span></span>               | <span data-ttu-id="ba9ee-110">Int64</span><span class="sxs-lookup"><span data-stu-id="ba9ee-110">Int64</span></span>  |
| <span data-ttu-id="ba9ee-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="ba9ee-111">windowsPhone</span></span>      | <span data-ttu-id="ba9ee-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ba9ee-112">Int64</span></span>  |
| <span data-ttu-id="ba9ee-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="ba9ee-113">androidPhone</span></span>      | <span data-ttu-id="ba9ee-114">Int64</span><span class="sxs-lookup"><span data-stu-id="ba9ee-114">Int64</span></span>  |
| <span data-ttu-id="ba9ee-115">IOS</span><span class="sxs-lookup"><span data-stu-id="ba9ee-115">ios</span></span>               | <span data-ttu-id="ba9ee-116">Int64</span><span class="sxs-lookup"><span data-stu-id="ba9ee-116">Int64</span></span>  |
| <span data-ttu-id="ba9ee-117">mac</span><span class="sxs-lookup"><span data-stu-id="ba9ee-117">mac</span></span>               | <span data-ttu-id="ba9ee-118">Int64</span><span class="sxs-lookup"><span data-stu-id="ba9ee-118">Int64</span></span>  |
| <span data-ttu-id="ba9ee-119">Windows</span><span class="sxs-lookup"><span data-stu-id="ba9ee-119">windows</span></span>           | <span data-ttu-id="ba9ee-120">Int64</span><span class="sxs-lookup"><span data-stu-id="ba9ee-120">Int64</span></span>  |
| <span data-ttu-id="ba9ee-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ba9ee-121">reportPeriod</span></span>      | <span data-ttu-id="ba9ee-122">String</span><span class="sxs-lookup"><span data-stu-id="ba9ee-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ba9ee-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba9ee-123">JSON representation</span></span>

<span data-ttu-id="ba9ee-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba9ee-124">The following is a JSON representation of the resource.</span></span>

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
