---
title: tipo de recurso de teamsUserActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
ms.openlocfilehash: f4e10f1e34d4c6bdbed83279b98632c504630bc7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330454"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="45ac2-103">tipo de recurso de teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="45ac2-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="45ac2-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45ac2-104">Properties</span></span>

| <span data-ttu-id="45ac2-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45ac2-105">Property</span></span>            | <span data-ttu-id="45ac2-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="45ac2-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="45ac2-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="45ac2-107">reportRefreshDate</span></span>   | <span data-ttu-id="45ac2-108">Data</span><span class="sxs-lookup"><span data-stu-id="45ac2-108">Date</span></span>   |
| <span data-ttu-id="45ac2-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="45ac2-109">reportDate</span></span>          | <span data-ttu-id="45ac2-110">Data</span><span class="sxs-lookup"><span data-stu-id="45ac2-110">Date</span></span>   |
| <span data-ttu-id="45ac2-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="45ac2-111">teamChatMessages</span></span>    | <span data-ttu-id="45ac2-112">Int64</span><span class="sxs-lookup"><span data-stu-id="45ac2-112">Int64</span></span>  |
| <span data-ttu-id="45ac2-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="45ac2-113">privateChatMessages</span></span> | <span data-ttu-id="45ac2-114">Int64</span><span class="sxs-lookup"><span data-stu-id="45ac2-114">Int64</span></span>  |
| <span data-ttu-id="45ac2-115">chamadas</span><span class="sxs-lookup"><span data-stu-id="45ac2-115">calls</span></span>               | <span data-ttu-id="45ac2-116">Int64</span><span class="sxs-lookup"><span data-stu-id="45ac2-116">Int64</span></span>  |
| <span data-ttu-id="45ac2-117">reuniões</span><span class="sxs-lookup"><span data-stu-id="45ac2-117">meetings</span></span>            | <span data-ttu-id="45ac2-118">Int64</span><span class="sxs-lookup"><span data-stu-id="45ac2-118">Int64</span></span>  |
| <span data-ttu-id="45ac2-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="45ac2-119">otherActions</span></span>        | <span data-ttu-id="45ac2-120">Int64</span><span class="sxs-lookup"><span data-stu-id="45ac2-120">Int64</span></span>  |
| <span data-ttu-id="45ac2-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="45ac2-121">reportPeriod</span></span>        | <span data-ttu-id="45ac2-122">String</span><span class="sxs-lookup"><span data-stu-id="45ac2-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="45ac2-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45ac2-123">JSON representation</span></span>

<span data-ttu-id="45ac2-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="45ac2-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```
