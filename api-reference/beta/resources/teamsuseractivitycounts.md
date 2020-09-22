---
title: tipo de recurso teamsUserActivityCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 68eb66cbd0e076d9cf2559170fee4c81dca1e65c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046339"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="c48fd-103">tipo de recurso teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="c48fd-103">teamsUserActivityCounts resource type</span></span>

<span data-ttu-id="c48fd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c48fd-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c48fd-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c48fd-105">Properties</span></span>

| <span data-ttu-id="c48fd-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c48fd-106">Property</span></span>            | <span data-ttu-id="c48fd-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c48fd-107">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="c48fd-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c48fd-108">reportRefreshDate</span></span>   | <span data-ttu-id="c48fd-109">Data</span><span class="sxs-lookup"><span data-stu-id="c48fd-109">Date</span></span>   |
| <span data-ttu-id="c48fd-110">reportDate</span><span class="sxs-lookup"><span data-stu-id="c48fd-110">reportDate</span></span>          | <span data-ttu-id="c48fd-111">Data</span><span class="sxs-lookup"><span data-stu-id="c48fd-111">Date</span></span>   |
| <span data-ttu-id="c48fd-112">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="c48fd-112">teamChatMessages</span></span>    | <span data-ttu-id="c48fd-113">Int64</span><span class="sxs-lookup"><span data-stu-id="c48fd-113">Int64</span></span>  |
| <span data-ttu-id="c48fd-114">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="c48fd-114">privateChatMessages</span></span> | <span data-ttu-id="c48fd-115">Int64</span><span class="sxs-lookup"><span data-stu-id="c48fd-115">Int64</span></span>  |
| <span data-ttu-id="c48fd-116">calls</span><span class="sxs-lookup"><span data-stu-id="c48fd-116">calls</span></span>               | <span data-ttu-id="c48fd-117">Int64</span><span class="sxs-lookup"><span data-stu-id="c48fd-117">Int64</span></span>  |
| <span data-ttu-id="c48fd-118">treinamento</span><span class="sxs-lookup"><span data-stu-id="c48fd-118">meetings</span></span>            | <span data-ttu-id="c48fd-119">Int64</span><span class="sxs-lookup"><span data-stu-id="c48fd-119">Int64</span></span>  |
| <span data-ttu-id="c48fd-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c48fd-120">reportPeriod</span></span>        | <span data-ttu-id="c48fd-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c48fd-121">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c48fd-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c48fd-122">JSON representation</span></span>

<span data-ttu-id="c48fd-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c48fd-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```


