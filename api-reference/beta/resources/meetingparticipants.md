---
title: tipo de recurso meetingParticipants
description: Participantes de uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e6d53d0359b9dc71e538c5bbe025e093a4912ffb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971647"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="245dc-103">tipo de recurso meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="245dc-103">meetingParticipants resource type</span></span>

<span data-ttu-id="245dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="245dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="245dc-105">Participantes de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="245dc-105">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="245dc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="245dc-106">Properties</span></span>

| <span data-ttu-id="245dc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="245dc-107">Property</span></span>       | <span data-ttu-id="245dc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="245dc-108">Type</span></span>    | <span data-ttu-id="245dc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="245dc-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="245dc-110">attendees</span><span class="sxs-lookup"><span data-stu-id="245dc-110">attendees</span></span> | <span data-ttu-id="245dc-111">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="245dc-111">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="245dc-112">organizer</span><span class="sxs-lookup"><span data-stu-id="245dc-112">organizer</span></span> | [<span data-ttu-id="245dc-113">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="245dc-113">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |
| <span data-ttu-id="245dc-114">produtores</span><span class="sxs-lookup"><span data-stu-id="245dc-114">producers</span></span> | <span data-ttu-id="245dc-115">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="245dc-115">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="245dc-116">Somente para reunião de transmissão.</span><span class="sxs-lookup"><span data-stu-id="245dc-116">For broadcast meeting only.</span></span> |
| <span data-ttu-id="245dc-117">colaboradores</span><span class="sxs-lookup"><span data-stu-id="245dc-117">contributors</span></span> | <span data-ttu-id="245dc-118">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="245dc-118">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="245dc-119">Somente para reunião de transmissão.</span><span class="sxs-lookup"><span data-stu-id="245dc-119">For broadcast meeting only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="245dc-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="245dc-120">JSON representation</span></span>

<span data-ttu-id="245dc-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="245dc-121">The following is a JSON representation of the resource.</span></span>

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


