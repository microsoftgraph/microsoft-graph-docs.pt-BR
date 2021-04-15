---
title: Tipo de recurso teamsUserActivityUserCounts
description: Representa números de usuários diários por tipo de atividade.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f1ddb3e6e5e6a0b6fbb5c9973bec7e29f4492089
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766438"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="18ca9-103">Tipo de recurso teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="18ca9-103">teamsUserActivityUserCounts resource type</span></span>

<span data-ttu-id="18ca9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18ca9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18ca9-105">Representa números de usuários diários por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="18ca9-105">Represents numbers of daily users by activity type.</span></span>

## <a name="properties"></a><span data-ttu-id="18ca9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18ca9-106">Properties</span></span>

| <span data-ttu-id="18ca9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18ca9-107">Property</span></span>            | <span data-ttu-id="18ca9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="18ca9-108">Type</span></span>   | <span data-ttu-id="18ca9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="18ca9-109">Description</span></span>                                                  |
| :------------------ | :----- | ------------------------------------------------------------ |
| <span data-ttu-id="18ca9-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="18ca9-110">reportRefreshDate</span></span>   | <span data-ttu-id="18ca9-111">Data</span><span class="sxs-lookup"><span data-stu-id="18ca9-111">Date</span></span>   | <span data-ttu-id="18ca9-112">A data mais recente do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="18ca9-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="18ca9-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="18ca9-113">reportDate</span></span>          | <span data-ttu-id="18ca9-114">Data</span><span class="sxs-lookup"><span data-stu-id="18ca9-114">Date</span></span>   | <span data-ttu-id="18ca9-115">A data em que os usuários realizaram as atividades.</span><span class="sxs-lookup"><span data-stu-id="18ca9-115">The date on which the users performed the activities.</span></span>        |
| <span data-ttu-id="18ca9-116">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="18ca9-116">teamChatMessages</span></span>    | <span data-ttu-id="18ca9-117">Int64</span><span class="sxs-lookup"><span data-stu-id="18ca9-117">Int64</span></span>  | <span data-ttu-id="18ca9-118">O número de usuários que postaram mensagens em um chat de equipe.</span><span class="sxs-lookup"><span data-stu-id="18ca9-118">The number of users who posted message in a team chat.</span></span>       |
| <span data-ttu-id="18ca9-119">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="18ca9-119">privateChatMessages</span></span> | <span data-ttu-id="18ca9-120">Int64</span><span class="sxs-lookup"><span data-stu-id="18ca9-120">Int64</span></span>  | <span data-ttu-id="18ca9-121">O número de usuários que postaram mensagens em um chat privado.</span><span class="sxs-lookup"><span data-stu-id="18ca9-121">The number of users who posted message in a private chat.</span></span>    |
| <span data-ttu-id="18ca9-122">calls</span><span class="sxs-lookup"><span data-stu-id="18ca9-122">calls</span></span>               | <span data-ttu-id="18ca9-123">Int64</span><span class="sxs-lookup"><span data-stu-id="18ca9-123">Int64</span></span>  | <span data-ttu-id="18ca9-124">O número de usuários que participaram de chamadas 1:1.</span><span class="sxs-lookup"><span data-stu-id="18ca9-124">The number of users who participated in 1:1 calls.</span></span>           |
| <span data-ttu-id="18ca9-125">meetings</span><span class="sxs-lookup"><span data-stu-id="18ca9-125">meetings</span></span>            | <span data-ttu-id="18ca9-126">Int64</span><span class="sxs-lookup"><span data-stu-id="18ca9-126">Int64</span></span>  | <span data-ttu-id="18ca9-127">O número de usuários que participaram de reuniões online.</span><span class="sxs-lookup"><span data-stu-id="18ca9-127">The number of users who participated in online meetings.</span></span>     |
| <span data-ttu-id="18ca9-128">otherActions</span><span class="sxs-lookup"><span data-stu-id="18ca9-128">otherActions</span></span>        | <span data-ttu-id="18ca9-129">Int64</span><span class="sxs-lookup"><span data-stu-id="18ca9-129">Int64</span></span>  | <span data-ttu-id="18ca9-130">O número de usuários que estavam ativos, mas realizaram outras atividades que não os tipos de ação expostos oferecidos no relatório (enviando ou respondendo a mensagens de canal e mensagens de chat, agendando ou participando de chamadas e reuniões 1:1).</span><span class="sxs-lookup"><span data-stu-id="18ca9-130">The number of users who were active but performed other activities than exposed action types offered in the report (sending or replying to channel messages and chat messages, scheduling or participating in 1:1 calls and meetings).</span></span> <span data-ttu-id="18ca9-131">Exemplos de ações são quando um usuário altera o status do Teams ou a mensagem de status do Teams ou abre uma postagem mensagem de canal, mas não responde.</span><span class="sxs-lookup"><span data-stu-id="18ca9-131">Examples actions are when a user changes the Teams status or the Teams status message or opens a Channel Message post but does not reply.</span></span> |
| <span data-ttu-id="18ca9-132">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="18ca9-132">reportPeriod</span></span>        | <span data-ttu-id="18ca9-133">String</span><span class="sxs-lookup"><span data-stu-id="18ca9-133">String</span></span> | <span data-ttu-id="18ca9-134">O número de dias que o relatório aborda.</span><span class="sxs-lookup"><span data-stu-id="18ca9-134">The number of days the report covers.</span></span>                        |

## <a name="json-representation"></a><span data-ttu-id="18ca9-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18ca9-135">JSON representation</span></span>

<span data-ttu-id="18ca9-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18ca9-136">The following is a JSON representation of the resource.</span></span>

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


