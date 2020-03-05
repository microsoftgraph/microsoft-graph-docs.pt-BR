---
title: tipo de recurso yammerDeviceUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: ca8a1eaee94f7f125e2d2eb039561286737d58c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519005"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="19619-103">tipo de recurso yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="19619-103">yammerDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="19619-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="19619-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="19619-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="19619-105">Properties</span></span>

| <span data-ttu-id="19619-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19619-106">Property</span></span>          | <span data-ttu-id="19619-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="19619-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="19619-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="19619-108">reportRefreshDate</span></span> | <span data-ttu-id="19619-109">Data</span><span class="sxs-lookup"><span data-stu-id="19619-109">Date</span></span>   |
| <span data-ttu-id="19619-110">web</span><span class="sxs-lookup"><span data-stu-id="19619-110">web</span></span>               | <span data-ttu-id="19619-111">Int32</span><span class="sxs-lookup"><span data-stu-id="19619-111">Int32</span></span>  |
| <span data-ttu-id="19619-112">Windowsphonee</span><span class="sxs-lookup"><span data-stu-id="19619-112">windowsPhone</span></span>      | <span data-ttu-id="19619-113">Int32</span><span class="sxs-lookup"><span data-stu-id="19619-113">Int32</span></span>  |
| <span data-ttu-id="19619-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="19619-114">androidPhone</span></span>      | <span data-ttu-id="19619-115">Int32</span><span class="sxs-lookup"><span data-stu-id="19619-115">Int32</span></span>  |
| <span data-ttu-id="19619-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="19619-116">iPhone</span></span>            | <span data-ttu-id="19619-117">Int32</span><span class="sxs-lookup"><span data-stu-id="19619-117">Int32</span></span>  |
| <span data-ttu-id="19619-118">iPad</span><span class="sxs-lookup"><span data-stu-id="19619-118">iPad</span></span>              | <span data-ttu-id="19619-119">Int32</span><span class="sxs-lookup"><span data-stu-id="19619-119">Int32</span></span>  |
| <span data-ttu-id="19619-120">outro</span><span class="sxs-lookup"><span data-stu-id="19619-120">other</span></span>             | <span data-ttu-id="19619-121">Int32</span><span class="sxs-lookup"><span data-stu-id="19619-121">Int32</span></span>  |
| <span data-ttu-id="19619-122">reportDate</span><span class="sxs-lookup"><span data-stu-id="19619-122">reportDate</span></span>        | <span data-ttu-id="19619-123">Data</span><span class="sxs-lookup"><span data-stu-id="19619-123">Date</span></span>   |
| <span data-ttu-id="19619-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="19619-124">reportPeriod</span></span>      | <span data-ttu-id="19619-125">String</span><span class="sxs-lookup"><span data-stu-id="19619-125">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="19619-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="19619-126">JSON representation</span></span>

<span data-ttu-id="19619-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="19619-127">The following is a JSON representation of the resource.</span></span>

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
