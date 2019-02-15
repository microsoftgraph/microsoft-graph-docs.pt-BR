---
title: Tipo de recurso meetingTimeSuggestion
description: 'Uma sugestão de reunião que inclui informações como o horário da reunião, a probabilidade de presença, individual '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 379bb4ac4be8e2d8d1bec494cf4d573550d46b55
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057026"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="4a0f9-103">Tipo de recurso meetingTimeSuggestion</span><span class="sxs-lookup"><span data-stu-id="4a0f9-103">meetingTimeSuggestion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a0f9-104">Uma sugestão de reunião que inclui informações como o horário da reunião, a probabilidade de presença, a disponibilidade individual e os locais de reunião disponíveis.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a0f9-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a0f9-105">JSON representation</span></span>

<span data-ttu-id="4a0f9-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="4a0f9-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailabilityDataModel"}],
  "confidence": 1024.0,
  "locations": [{"@odata.type": "microsoft.graph.locationDataModel"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.meetingTimeSlotDataModel"},
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="4a0f9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a0f9-107">Properties</span></span>
| <span data-ttu-id="4a0f9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a0f9-108">Property</span></span>     | <span data-ttu-id="4a0f9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a0f9-109">Type</span></span>   |<span data-ttu-id="4a0f9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a0f9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a0f9-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="4a0f9-111">attendeeAvailability</span></span>|<span data-ttu-id="4a0f9-112">coleção [attendeeAvailabilityDataModel](attendeeavailabilitydatamodel.md)</span><span class="sxs-lookup"><span data-stu-id="4a0f9-112">[attendeeAvailabilityDataModel](attendeeavailabilitydatamodel.md) collection</span></span>|<span data-ttu-id="4a0f9-113">Uma matriz que mostra o status de disponibilidade de cada participante para essa sugestão da reunião.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="4a0f9-114">confidence</span><span class="sxs-lookup"><span data-stu-id="4a0f9-114">confidence</span></span>|<span data-ttu-id="4a0f9-115">Double</span><span class="sxs-lookup"><span data-stu-id="4a0f9-115">Double</span></span>|<span data-ttu-id="4a0f9-116">Uma porcentagem que representa a probabilidade de todos os participantes comparecerem.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="4a0f9-117">locations</span><span class="sxs-lookup"><span data-stu-id="4a0f9-117">locations</span></span>|<span data-ttu-id="4a0f9-118">coleção [locationDataModel](locationdatamodel.md)</span><span class="sxs-lookup"><span data-stu-id="4a0f9-118">[locationDataModel](locationdatamodel.md) collection</span></span>|<span data-ttu-id="4a0f9-119">Uma matriz que especifica o nome e a localização geográfica de cada local da reunião para esta sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="4a0f9-120">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="4a0f9-120">meetingTimeSlot</span></span>|[<span data-ttu-id="4a0f9-121">meetingTimeSlotDataModel</span><span class="sxs-lookup"><span data-stu-id="4a0f9-121">meetingTimeSlotDataModel</span></span>](meetingtimeslotdatamodel.md)|<span data-ttu-id="4a0f9-122">Um período de tempo sugerido para a reunião.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="4a0f9-123">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="4a0f9-123">organizerAvailability</span></span>|<span data-ttu-id="4a0f9-124">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="4a0f9-124">availabilityStatus</span></span>| <span data-ttu-id="4a0f9-p101">Disponibilidade do organizador da reunião para essa sugestão de reunião. Os possíveis valores são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-p101">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="4a0f9-127">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="4a0f9-127">suggestionReason</span></span>|<span data-ttu-id="4a0f9-128">String</span><span class="sxs-lookup"><span data-stu-id="4a0f9-128">String</span></span>|<span data-ttu-id="4a0f9-129">Razão da sugestão de horário da reunião.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-129">Reason for suggesting the meeting time.</span></span>|

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
