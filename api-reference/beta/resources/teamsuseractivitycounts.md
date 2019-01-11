---
title: tipo de recurso de teamsUserActivityCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: c7351795f6b3dafbac996844fc1ac11cd24bbc03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886587"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="83959-103">tipo de recurso de teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="83959-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="83959-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83959-104">Properties</span></span>

| <span data-ttu-id="83959-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83959-105">Property</span></span>            | <span data-ttu-id="83959-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="83959-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="83959-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="83959-107">reportRefreshDate</span></span>   | <span data-ttu-id="83959-108">Data</span><span class="sxs-lookup"><span data-stu-id="83959-108">Date</span></span>   |
| <span data-ttu-id="83959-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="83959-109">reportDate</span></span>          | <span data-ttu-id="83959-110">Data</span><span class="sxs-lookup"><span data-stu-id="83959-110">Date</span></span>   |
| <span data-ttu-id="83959-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="83959-111">teamChatMessages</span></span>    | <span data-ttu-id="83959-112">Int64</span><span class="sxs-lookup"><span data-stu-id="83959-112">Int64</span></span>  |
| <span data-ttu-id="83959-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="83959-113">privateChatMessages</span></span> | <span data-ttu-id="83959-114">Int64</span><span class="sxs-lookup"><span data-stu-id="83959-114">Int64</span></span>  |
| <span data-ttu-id="83959-115">chamadas</span><span class="sxs-lookup"><span data-stu-id="83959-115">calls</span></span>               | <span data-ttu-id="83959-116">Int64</span><span class="sxs-lookup"><span data-stu-id="83959-116">Int64</span></span>  |
| <span data-ttu-id="83959-117">reuniões</span><span class="sxs-lookup"><span data-stu-id="83959-117">meetings</span></span>            | <span data-ttu-id="83959-118">Int64</span><span class="sxs-lookup"><span data-stu-id="83959-118">Int64</span></span>  |
| <span data-ttu-id="83959-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="83959-119">reportPeriod</span></span>        | <span data-ttu-id="83959-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83959-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="83959-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83959-121">JSON representation</span></span>

<span data-ttu-id="83959-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83959-122">The following is a JSON representation of the resource.</span></span>

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
