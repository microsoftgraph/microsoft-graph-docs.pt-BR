---
title: tipo de recurso yammerDeviceUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 6832d4c1829c6fd7ce679fe12511b694cc999b95
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963777"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="31ac4-103">tipo de recurso yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="31ac4-103">yammerDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="31ac4-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31ac4-104">Properties</span></span>

| <span data-ttu-id="31ac4-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31ac4-105">Property</span></span>          | <span data-ttu-id="31ac4-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="31ac4-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="31ac4-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="31ac4-107">reportRefreshDate</span></span> | <span data-ttu-id="31ac4-108">Data</span><span class="sxs-lookup"><span data-stu-id="31ac4-108">Date</span></span>   |
| <span data-ttu-id="31ac4-109">web</span><span class="sxs-lookup"><span data-stu-id="31ac4-109">web</span></span>               | <span data-ttu-id="31ac4-110">Int32</span><span class="sxs-lookup"><span data-stu-id="31ac4-110">Int32</span></span>  |
| <span data-ttu-id="31ac4-111">Windowsphonee</span><span class="sxs-lookup"><span data-stu-id="31ac4-111">windowsPhone</span></span>      | <span data-ttu-id="31ac4-112">Int32</span><span class="sxs-lookup"><span data-stu-id="31ac4-112">Int32</span></span>  |
| <span data-ttu-id="31ac4-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="31ac4-113">androidPhone</span></span>      | <span data-ttu-id="31ac4-114">Int32</span><span class="sxs-lookup"><span data-stu-id="31ac4-114">Int32</span></span>  |
| <span data-ttu-id="31ac4-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="31ac4-115">iPhone</span></span>            | <span data-ttu-id="31ac4-116">Int32</span><span class="sxs-lookup"><span data-stu-id="31ac4-116">Int32</span></span>  |
| <span data-ttu-id="31ac4-117">iPad</span><span class="sxs-lookup"><span data-stu-id="31ac4-117">iPad</span></span>              | <span data-ttu-id="31ac4-118">Int32</span><span class="sxs-lookup"><span data-stu-id="31ac4-118">Int32</span></span>  |
| <span data-ttu-id="31ac4-119">outro</span><span class="sxs-lookup"><span data-stu-id="31ac4-119">other</span></span>             | <span data-ttu-id="31ac4-120">Int32</span><span class="sxs-lookup"><span data-stu-id="31ac4-120">Int32</span></span>  |
| <span data-ttu-id="31ac4-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="31ac4-121">reportDate</span></span>        | <span data-ttu-id="31ac4-122">Data</span><span class="sxs-lookup"><span data-stu-id="31ac4-122">Date</span></span>   |
| <span data-ttu-id="31ac4-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="31ac4-123">reportPeriod</span></span>      | <span data-ttu-id="31ac4-124">String</span><span class="sxs-lookup"><span data-stu-id="31ac4-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="31ac4-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31ac4-125">JSON representation</span></span>

<span data-ttu-id="31ac4-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="31ac4-126">The following is a JSON representation of the resource.</span></span>

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
