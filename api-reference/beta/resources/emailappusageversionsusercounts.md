---
title: tipo de recurso de emailAppUsageVersionsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 371352c42e870f45224999b7a618d1bb694ea512
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965282"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="109b8-103">tipo de recurso de emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="109b8-103">emailAppUsageVersionsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="109b8-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="109b8-104">Properties</span></span>

| <span data-ttu-id="109b8-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="109b8-105">Property</span></span>          | <span data-ttu-id="109b8-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="109b8-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="109b8-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="109b8-107">reportRefreshDate</span></span> | <span data-ttu-id="109b8-108">Data</span><span class="sxs-lookup"><span data-stu-id="109b8-108">Date</span></span>   |
| <span data-ttu-id="109b8-109">outlook2016</span><span class="sxs-lookup"><span data-stu-id="109b8-109">outlook2016</span></span>       | <span data-ttu-id="109b8-110">Int64</span><span class="sxs-lookup"><span data-stu-id="109b8-110">Int64</span></span>  |
| <span data-ttu-id="109b8-111">outlook2013</span><span class="sxs-lookup"><span data-stu-id="109b8-111">outlook2013</span></span>       | <span data-ttu-id="109b8-112">Int64</span><span class="sxs-lookup"><span data-stu-id="109b8-112">Int64</span></span>  |
| <span data-ttu-id="109b8-113">outlook2010</span><span class="sxs-lookup"><span data-stu-id="109b8-113">outlook2010</span></span>       | <span data-ttu-id="109b8-114">Int64</span><span class="sxs-lookup"><span data-stu-id="109b8-114">Int64</span></span>  |
| <span data-ttu-id="109b8-115">outlook2007</span><span class="sxs-lookup"><span data-stu-id="109b8-115">outlook2007</span></span>       | <span data-ttu-id="109b8-116">Int64</span><span class="sxs-lookup"><span data-stu-id="109b8-116">Int64</span></span>  |
| <span data-ttu-id="109b8-117">indeterminado</span><span class="sxs-lookup"><span data-stu-id="109b8-117">undetermined</span></span>      | <span data-ttu-id="109b8-118">Int64</span><span class="sxs-lookup"><span data-stu-id="109b8-118">Int64</span></span>  |
| <span data-ttu-id="109b8-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="109b8-119">reportPeriod</span></span>      | <span data-ttu-id="109b8-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="109b8-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="109b8-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="109b8-121">JSON representation</span></span>

<span data-ttu-id="109b8-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="109b8-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "outlook2016": 1024, 
  "outlook2013": 1024, 
  "outlook2010": 1024, 
  "outlook2007": 1024, 
  "undetermined": 1024, 
  "reportPeriod": "String"
}
```
