---
title: Tipo de recurso teamsUserActivityDistributionUserCounts
description: Representa o número de usuários por tipo de atividade durante o período de tempo selecionado.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3d4fa8b3aec98a03d7e51819db0dc4797367f499
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766905"
---
# <a name="teamsuseractivitydistributionusercounts-resource-type"></a><span data-ttu-id="2d4da-103">Tipo de recurso teamsUserActivityDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="2d4da-103">teamsUserActivityDistributionUserCounts resource type</span></span>

<span data-ttu-id="2d4da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d4da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d4da-105">Representa o número de usuários por tipo de atividade durante o período de tempo selecionado.</span><span class="sxs-lookup"><span data-stu-id="2d4da-105">Represents numbers of users by activity type over the selected time period.</span></span>

## <a name="properties"></a><span data-ttu-id="2d4da-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d4da-106">Properties</span></span>

| <span data-ttu-id="2d4da-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d4da-107">Property</span></span>            | <span data-ttu-id="2d4da-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d4da-108">Type</span></span>   | <span data-ttu-id="2d4da-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d4da-109">Description</span></span>                                                  |
| :------------------ | :----- | ------------------------------------------------------------ |
| <span data-ttu-id="2d4da-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2d4da-110">reportRefreshDate</span></span>   | <span data-ttu-id="2d4da-111">Data</span><span class="sxs-lookup"><span data-stu-id="2d4da-111">Date</span></span>   | <span data-ttu-id="2d4da-112">A data mais recente do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2d4da-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="2d4da-113">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="2d4da-113">teamChatMessages</span></span>    | <span data-ttu-id="2d4da-114">Int64</span><span class="sxs-lookup"><span data-stu-id="2d4da-114">Int64</span></span>  | <span data-ttu-id="2d4da-115">O número de mensagens exclusivas que os usuários postaram em um chat de equipe.</span><span class="sxs-lookup"><span data-stu-id="2d4da-115">The number of unique messages that users posted in a team chat.</span></span> |
| <span data-ttu-id="2d4da-116">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="2d4da-116">privateChatMessages</span></span> | <span data-ttu-id="2d4da-117">Int64</span><span class="sxs-lookup"><span data-stu-id="2d4da-117">Int64</span></span>  | <span data-ttu-id="2d4da-118">O número de mensagens exclusivas que os usuários postaram em um chat privado.</span><span class="sxs-lookup"><span data-stu-id="2d4da-118">The number of unique messages that users posted in a private chat.</span></span> |
| <span data-ttu-id="2d4da-119">calls</span><span class="sxs-lookup"><span data-stu-id="2d4da-119">calls</span></span>               | <span data-ttu-id="2d4da-120">Int64</span><span class="sxs-lookup"><span data-stu-id="2d4da-120">Int64</span></span>  | <span data-ttu-id="2d4da-121">O número de chamadas exclusivas de 1:1 que os usuários participaram.</span><span class="sxs-lookup"><span data-stu-id="2d4da-121">The number of unique 1:1 calls that users participated in.</span></span>   |
| <span data-ttu-id="2d4da-122">meetings</span><span class="sxs-lookup"><span data-stu-id="2d4da-122">meetings</span></span>            | <span data-ttu-id="2d4da-123">Int64</span><span class="sxs-lookup"><span data-stu-id="2d4da-123">Int64</span></span>  | <span data-ttu-id="2d4da-124">O número de reuniões online exclusivas que os usuários participaram.</span><span class="sxs-lookup"><span data-stu-id="2d4da-124">The number of unique online meetings that users participated in.</span></span> |
| <span data-ttu-id="2d4da-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2d4da-125">reportPeriod</span></span>        | <span data-ttu-id="2d4da-126">String</span><span class="sxs-lookup"><span data-stu-id="2d4da-126">String</span></span> | <span data-ttu-id="2d4da-127">O número de dias que o relatório aborda.</span><span class="sxs-lookup"><span data-stu-id="2d4da-127">The number of days the report covers.</span></span>                        |

## <a name="json-representation"></a><span data-ttu-id="2d4da-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d4da-128">JSON representation</span></span>

<span data-ttu-id="2d4da-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d4da-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```


