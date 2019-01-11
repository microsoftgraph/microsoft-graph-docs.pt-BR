---
title: tipo de recurso de skypeForBusinessDeviceUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: d98590e83637e45d35f135c56f2c0b8ff7d282bb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866924"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="05c29-103">tipo de recurso de skypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="05c29-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="05c29-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05c29-104">Properties</span></span>

| <span data-ttu-id="05c29-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05c29-105">Property</span></span>          | <span data-ttu-id="05c29-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="05c29-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="05c29-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="05c29-107">reportRefreshDate</span></span> | <span data-ttu-id="05c29-108">Data</span><span class="sxs-lookup"><span data-stu-id="05c29-108">Date</span></span>   |
| <span data-ttu-id="05c29-109">Windows</span><span class="sxs-lookup"><span data-stu-id="05c29-109">windows</span></span>           | <span data-ttu-id="05c29-110">Int64</span><span class="sxs-lookup"><span data-stu-id="05c29-110">Int64</span></span>  |
| <span data-ttu-id="05c29-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="05c29-111">windowsPhone</span></span>      | <span data-ttu-id="05c29-112">Int64</span><span class="sxs-lookup"><span data-stu-id="05c29-112">Int64</span></span>  |
| <span data-ttu-id="05c29-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="05c29-113">androidPhone</span></span>      | <span data-ttu-id="05c29-114">Int64</span><span class="sxs-lookup"><span data-stu-id="05c29-114">Int64</span></span>  |
| <span data-ttu-id="05c29-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="05c29-115">iPhone</span></span>            | <span data-ttu-id="05c29-116">Int64</span><span class="sxs-lookup"><span data-stu-id="05c29-116">Int64</span></span>  |
| <span data-ttu-id="05c29-117">iPad</span><span class="sxs-lookup"><span data-stu-id="05c29-117">iPad</span></span>              | <span data-ttu-id="05c29-118">Int64</span><span class="sxs-lookup"><span data-stu-id="05c29-118">Int64</span></span>  |
| <span data-ttu-id="05c29-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="05c29-119">reportDate</span></span>        | <span data-ttu-id="05c29-120">Data</span><span class="sxs-lookup"><span data-stu-id="05c29-120">Date</span></span>   |
| <span data-ttu-id="05c29-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="05c29-121">reportPeriod</span></span>      | <span data-ttu-id="05c29-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05c29-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="05c29-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05c29-123">JSON representation</span></span>

<span data-ttu-id="05c29-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="05c29-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "windows": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
