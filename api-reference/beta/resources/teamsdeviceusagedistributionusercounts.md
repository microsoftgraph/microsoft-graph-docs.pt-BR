---
title: tipo de recurso teamsDeviceUsageDistributionUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c6b10af0e4b32c37a5fe365dc8deedae63efc8c4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519873"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="95c6d-103">tipo de recurso teamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="95c6d-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="95c6d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="95c6d-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="95c6d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95c6d-105">Properties</span></span>

| <span data-ttu-id="95c6d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95c6d-106">Property</span></span>          | <span data-ttu-id="95c6d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="95c6d-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="95c6d-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="95c6d-108">reportRefreshDate</span></span> | <span data-ttu-id="95c6d-109">Data</span><span class="sxs-lookup"><span data-stu-id="95c6d-109">Date</span></span>   |
| <span data-ttu-id="95c6d-110">web</span><span class="sxs-lookup"><span data-stu-id="95c6d-110">web</span></span>               | <span data-ttu-id="95c6d-111">Int64</span><span class="sxs-lookup"><span data-stu-id="95c6d-111">Int64</span></span>  |
| <span data-ttu-id="95c6d-112">Windowsphonee</span><span class="sxs-lookup"><span data-stu-id="95c6d-112">windowsPhone</span></span>      | <span data-ttu-id="95c6d-113">Int64</span><span class="sxs-lookup"><span data-stu-id="95c6d-113">Int64</span></span>  |
| <span data-ttu-id="95c6d-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="95c6d-114">androidPhone</span></span>      | <span data-ttu-id="95c6d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="95c6d-115">Int64</span></span>  |
| <span data-ttu-id="95c6d-116">emiti</span><span class="sxs-lookup"><span data-stu-id="95c6d-116">ios</span></span>               | <span data-ttu-id="95c6d-117">Int64</span><span class="sxs-lookup"><span data-stu-id="95c6d-117">Int64</span></span>  |
| <span data-ttu-id="95c6d-118">mac</span><span class="sxs-lookup"><span data-stu-id="95c6d-118">mac</span></span>               | <span data-ttu-id="95c6d-119">Int64</span><span class="sxs-lookup"><span data-stu-id="95c6d-119">Int64</span></span>  |
| <span data-ttu-id="95c6d-120">Windows</span><span class="sxs-lookup"><span data-stu-id="95c6d-120">windows</span></span>           | <span data-ttu-id="95c6d-121">Int64</span><span class="sxs-lookup"><span data-stu-id="95c6d-121">Int64</span></span>  |
| <span data-ttu-id="95c6d-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="95c6d-122">reportPeriod</span></span>      | <span data-ttu-id="95c6d-123">String</span><span class="sxs-lookup"><span data-stu-id="95c6d-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="95c6d-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95c6d-124">JSON representation</span></span>

<span data-ttu-id="95c6d-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95c6d-125">The following is a JSON representation of the resource.</span></span>

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
