---
title: Tipo de recurso teamsUserActivityCounts
description: Representa numers de atividades por tipo.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7e931d3488fce488710c638a0155ef0c5dd3a521
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766088"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="513d8-103">Tipo de recurso teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="513d8-103">teamsUserActivityCounts resource type</span></span>

<span data-ttu-id="513d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="513d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="513d8-105">Representa numers de atividades por tipo.</span><span class="sxs-lookup"><span data-stu-id="513d8-105">Represents numers of activities by type.</span></span>

## <a name="properties"></a><span data-ttu-id="513d8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="513d8-106">Properties</span></span>

| <span data-ttu-id="513d8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="513d8-107">Property</span></span>            | <span data-ttu-id="513d8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="513d8-108">Type</span></span>   | <span data-ttu-id="513d8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="513d8-109">Description</span></span>                                                  |
| :------------------ | :----- | ------------------------------------------------------------ |
| <span data-ttu-id="513d8-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="513d8-110">reportRefreshDate</span></span>   | <span data-ttu-id="513d8-111">Data</span><span class="sxs-lookup"><span data-stu-id="513d8-111">Date</span></span>   | <span data-ttu-id="513d8-112">A data mais recente do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="513d8-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="513d8-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="513d8-113">reportDate</span></span>          | <span data-ttu-id="513d8-114">Data</span><span class="sxs-lookup"><span data-stu-id="513d8-114">Date</span></span>   | <span data-ttu-id="513d8-115">A data em que os usuários realizaram as atividades.</span><span class="sxs-lookup"><span data-stu-id="513d8-115">The date on which the users performed the activities.</span></span>        |
| <span data-ttu-id="513d8-116">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="513d8-116">teamChatMessages</span></span>    | <span data-ttu-id="513d8-117">Int64</span><span class="sxs-lookup"><span data-stu-id="513d8-117">Int64</span></span>  | <span data-ttu-id="513d8-118">O número de mensagens exclusivas que os usuários postaram em um chat de equipe.</span><span class="sxs-lookup"><span data-stu-id="513d8-118">The number of unique messages that users posted in a team chat.</span></span> |
| <span data-ttu-id="513d8-119">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="513d8-119">privateChatMessages</span></span> | <span data-ttu-id="513d8-120">Int64</span><span class="sxs-lookup"><span data-stu-id="513d8-120">Int64</span></span>  | <span data-ttu-id="513d8-121">O número de mensagens exclusivas que os usuários postaram em um chat privado.</span><span class="sxs-lookup"><span data-stu-id="513d8-121">The number of unique messages that users posted in a private chat.</span></span> |
| <span data-ttu-id="513d8-122">calls</span><span class="sxs-lookup"><span data-stu-id="513d8-122">calls</span></span>               | <span data-ttu-id="513d8-123">Int64</span><span class="sxs-lookup"><span data-stu-id="513d8-123">Int64</span></span>  | <span data-ttu-id="513d8-124">O número de chamadas exclusivas de 1:1 que os usuários participaram.</span><span class="sxs-lookup"><span data-stu-id="513d8-124">The number of unique 1:1 calls that users participated in.</span></span>   |
| <span data-ttu-id="513d8-125">meetings</span><span class="sxs-lookup"><span data-stu-id="513d8-125">meetings</span></span>            | <span data-ttu-id="513d8-126">Int64</span><span class="sxs-lookup"><span data-stu-id="513d8-126">Int64</span></span>  | <span data-ttu-id="513d8-127">O número de reuniões online exclusivas que os usuários participaram.</span><span class="sxs-lookup"><span data-stu-id="513d8-127">The number of unique online meetings that users participated in.</span></span> |
| <span data-ttu-id="513d8-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="513d8-128">reportPeriod</span></span>        | <span data-ttu-id="513d8-129">String</span><span class="sxs-lookup"><span data-stu-id="513d8-129">String</span></span> | <span data-ttu-id="513d8-130">O número de dias que o relatório aborda.</span><span class="sxs-lookup"><span data-stu-id="513d8-130">The number of days the report covers.</span></span>                        |


## <a name="json-representation"></a><span data-ttu-id="513d8-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="513d8-131">JSON representation</span></span>

<span data-ttu-id="513d8-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="513d8-132">The following is a JSON representation of the resource.</span></span>

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


