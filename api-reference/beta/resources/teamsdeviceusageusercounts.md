---
title: tipo de recurso teamsDeviceUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 99cb675880962591d6298062f979f0930bc0a15d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964393"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="10744-103">tipo de recurso teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="10744-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="10744-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10744-104">Properties</span></span>

| <span data-ttu-id="10744-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10744-105">Property</span></span>          | <span data-ttu-id="10744-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="10744-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="10744-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="10744-107">reportRefreshDate</span></span> | <span data-ttu-id="10744-108">Data</span><span class="sxs-lookup"><span data-stu-id="10744-108">Date</span></span>   |
| <span data-ttu-id="10744-109">web</span><span class="sxs-lookup"><span data-stu-id="10744-109">web</span></span>               | <span data-ttu-id="10744-110">Int64</span><span class="sxs-lookup"><span data-stu-id="10744-110">Int64</span></span>  |
| <span data-ttu-id="10744-111">Windowsphonee</span><span class="sxs-lookup"><span data-stu-id="10744-111">windowsPhone</span></span>      | <span data-ttu-id="10744-112">Int64</span><span class="sxs-lookup"><span data-stu-id="10744-112">Int64</span></span>  |
| <span data-ttu-id="10744-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="10744-113">androidPhone</span></span>      | <span data-ttu-id="10744-114">Int64</span><span class="sxs-lookup"><span data-stu-id="10744-114">Int64</span></span>  |
| <span data-ttu-id="10744-115">emiti</span><span class="sxs-lookup"><span data-stu-id="10744-115">ios</span></span>               | <span data-ttu-id="10744-116">Int64</span><span class="sxs-lookup"><span data-stu-id="10744-116">Int64</span></span>  |
| <span data-ttu-id="10744-117">mac</span><span class="sxs-lookup"><span data-stu-id="10744-117">mac</span></span>               | <span data-ttu-id="10744-118">Int64</span><span class="sxs-lookup"><span data-stu-id="10744-118">Int64</span></span>  |
| <span data-ttu-id="10744-119">Windows</span><span class="sxs-lookup"><span data-stu-id="10744-119">windows</span></span>           | <span data-ttu-id="10744-120">Int64</span><span class="sxs-lookup"><span data-stu-id="10744-120">Int64</span></span>  |
| <span data-ttu-id="10744-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="10744-121">reportDate</span></span>        | <span data-ttu-id="10744-122">Data</span><span class="sxs-lookup"><span data-stu-id="10744-122">Date</span></span>   |
| <span data-ttu-id="10744-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="10744-123">reportPeriod</span></span>      | <span data-ttu-id="10744-124">String</span><span class="sxs-lookup"><span data-stu-id="10744-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="10744-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10744-125">JSON representation</span></span>

<span data-ttu-id="10744-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10744-126">The following is a JSON representation of the resource.</span></span>

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
