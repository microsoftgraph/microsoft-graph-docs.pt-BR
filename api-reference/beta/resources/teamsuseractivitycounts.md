---
title: tipo de recurso teamsUserActivityCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3066877d109e7dd61243b7cd2f4c105b03c0c533
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519824"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="e4a62-103">tipo de recurso teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="e4a62-103">teamsUserActivityCounts resource type</span></span>

<span data-ttu-id="e4a62-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e4a62-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="e4a62-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e4a62-105">Properties</span></span>

| <span data-ttu-id="e4a62-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4a62-106">Property</span></span>            | <span data-ttu-id="e4a62-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4a62-107">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="e4a62-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e4a62-108">reportRefreshDate</span></span>   | <span data-ttu-id="e4a62-109">Data</span><span class="sxs-lookup"><span data-stu-id="e4a62-109">Date</span></span>   |
| <span data-ttu-id="e4a62-110">reportDate</span><span class="sxs-lookup"><span data-stu-id="e4a62-110">reportDate</span></span>          | <span data-ttu-id="e4a62-111">Data</span><span class="sxs-lookup"><span data-stu-id="e4a62-111">Date</span></span>   |
| <span data-ttu-id="e4a62-112">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="e4a62-112">teamChatMessages</span></span>    | <span data-ttu-id="e4a62-113">Int64</span><span class="sxs-lookup"><span data-stu-id="e4a62-113">Int64</span></span>  |
| <span data-ttu-id="e4a62-114">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="e4a62-114">privateChatMessages</span></span> | <span data-ttu-id="e4a62-115">Int64</span><span class="sxs-lookup"><span data-stu-id="e4a62-115">Int64</span></span>  |
| <span data-ttu-id="e4a62-116">calls</span><span class="sxs-lookup"><span data-stu-id="e4a62-116">calls</span></span>               | <span data-ttu-id="e4a62-117">Int64</span><span class="sxs-lookup"><span data-stu-id="e4a62-117">Int64</span></span>  |
| <span data-ttu-id="e4a62-118">treinamento</span><span class="sxs-lookup"><span data-stu-id="e4a62-118">meetings</span></span>            | <span data-ttu-id="e4a62-119">Int64</span><span class="sxs-lookup"><span data-stu-id="e4a62-119">Int64</span></span>  |
| <span data-ttu-id="e4a62-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e4a62-120">reportPeriod</span></span>        | <span data-ttu-id="e4a62-121">String</span><span class="sxs-lookup"><span data-stu-id="e4a62-121">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="e4a62-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e4a62-122">JSON representation</span></span>

<span data-ttu-id="e4a62-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e4a62-123">The following is a JSON representation of the resource.</span></span>

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
