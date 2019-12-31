---
title: tipo de recurso meetingParticipants
description: Participantes de uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3bcce64ab900dae7c7f13d7da0c3d34d164fd35d
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913517"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="60e3e-103">tipo de recurso meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="60e3e-103">meetingParticipants resource type</span></span>

<span data-ttu-id="60e3e-104">Participantes de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="60e3e-104">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="60e3e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60e3e-105">Properties</span></span>

| <span data-ttu-id="60e3e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60e3e-106">Property</span></span>       | <span data-ttu-id="60e3e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="60e3e-107">Type</span></span>    | <span data-ttu-id="60e3e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="60e3e-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="60e3e-109">attendees</span><span class="sxs-lookup"><span data-stu-id="60e3e-109">attendees</span></span> | <span data-ttu-id="60e3e-110">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="60e3e-110">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="60e3e-111">organizer</span><span class="sxs-lookup"><span data-stu-id="60e3e-111">organizer</span></span> | [<span data-ttu-id="60e3e-112">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="60e3e-112">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="60e3e-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60e3e-113">JSON representation</span></span>

<span data-ttu-id="60e3e-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60e3e-114">The following is a JSON representation of the resource.</span></span>

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
