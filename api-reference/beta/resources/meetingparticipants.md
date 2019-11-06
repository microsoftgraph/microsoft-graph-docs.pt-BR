---
title: tipo de recurso meetingParticipants
description: Participantes de uma reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 171d24629c8a219f788ad17cdf97874bbf299a62
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006624"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="cbef6-103">tipo de recurso meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="cbef6-103">meetingParticipants resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbef6-104">Participantes de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="cbef6-104">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="cbef6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cbef6-105">Properties</span></span>

| <span data-ttu-id="cbef6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbef6-106">Property</span></span>       | <span data-ttu-id="cbef6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbef6-107">Type</span></span>    | <span data-ttu-id="cbef6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbef6-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cbef6-109">attendees</span><span class="sxs-lookup"><span data-stu-id="cbef6-109">attendees</span></span> | <span data-ttu-id="cbef6-110">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="cbef6-110">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="cbef6-111">organizer</span><span class="sxs-lookup"><span data-stu-id="cbef6-111">organizer</span></span> | [<span data-ttu-id="cbef6-112">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="cbef6-112">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |
| <span data-ttu-id="cbef6-113">produtores</span><span class="sxs-lookup"><span data-stu-id="cbef6-113">producers</span></span> | <span data-ttu-id="cbef6-114">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="cbef6-114">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="cbef6-115">Somente para reunião de transmissão.</span><span class="sxs-lookup"><span data-stu-id="cbef6-115">For broadcast meeting only.</span></span> |
| <span data-ttu-id="cbef6-116">colaboradores</span><span class="sxs-lookup"><span data-stu-id="cbef6-116">contributors</span></span> | <span data-ttu-id="cbef6-117">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="cbef6-117">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="cbef6-118">Somente para reunião de transmissão.</span><span class="sxs-lookup"><span data-stu-id="cbef6-118">For broadcast meeting only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cbef6-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cbef6-119">JSON representation</span></span>

<span data-ttu-id="cbef6-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cbef6-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"},
  "producers": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "contributors": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
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
