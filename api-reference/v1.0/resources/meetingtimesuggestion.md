---
title: Tipo de recurso meetingTimeSuggestion
description: 'Uma sugestão de reunião que inclui informações como hora da reunião, probabilidade de participação, individual '
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5340fa9912ecb183dda8603d4b3ce4bbf6d70e8d
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474698"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="d4889-103">Tipo de recurso meetingTimeSuggestion</span><span class="sxs-lookup"><span data-stu-id="d4889-103">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="d4889-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4889-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4889-105">Uma sugestão de reunião que inclui informações como o horário da reunião, a probabilidade de presença, a disponibilidade individual e os locais de reunião disponíveis.</span><span class="sxs-lookup"><span data-stu-id="d4889-105">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4889-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4889-106">JSON representation</span></span>

<span data-ttu-id="d4889-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d4889-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 100.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="d4889-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4889-108">Properties</span></span>
| <span data-ttu-id="d4889-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4889-109">Property</span></span>     | <span data-ttu-id="d4889-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4889-110">Type</span></span>   |<span data-ttu-id="d4889-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4889-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4889-112">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="d4889-112">attendeeAvailability</span></span>|<span data-ttu-id="d4889-113">Coleção [attendeeAvailability](attendeeavailability.md)</span><span class="sxs-lookup"><span data-stu-id="d4889-113">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="d4889-114">Uma matriz que mostra o status de disponibilidade de cada participante para essa sugestão da reunião.</span><span class="sxs-lookup"><span data-stu-id="d4889-114">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="d4889-115">confidence</span><span class="sxs-lookup"><span data-stu-id="d4889-115">confidence</span></span>|<span data-ttu-id="d4889-116">Double</span><span class="sxs-lookup"><span data-stu-id="d4889-116">Double</span></span>|<span data-ttu-id="d4889-117">Uma porcentagem que representa a probabilidade de todos os participantes comparecerem.</span><span class="sxs-lookup"><span data-stu-id="d4889-117">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="d4889-118">locations</span><span class="sxs-lookup"><span data-stu-id="d4889-118">locations</span></span>|<span data-ttu-id="d4889-119">Coleção [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="d4889-119">[location](location.md) collection</span></span>|<span data-ttu-id="d4889-120">Uma matriz que especifica o nome e a localização geográfica de cada local da reunião para esta sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="d4889-120">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="d4889-121">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="d4889-121">meetingTimeSlot</span></span>|[<span data-ttu-id="d4889-122">timeSlot</span><span class="sxs-lookup"><span data-stu-id="d4889-122">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="d4889-123">Um período de tempo sugerido para a reunião.</span><span class="sxs-lookup"><span data-stu-id="d4889-123">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="d4889-124">order</span><span class="sxs-lookup"><span data-stu-id="d4889-124">order</span></span>|<span data-ttu-id="d4889-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d4889-125">Int32</span></span>|<span data-ttu-id="d4889-126">Sugestões de hora de reunião, ordenadas por seu valor de confiança calculado de alto para baixo, em seguida, por cronologia, se houver sugestões com a mesma confiança.</span><span class="sxs-lookup"><span data-stu-id="d4889-126">Order of meeting time suggestions sorted by their computed confidence value from high to low, then by chronology if there are suggestions with the same confidence.</span></span> |
|<span data-ttu-id="d4889-127">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="d4889-127">organizerAvailability</span></span>|<span data-ttu-id="d4889-128">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="d4889-128">freeBusyStatus</span></span>| <span data-ttu-id="d4889-129">Disponibilidade do organizador da reunião para essa sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="d4889-129">Availability of the meeting organizer for this meeting suggestion.</span></span> <span data-ttu-id="d4889-130">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d4889-130">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="d4889-131">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="d4889-131">suggestionReason</span></span>|<span data-ttu-id="d4889-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4889-132">String</span></span>|<span data-ttu-id="d4889-133">Razão da sugestão de horário da reunião.</span><span class="sxs-lookup"><span data-stu-id="d4889-133">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

