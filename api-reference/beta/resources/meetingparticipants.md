---
title: tipo de recurso meetingParticipants
description: Participantes de uma reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f6446ec0b896854e2566d4de82acfdb53bee893d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342405"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="adef8-103">tipo de recurso meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="adef8-103">meetingParticipants resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adef8-104">Participantes de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="adef8-104">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="adef8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="adef8-105">Properties</span></span>

| <span data-ttu-id="adef8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="adef8-106">Property</span></span>       | <span data-ttu-id="adef8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="adef8-107">Type</span></span>    | <span data-ttu-id="adef8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="adef8-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="adef8-109">attendees</span><span class="sxs-lookup"><span data-stu-id="adef8-109">attendees</span></span> | <span data-ttu-id="adef8-110">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="adef8-110">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="adef8-111">organizer</span><span class="sxs-lookup"><span data-stu-id="adef8-111">organizer</span></span> | [<span data-ttu-id="adef8-112">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="adef8-112">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="adef8-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="adef8-113">JSON representation</span></span>

<span data-ttu-id="adef8-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="adef8-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"}
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
