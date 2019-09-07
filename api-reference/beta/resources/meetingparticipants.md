---
title: tipo de recurso meetingParticipants
description: Participantes de uma reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2d40479390703f50ac87b7c3196aa4d5bc55bc8a
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792762"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="452a5-103">tipo de recurso meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="452a5-103">meetingParticipants resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="452a5-104">Participantes de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="452a5-104">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="452a5-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="452a5-105">Properties</span></span>

| <span data-ttu-id="452a5-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="452a5-106">Property</span></span>       | <span data-ttu-id="452a5-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="452a5-107">Type</span></span>    | <span data-ttu-id="452a5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="452a5-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="452a5-109">attendees</span><span class="sxs-lookup"><span data-stu-id="452a5-109">attendees</span></span> | <span data-ttu-id="452a5-110">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="452a5-110">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="452a5-111">organizer</span><span class="sxs-lookup"><span data-stu-id="452a5-111">organizer</span></span> | [<span data-ttu-id="452a5-112">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="452a5-112">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |
| <span data-ttu-id="452a5-113">produtores</span><span class="sxs-lookup"><span data-stu-id="452a5-113">producers</span></span> | <span data-ttu-id="452a5-114">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="452a5-114">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="452a5-115">Somente para reunião de transmissão.</span><span class="sxs-lookup"><span data-stu-id="452a5-115">For broadcast meeting only.</span></span> |
| <span data-ttu-id="452a5-116">colaboradores</span><span class="sxs-lookup"><span data-stu-id="452a5-116">contributors</span></span> | <span data-ttu-id="452a5-117">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="452a5-117">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> | <span data-ttu-id="452a5-118">Somente para reunião de transmissão.</span><span class="sxs-lookup"><span data-stu-id="452a5-118">For broadcast meeting only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="452a5-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="452a5-119">JSON representation</span></span>

<span data-ttu-id="452a5-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="452a5-120">The following is a JSON representation of the resource.</span></span>

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
