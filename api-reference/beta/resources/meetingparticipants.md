---
title: Tipo de recurso meetingParticipants
description: Participantes em uma reunião.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8ee5cf115a80c642f5442230d7111dfaeffca930
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896617"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="0ef03-103">Tipo de recurso meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="0ef03-103">meetingParticipants resource type</span></span>

<span data-ttu-id="0ef03-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ef03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ef03-105">Participantes em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="0ef03-105">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="0ef03-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ef03-106">Properties</span></span>

| <span data-ttu-id="0ef03-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ef03-107">Property</span></span>                  | <span data-ttu-id="0ef03-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ef03-108">Type</span></span>                                                           | <span data-ttu-id="0ef03-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ef03-109">Description</span></span>                           |
| :------------------------ | :------------------------------------------------------------- | :------------------------------------ |
| <span data-ttu-id="0ef03-110">attendees</span><span class="sxs-lookup"><span data-stu-id="0ef03-110">attendees</span></span>                 | <span data-ttu-id="0ef03-111">[coleção meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="0ef03-111">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="0ef03-112">Informações dos participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="0ef03-112">Information of the meeting attendees.</span></span> |
| <span data-ttu-id="0ef03-113">organizer</span><span class="sxs-lookup"><span data-stu-id="0ef03-113">organizer</span></span>                 | [<span data-ttu-id="0ef03-114">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="0ef03-114">meetingParticipantInfo</span></span>](meetingparticipantinfo.md)            | <span data-ttu-id="0ef03-115">Informações do organizador da reunião.</span><span class="sxs-lookup"><span data-stu-id="0ef03-115">Information of the meeting organizer.</span></span> |
| <span data-ttu-id="0ef03-116">produtores (preterido)</span><span class="sxs-lookup"><span data-stu-id="0ef03-116">producers (deprecated)</span></span>    | <span data-ttu-id="0ef03-117">[coleção meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="0ef03-117">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="0ef03-118">Somente para a reunião de transmissão.</span><span class="sxs-lookup"><span data-stu-id="0ef03-118">For broadcast meeting only.</span></span>           |
| <span data-ttu-id="0ef03-119">colaboradores (preterido)</span><span class="sxs-lookup"><span data-stu-id="0ef03-119">contributors (deprecated)</span></span> | <span data-ttu-id="0ef03-120">[coleção meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="0ef03-120">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="0ef03-121">Somente para a reunião de transmissão.</span><span class="sxs-lookup"><span data-stu-id="0ef03-121">For broadcast meeting only.</span></span>           |

> [!CAUTION]
> <span data-ttu-id="0ef03-122">As **propriedades de produtores** **e** colaboradores são preteridas.</span><span class="sxs-lookup"><span data-stu-id="0ef03-122">The **producers** and **contributors** properties are deprecated.</span></span> <span data-ttu-id="0ef03-123">Todos os participantes da reunião são retornados **na coleção de participantes.**</span><span class="sxs-lookup"><span data-stu-id="0ef03-123">All meeting participants are returned in the **attendees** collection.</span></span> <span data-ttu-id="0ef03-124">Use a **propriedade role** de [meetingParticipantInfo](meetingparticipantinfo.md) para identificar a função de reunião do participante.</span><span class="sxs-lookup"><span data-stu-id="0ef03-124">Use the **role** property of [meetingParticipantInfo](meetingparticipantinfo.md) to identify the meeting role of the attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ef03-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ef03-125">JSON representation</span></span>

<span data-ttu-id="0ef03-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ef03-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"},
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipants resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


