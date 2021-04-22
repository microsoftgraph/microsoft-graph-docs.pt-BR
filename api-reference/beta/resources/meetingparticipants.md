---
title: Tipo de recurso meetingParticipants
description: Participantes em uma reunião.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 93ca3d73518f9739cc3115c80efd2aec551629b5
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944160"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="584f8-103">Tipo de recurso meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="584f8-103">meetingParticipants resource type</span></span>

<span data-ttu-id="584f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="584f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="584f8-105">Participantes em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="584f8-105">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="584f8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="584f8-106">Properties</span></span>

| <span data-ttu-id="584f8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="584f8-107">Property</span></span>                  | <span data-ttu-id="584f8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="584f8-108">Type</span></span>                                                           | <span data-ttu-id="584f8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="584f8-109">Description</span></span>                           |
| :------------------------ | :------------------------------------------------------------- | :------------------------------------ |
| <span data-ttu-id="584f8-110">attendees</span><span class="sxs-lookup"><span data-stu-id="584f8-110">attendees</span></span>                 | <span data-ttu-id="584f8-111">[coleção meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="584f8-111">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="584f8-112">Informações dos participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="584f8-112">Information of the meeting attendees.</span></span> |
| <span data-ttu-id="584f8-113">organizer</span><span class="sxs-lookup"><span data-stu-id="584f8-113">organizer</span></span>                 | [<span data-ttu-id="584f8-114">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="584f8-114">meetingParticipantInfo</span></span>](meetingparticipantinfo.md)            | <span data-ttu-id="584f8-115">Informações do organizador da reunião.</span><span class="sxs-lookup"><span data-stu-id="584f8-115">Information of the meeting organizer.</span></span> |
| <span data-ttu-id="584f8-116">produtores (preterido)</span><span class="sxs-lookup"><span data-stu-id="584f8-116">producers (deprecated)</span></span>    | <span data-ttu-id="584f8-117">[coleção meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="584f8-117">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="584f8-118">Somente para a reunião de transmissão.</span><span class="sxs-lookup"><span data-stu-id="584f8-118">For broadcast meeting only.</span></span>           |
| <span data-ttu-id="584f8-119">colaboradores (preterido)</span><span class="sxs-lookup"><span data-stu-id="584f8-119">contributors (deprecated)</span></span> | <span data-ttu-id="584f8-120">[coleção meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="584f8-120">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="584f8-121">Somente para a reunião de transmissão.</span><span class="sxs-lookup"><span data-stu-id="584f8-121">For broadcast meeting only.</span></span>           |

> [!CAUTION]
> <span data-ttu-id="584f8-122">As **propriedades de produtores** **e** colaboradores são preteridas.</span><span class="sxs-lookup"><span data-stu-id="584f8-122">The **producers** and **contributors** properties are deprecated.</span></span> <span data-ttu-id="584f8-123">Todos os participantes da reunião são retornados **na coleção de participantes.**</span><span class="sxs-lookup"><span data-stu-id="584f8-123">All meeting participants are returned in the **attendees** collection.</span></span> <span data-ttu-id="584f8-124">Use a **propriedade role** de [meetingParticipantInfo](meetingparticipantinfo.md) para identificar a função de reunião do participante.</span><span class="sxs-lookup"><span data-stu-id="584f8-124">Use the **role** property of [meetingParticipantInfo](meetingparticipantinfo.md) to identify the meeting role of the attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="584f8-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="584f8-125">JSON representation</span></span>

<span data-ttu-id="584f8-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="584f8-126">The following is a JSON representation of the resource.</span></span>

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


