---
title: tipo de recurso de teamsDeviceUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 07a43b024d133e5ac1d8eb8a2665fd3027001edb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857348"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="f1fff-103">tipo de recurso de teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="f1fff-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f1fff-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1fff-104">Properties</span></span>

| <span data-ttu-id="f1fff-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1fff-105">Property</span></span>          | <span data-ttu-id="f1fff-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1fff-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f1fff-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f1fff-107">reportRefreshDate</span></span> | <span data-ttu-id="f1fff-108">Data</span><span class="sxs-lookup"><span data-stu-id="f1fff-108">Date</span></span>   |
| <span data-ttu-id="f1fff-109">web</span><span class="sxs-lookup"><span data-stu-id="f1fff-109">web</span></span>               | <span data-ttu-id="f1fff-110">Int64</span><span class="sxs-lookup"><span data-stu-id="f1fff-110">Int64</span></span>  |
| <span data-ttu-id="f1fff-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="f1fff-111">windowsPhone</span></span>      | <span data-ttu-id="f1fff-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f1fff-112">Int64</span></span>  |
| <span data-ttu-id="f1fff-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="f1fff-113">androidPhone</span></span>      | <span data-ttu-id="f1fff-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f1fff-114">Int64</span></span>  |
| <span data-ttu-id="f1fff-115">IOS</span><span class="sxs-lookup"><span data-stu-id="f1fff-115">ios</span></span>               | <span data-ttu-id="f1fff-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f1fff-116">Int64</span></span>  |
| <span data-ttu-id="f1fff-117">mac</span><span class="sxs-lookup"><span data-stu-id="f1fff-117">mac</span></span>               | <span data-ttu-id="f1fff-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f1fff-118">Int64</span></span>  |
| <span data-ttu-id="f1fff-119">Windows</span><span class="sxs-lookup"><span data-stu-id="f1fff-119">windows</span></span>           | <span data-ttu-id="f1fff-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f1fff-120">Int64</span></span>  |
| <span data-ttu-id="f1fff-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="f1fff-121">reportDate</span></span>        | <span data-ttu-id="f1fff-122">Data</span><span class="sxs-lookup"><span data-stu-id="f1fff-122">Date</span></span>   |
| <span data-ttu-id="f1fff-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f1fff-123">reportPeriod</span></span>      | <span data-ttu-id="f1fff-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1fff-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f1fff-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1fff-125">JSON representation</span></span>

<span data-ttu-id="f1fff-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1fff-126">The following is a JSON representation of the resource.</span></span>

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
