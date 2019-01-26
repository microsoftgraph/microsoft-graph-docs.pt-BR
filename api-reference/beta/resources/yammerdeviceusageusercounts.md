---
title: tipo de recurso de yammerDeviceUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 63bd3e150e822d3c356f4409c2920e4998e53ec2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577323"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="8226d-103">tipo de recurso de yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="8226d-103">yammerDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8226d-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8226d-104">Properties</span></span>

| <span data-ttu-id="8226d-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8226d-105">Property</span></span>          | <span data-ttu-id="8226d-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="8226d-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="8226d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8226d-107">reportRefreshDate</span></span> | <span data-ttu-id="8226d-108">Data</span><span class="sxs-lookup"><span data-stu-id="8226d-108">Date</span></span>   |
| <span data-ttu-id="8226d-109">web</span><span class="sxs-lookup"><span data-stu-id="8226d-109">web</span></span>               | <span data-ttu-id="8226d-110">Int32</span><span class="sxs-lookup"><span data-stu-id="8226d-110">Int32</span></span>  |
| <span data-ttu-id="8226d-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="8226d-111">windowsPhone</span></span>      | <span data-ttu-id="8226d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="8226d-112">Int32</span></span>  |
| <span data-ttu-id="8226d-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="8226d-113">androidPhone</span></span>      | <span data-ttu-id="8226d-114">Int32</span><span class="sxs-lookup"><span data-stu-id="8226d-114">Int32</span></span>  |
| <span data-ttu-id="8226d-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="8226d-115">iPhone</span></span>            | <span data-ttu-id="8226d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="8226d-116">Int32</span></span>  |
| <span data-ttu-id="8226d-117">iPad</span><span class="sxs-lookup"><span data-stu-id="8226d-117">iPad</span></span>              | <span data-ttu-id="8226d-118">Int32</span><span class="sxs-lookup"><span data-stu-id="8226d-118">Int32</span></span>  |
| <span data-ttu-id="8226d-119">outros</span><span class="sxs-lookup"><span data-stu-id="8226d-119">other</span></span>             | <span data-ttu-id="8226d-120">Int32</span><span class="sxs-lookup"><span data-stu-id="8226d-120">Int32</span></span>  |
| <span data-ttu-id="8226d-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="8226d-121">reportDate</span></span>        | <span data-ttu-id="8226d-122">Data</span><span class="sxs-lookup"><span data-stu-id="8226d-122">Date</span></span>   |
| <span data-ttu-id="8226d-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8226d-123">reportPeriod</span></span>      | <span data-ttu-id="8226d-124">String</span><span class="sxs-lookup"><span data-stu-id="8226d-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8226d-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8226d-125">JSON representation</span></span>

<span data-ttu-id="8226d-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8226d-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "other": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
