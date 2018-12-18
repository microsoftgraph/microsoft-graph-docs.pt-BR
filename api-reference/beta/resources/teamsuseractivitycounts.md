---
title: tipo de recurso de teamsUserActivityCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
ms.openlocfilehash: f67540f4172993b1076d9590438262b0d4da1846
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334514"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="04314-103">tipo de recurso de teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="04314-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="04314-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04314-104">Properties</span></span>

| <span data-ttu-id="04314-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04314-105">Property</span></span>            | <span data-ttu-id="04314-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="04314-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="04314-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="04314-107">reportRefreshDate</span></span>   | <span data-ttu-id="04314-108">Data</span><span class="sxs-lookup"><span data-stu-id="04314-108">Date</span></span>   |
| <span data-ttu-id="04314-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="04314-109">reportDate</span></span>          | <span data-ttu-id="04314-110">Data</span><span class="sxs-lookup"><span data-stu-id="04314-110">Date</span></span>   |
| <span data-ttu-id="04314-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="04314-111">teamChatMessages</span></span>    | <span data-ttu-id="04314-112">Int64</span><span class="sxs-lookup"><span data-stu-id="04314-112">Int64</span></span>  |
| <span data-ttu-id="04314-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="04314-113">privateChatMessages</span></span> | <span data-ttu-id="04314-114">Int64</span><span class="sxs-lookup"><span data-stu-id="04314-114">Int64</span></span>  |
| <span data-ttu-id="04314-115">chamadas</span><span class="sxs-lookup"><span data-stu-id="04314-115">calls</span></span>               | <span data-ttu-id="04314-116">Int64</span><span class="sxs-lookup"><span data-stu-id="04314-116">Int64</span></span>  |
| <span data-ttu-id="04314-117">reuniões</span><span class="sxs-lookup"><span data-stu-id="04314-117">meetings</span></span>            | <span data-ttu-id="04314-118">Int64</span><span class="sxs-lookup"><span data-stu-id="04314-118">Int64</span></span>  |
| <span data-ttu-id="04314-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="04314-119">reportPeriod</span></span>        | <span data-ttu-id="04314-120">String</span><span class="sxs-lookup"><span data-stu-id="04314-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="04314-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04314-121">JSON representation</span></span>

<span data-ttu-id="04314-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04314-122">The following is a JSON representation of the resource.</span></span>

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
