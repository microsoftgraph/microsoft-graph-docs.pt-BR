---
title: tipo de recurso de teamsDeviceUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
ms.openlocfilehash: 1255a8e1e92bb461d5c100c72e9030f57db5f8fa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306507"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="3a5e4-103">tipo de recurso de teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="3a5e4-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3a5e4-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a5e4-104">Properties</span></span>

| <span data-ttu-id="3a5e4-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a5e4-105">Property</span></span>          | <span data-ttu-id="3a5e4-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a5e4-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="3a5e4-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3a5e4-107">reportRefreshDate</span></span> | <span data-ttu-id="3a5e4-108">Data</span><span class="sxs-lookup"><span data-stu-id="3a5e4-108">Date</span></span>   |
| <span data-ttu-id="3a5e4-109">web</span><span class="sxs-lookup"><span data-stu-id="3a5e4-109">web</span></span>               | <span data-ttu-id="3a5e4-110">Int64</span><span class="sxs-lookup"><span data-stu-id="3a5e4-110">Int64</span></span>  |
| <span data-ttu-id="3a5e4-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="3a5e4-111">windowsPhone</span></span>      | <span data-ttu-id="3a5e4-112">Int64</span><span class="sxs-lookup"><span data-stu-id="3a5e4-112">Int64</span></span>  |
| <span data-ttu-id="3a5e4-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="3a5e4-113">androidPhone</span></span>      | <span data-ttu-id="3a5e4-114">Int64</span><span class="sxs-lookup"><span data-stu-id="3a5e4-114">Int64</span></span>  |
| <span data-ttu-id="3a5e4-115">IOS</span><span class="sxs-lookup"><span data-stu-id="3a5e4-115">ios</span></span>               | <span data-ttu-id="3a5e4-116">Int64</span><span class="sxs-lookup"><span data-stu-id="3a5e4-116">Int64</span></span>  |
| <span data-ttu-id="3a5e4-117">mac</span><span class="sxs-lookup"><span data-stu-id="3a5e4-117">mac</span></span>               | <span data-ttu-id="3a5e4-118">Int64</span><span class="sxs-lookup"><span data-stu-id="3a5e4-118">Int64</span></span>  |
| <span data-ttu-id="3a5e4-119">Windows</span><span class="sxs-lookup"><span data-stu-id="3a5e4-119">windows</span></span>           | <span data-ttu-id="3a5e4-120">Int64</span><span class="sxs-lookup"><span data-stu-id="3a5e4-120">Int64</span></span>  |
| <span data-ttu-id="3a5e4-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="3a5e4-121">reportDate</span></span>        | <span data-ttu-id="3a5e4-122">Data</span><span class="sxs-lookup"><span data-stu-id="3a5e4-122">Date</span></span>   |
| <span data-ttu-id="3a5e4-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3a5e4-123">reportPeriod</span></span>      | <span data-ttu-id="3a5e4-124">String</span><span class="sxs-lookup"><span data-stu-id="3a5e4-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3a5e4-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a5e4-125">JSON representation</span></span>

<span data-ttu-id="3a5e4-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a5e4-126">The following is a JSON representation of the resource.</span></span>

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
