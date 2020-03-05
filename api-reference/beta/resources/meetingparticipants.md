---
title: tipo de recurso meetingParticipants
description: Participantes de uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 38071e4ab18127ca8f49b4ef4befdfafbf4c7e04
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522719"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="8c8e1-103">tipo de recurso meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="8c8e1-103">meetingParticipants resource type</span></span>

<span data-ttu-id="8c8e1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8c8e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c8e1-105">Participantes de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="8c8e1-105">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="8c8e1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c8e1-106">Properties</span></span>

| <span data-ttu-id="8c8e1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c8e1-107">Property</span></span>       | <span data-ttu-id="8c8e1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c8e1-108">Type</span></span>    | <span data-ttu-id="8c8e1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c8e1-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8c8e1-110">attendees</span><span class="sxs-lookup"><span data-stu-id="8c8e1-110">attendees</span></span> | <span data-ttu-id="8c8e1-111">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="8c8e1-111">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="8c8e1-112">organizer</span><span class="sxs-lookup"><span data-stu-id="8c8e1-112">organizer</span></span> | [<span data-ttu-id="8c8e1-113">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="8c8e1-113">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |
| <span data-ttu-id="8c8e1-114">produtores</span><span class="sxs-lookup"><span data-stu-id="8c8e1-114">producers</span></span> | <span data-ttu-id="8c8e1-115">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="8c8e1-115">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="8c8e1-116">Somente para reunião de transmissão.</span><span class="sxs-lookup"><span data-stu-id="8c8e1-116">For broadcast meeting only.</span></span> |
| <span data-ttu-id="8c8e1-117">colaboradores</span><span class="sxs-lookup"><span data-stu-id="8c8e1-117">contributors</span></span> | <span data-ttu-id="8c8e1-118">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="8c8e1-118">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="8c8e1-119">Somente para reunião de transmissão.</span><span class="sxs-lookup"><span data-stu-id="8c8e1-119">For broadcast meeting only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8c8e1-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c8e1-120">JSON representation</span></span>

<span data-ttu-id="8c8e1-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c8e1-121">The following is a JSON representation of the resource.</span></span>

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
