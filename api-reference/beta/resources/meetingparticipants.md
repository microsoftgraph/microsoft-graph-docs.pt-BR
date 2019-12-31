---
title: tipo de recurso meetingParticipants
description: Participantes de uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 66bb521ae9a2222b5ea60709ac3687da930161d6
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913552"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="708c2-103">tipo de recurso meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="708c2-103">meetingParticipants resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="708c2-104">Participantes de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="708c2-104">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="708c2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="708c2-105">Properties</span></span>

| <span data-ttu-id="708c2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="708c2-106">Property</span></span>       | <span data-ttu-id="708c2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="708c2-107">Type</span></span>    | <span data-ttu-id="708c2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="708c2-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="708c2-109">attendees</span><span class="sxs-lookup"><span data-stu-id="708c2-109">attendees</span></span> | <span data-ttu-id="708c2-110">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="708c2-110">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="708c2-111">organizer</span><span class="sxs-lookup"><span data-stu-id="708c2-111">organizer</span></span> | [<span data-ttu-id="708c2-112">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="708c2-112">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |
| <span data-ttu-id="708c2-113">produtores</span><span class="sxs-lookup"><span data-stu-id="708c2-113">producers</span></span> | <span data-ttu-id="708c2-114">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="708c2-114">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="708c2-115">Somente para reunião de transmissão.</span><span class="sxs-lookup"><span data-stu-id="708c2-115">For broadcast meeting only.</span></span> |
| <span data-ttu-id="708c2-116">colaboradores</span><span class="sxs-lookup"><span data-stu-id="708c2-116">contributors</span></span> | <span data-ttu-id="708c2-117">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="708c2-117">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="708c2-118">Somente para reunião de transmissão.</span><span class="sxs-lookup"><span data-stu-id="708c2-118">For broadcast meeting only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="708c2-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="708c2-119">JSON representation</span></span>

<span data-ttu-id="708c2-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="708c2-120">The following is a JSON representation of the resource.</span></span>

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
