---
title: Tipo de recurso meetingTimeSuggestion
description: 'Uma sugestão de reunião que inclui informações como o horário da reunião, a probabilidade de presença, individual '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d0f6c36d0fb76c1bc115b9cd0490a79a3f94a77b
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936231"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="f4011-103">Tipo de recurso meetingTimeSuggestion</span><span class="sxs-lookup"><span data-stu-id="f4011-103">meetingTimeSuggestion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4011-104">Uma sugestão de reunião que inclui informações como o horário da reunião, a probabilidade de presença, a disponibilidade individual e os locais de reunião disponíveis.</span><span class="sxs-lookup"><span data-stu-id="f4011-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4011-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4011-105">JSON representation</span></span>

<span data-ttu-id="f4011-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f4011-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 1024.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="f4011-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4011-107">Properties</span></span>
| <span data-ttu-id="f4011-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4011-108">Property</span></span>     | <span data-ttu-id="f4011-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4011-109">Type</span></span>   |<span data-ttu-id="f4011-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4011-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4011-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="f4011-111">attendeeAvailability</span></span>|<span data-ttu-id="f4011-112">Coleção [attendeeAvailability](attendeeavailability.md)</span><span class="sxs-lookup"><span data-stu-id="f4011-112">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="f4011-113">Uma matriz que mostra o status de disponibilidade de cada participante para essa sugestão da reunião.</span><span class="sxs-lookup"><span data-stu-id="f4011-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="f4011-114">confidence</span><span class="sxs-lookup"><span data-stu-id="f4011-114">confidence</span></span>|<span data-ttu-id="f4011-115">Double</span><span class="sxs-lookup"><span data-stu-id="f4011-115">Double</span></span>|<span data-ttu-id="f4011-116">Uma porcentagem que representa a probabilidade de todos os participantes comparecerem.</span><span class="sxs-lookup"><span data-stu-id="f4011-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="f4011-117">locations</span><span class="sxs-lookup"><span data-stu-id="f4011-117">locations</span></span>|<span data-ttu-id="f4011-118">Coleção [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="f4011-118">[location](location.md) collection</span></span>|<span data-ttu-id="f4011-119">Uma matriz que especifica o nome e a localização geográfica de cada local da reunião para esta sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="f4011-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="f4011-120">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="f4011-120">meetingTimeSlot</span></span>|[<span data-ttu-id="f4011-121">timeSlot</span><span class="sxs-lookup"><span data-stu-id="f4011-121">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="f4011-122">Um período de tempo sugerido para a reunião.</span><span class="sxs-lookup"><span data-stu-id="f4011-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="f4011-123">Ordene</span><span class="sxs-lookup"><span data-stu-id="f4011-123">order</span></span>|<span data-ttu-id="f4011-124">Int32</span><span class="sxs-lookup"><span data-stu-id="f4011-124">Int32</span></span>|<span data-ttu-id="f4011-125">Ordem das sugestões de horário de reunião classificadas pelo valor de confiança computado de alto para baixo e, em seguida, por cronologia, se houver sugestões com a mesma confiança.</span><span class="sxs-lookup"><span data-stu-id="f4011-125">Order of meeting time suggestions sorted by their computed confidence value from high to low, then by chronology if there are suggestions with the same confidence.</span></span> |
|<span data-ttu-id="f4011-126">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="f4011-126">organizerAvailability</span></span>|<span data-ttu-id="f4011-127">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="f4011-127">availabilityStatus</span></span>| <span data-ttu-id="f4011-p101">Disponibilidade do organizador da reunião para essa sugestão de reunião. Os possíveis valores são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f4011-p101">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="f4011-130">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="f4011-130">suggestionReason</span></span>|<span data-ttu-id="f4011-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4011-131">String</span></span>|<span data-ttu-id="f4011-132">Razão da sugestão de horário da reunião.</span><span class="sxs-lookup"><span data-stu-id="f4011-132">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimesuggestion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
