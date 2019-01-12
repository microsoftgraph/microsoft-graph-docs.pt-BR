---
title: Tipo de recurso meetingTimeSuggestion
description: 'Uma sugestão de reunião que inclui informações sobre como tempo de reunião, a probabilidade de presença, indivíduo '
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: 8472526709e563900ac5193b0065111f3ed620fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978806"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="4ada7-103">Tipo de recurso meetingTimeSuggestion</span><span class="sxs-lookup"><span data-stu-id="4ada7-103">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="4ada7-104">Uma sugestão de reunião que inclui informações como o horário da reunião, a probabilidade de presença, a disponibilidade individual e os locais de reunião disponíveis.</span><span class="sxs-lookup"><span data-stu-id="4ada7-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ada7-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ada7-105">JSON representation</span></span>

<span data-ttu-id="4ada7-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="4ada7-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="4ada7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ada7-107">Properties</span></span>
| <span data-ttu-id="4ada7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ada7-108">Property</span></span>     | <span data-ttu-id="4ada7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ada7-109">Type</span></span>   |<span data-ttu-id="4ada7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ada7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ada7-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="4ada7-111">attendeeAvailability</span></span>|<span data-ttu-id="4ada7-112">[attendeeAvailability](attendeeavailability.md) collection</span><span class="sxs-lookup"><span data-stu-id="4ada7-112">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="4ada7-113">Uma matriz que mostra o status de disponibilidade de cada participante para essa sugestão da reunião.</span><span class="sxs-lookup"><span data-stu-id="4ada7-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="4ada7-114">confidence</span><span class="sxs-lookup"><span data-stu-id="4ada7-114">confidence</span></span>|<span data-ttu-id="4ada7-115">Double</span><span class="sxs-lookup"><span data-stu-id="4ada7-115">Double</span></span>|<span data-ttu-id="4ada7-116">Uma porcentagem que representa a probabilidade de todos os participantes comparecerem.</span><span class="sxs-lookup"><span data-stu-id="4ada7-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="4ada7-117">locations</span><span class="sxs-lookup"><span data-stu-id="4ada7-117">locations</span></span>|<span data-ttu-id="4ada7-118">Coleção [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="4ada7-118">[location](location.md) collection</span></span>|<span data-ttu-id="4ada7-119">Uma matriz que especifica o nome e a localização geográfica de cada local da reunião para esta sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="4ada7-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="4ada7-120">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="4ada7-120">meetingTimeSlot</span></span>|[<span data-ttu-id="4ada7-121">timeSlot</span><span class="sxs-lookup"><span data-stu-id="4ada7-121">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="4ada7-122">Um período de tempo sugerido para a reunião.</span><span class="sxs-lookup"><span data-stu-id="4ada7-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="4ada7-123">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="4ada7-123">organizerAvailability</span></span>|<span data-ttu-id="4ada7-124">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="4ada7-124">freeBusyStatus</span></span>| <span data-ttu-id="4ada7-125">Disponibilidade do organizador da reunião para essa sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="4ada7-125">Availability of the meeting organizer for this meeting suggestion.</span></span> <span data-ttu-id="4ada7-126">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4ada7-126">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="4ada7-127">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="4ada7-127">suggestionReason</span></span>|<span data-ttu-id="4ada7-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ada7-128">String</span></span>|<span data-ttu-id="4ada7-129">Razão da sugestão de horário da reunião.</span><span class="sxs-lookup"><span data-stu-id="4ada7-129">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
