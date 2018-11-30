---
title: Tipo de recurso meetingTimeSuggestion
description: 'Uma sugestão de reunião que inclui informações sobre como tempo de reunião, a probabilidade de presença, indivíduo '
ms.openlocfilehash: 345d09015be5e489c88cb89fe6a4175ebbab2874
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007116"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="41376-103">Tipo de recurso meetingTimeSuggestion</span><span class="sxs-lookup"><span data-stu-id="41376-103">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="41376-104">Uma sugestão de reunião que inclui informações como o horário da reunião, a probabilidade de presença, a disponibilidade individual e os locais de reunião disponíveis.</span><span class="sxs-lookup"><span data-stu-id="41376-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="41376-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41376-105">JSON representation</span></span>

<span data-ttu-id="41376-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="41376-106">Here is a JSON representation of the resource</span></span>

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
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="41376-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41376-107">Properties</span></span>
| <span data-ttu-id="41376-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41376-108">Property</span></span>     | <span data-ttu-id="41376-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="41376-109">Type</span></span>   |<span data-ttu-id="41376-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="41376-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41376-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="41376-111">attendeeAvailability</span></span>|<span data-ttu-id="41376-112">[attendeeAvailability](attendeeavailability.md) collection</span><span class="sxs-lookup"><span data-stu-id="41376-112">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="41376-113">Uma matriz que mostra o status de disponibilidade de cada participante para essa sugestão da reunião.</span><span class="sxs-lookup"><span data-stu-id="41376-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="41376-114">confidence</span><span class="sxs-lookup"><span data-stu-id="41376-114">confidence</span></span>|<span data-ttu-id="41376-115">Double</span><span class="sxs-lookup"><span data-stu-id="41376-115">Double</span></span>|<span data-ttu-id="41376-116">Uma porcentagem que representa a probabilidade de todos os participantes comparecerem.</span><span class="sxs-lookup"><span data-stu-id="41376-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="41376-117">locations</span><span class="sxs-lookup"><span data-stu-id="41376-117">locations</span></span>|<span data-ttu-id="41376-118">Coleção [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="41376-118">[location](location.md) collection</span></span>|<span data-ttu-id="41376-119">Uma matriz que especifica o nome e a localização geográfica de cada local da reunião para esta sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="41376-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="41376-120">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="41376-120">meetingTimeSlot</span></span>|[<span data-ttu-id="41376-121">timeSlot</span><span class="sxs-lookup"><span data-stu-id="41376-121">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="41376-122">Um período de tempo sugerido para a reunião.</span><span class="sxs-lookup"><span data-stu-id="41376-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="41376-123">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="41376-123">organizerAvailability</span></span>|<span data-ttu-id="41376-124">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="41376-124">freeBusyStatus</span></span>| <span data-ttu-id="41376-125">Disponibilidade do organizador da reunião para essa sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="41376-125">Availability of the meeting organizer for this meeting suggestion.</span></span> <span data-ttu-id="41376-126">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="41376-126">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="41376-127">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="41376-127">suggestionReason</span></span>|<span data-ttu-id="41376-128">String</span><span class="sxs-lookup"><span data-stu-id="41376-128">String</span></span>|<span data-ttu-id="41376-129">Razão da sugestão de horário da reunião.</span><span class="sxs-lookup"><span data-stu-id="41376-129">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->