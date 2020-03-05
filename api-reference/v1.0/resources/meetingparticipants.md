---
title: tipo de recurso meetingParticipants
description: Participantes de uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dd00cbf5ce8395a819136ad9e655fa7670e5f3fa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447413"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="c6a62-103">tipo de recurso meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="c6a62-103">meetingParticipants resource type</span></span>

<span data-ttu-id="c6a62-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c6a62-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c6a62-105">Participantes de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="c6a62-105">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="c6a62-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6a62-106">Properties</span></span>

| <span data-ttu-id="c6a62-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6a62-107">Property</span></span>       | <span data-ttu-id="c6a62-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6a62-108">Type</span></span>    | <span data-ttu-id="c6a62-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6a62-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c6a62-110">attendees</span><span class="sxs-lookup"><span data-stu-id="c6a62-110">attendees</span></span> | <span data-ttu-id="c6a62-111">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="c6a62-111">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="c6a62-112">organizer</span><span class="sxs-lookup"><span data-stu-id="c6a62-112">organizer</span></span> | [<span data-ttu-id="c6a62-113">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="c6a62-113">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="c6a62-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6a62-114">JSON representation</span></span>

<span data-ttu-id="c6a62-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c6a62-115">The following is a JSON representation of the resource.</span></span>

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
