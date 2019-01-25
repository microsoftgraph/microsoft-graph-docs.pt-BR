---
title: tipo de recurso de meetingTimeCandidate
description: 'Uma sugestão de reunião que inclui informações sobre como tempo de reunião, a probabilidade de presença, indivíduo '
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: 7da1240bc5bce285b041ef55ce372ba137b9d74a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523691"
---
# <a name="meetingtimecandidate-resource-type"></a><span data-ttu-id="98ec4-103">tipo de recurso de meetingTimeCandidate</span><span class="sxs-lookup"><span data-stu-id="98ec4-103">meetingTimeCandidate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98ec4-104">Uma sugestão de reunião que inclui informações como o horário da reunião, a probabilidade de presença, a disponibilidade individual e os locais de reunião disponíveis.</span><span class="sxs-lookup"><span data-stu-id="98ec4-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="98ec4-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="98ec4-105">JSON representation</span></span>

<span data-ttu-id="98ec4-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="98ec4-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeCandidate"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 1024.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "organizerAvailability": "String",
  "suggestionHint": "String"
}

```
## <a name="properties"></a><span data-ttu-id="98ec4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="98ec4-107">Properties</span></span>
| <span data-ttu-id="98ec4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98ec4-108">Property</span></span>     | <span data-ttu-id="98ec4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="98ec4-109">Type</span></span>   |<span data-ttu-id="98ec4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="98ec4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98ec4-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="98ec4-111">attendeeAvailability</span></span>|<span data-ttu-id="98ec4-112">[attendeeAvailability](attendeeavailability.md) collection</span><span class="sxs-lookup"><span data-stu-id="98ec4-112">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="98ec4-113">Uma matriz que mostra o status de disponibilidade de cada participante para essa sugestão da reunião.</span><span class="sxs-lookup"><span data-stu-id="98ec4-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="98ec4-114">confidence</span><span class="sxs-lookup"><span data-stu-id="98ec4-114">confidence</span></span>|<span data-ttu-id="98ec4-115">Double</span><span class="sxs-lookup"><span data-stu-id="98ec4-115">Double</span></span>|<span data-ttu-id="98ec4-116">Uma porcentagem que representa a probabilidade de todos os participantes comparecerem.</span><span class="sxs-lookup"><span data-stu-id="98ec4-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="98ec4-117">locations</span><span class="sxs-lookup"><span data-stu-id="98ec4-117">locations</span></span>|<span data-ttu-id="98ec4-118">Coleção [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="98ec4-118">[location](location.md) collection</span></span>|<span data-ttu-id="98ec4-119">Uma matriz que especifica o nome e a localização geográfica de cada local da reunião para esta sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="98ec4-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="98ec4-120">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="98ec4-120">meetingTimeSlot</span></span>|[<span data-ttu-id="98ec4-121">timeSlot</span><span class="sxs-lookup"><span data-stu-id="98ec4-121">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="98ec4-122">Um período de tempo sugerido para a reunião.</span><span class="sxs-lookup"><span data-stu-id="98ec4-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="98ec4-123">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="98ec4-123">organizerAvailability</span></span>|<span data-ttu-id="98ec4-124">String</span><span class="sxs-lookup"><span data-stu-id="98ec4-124">String</span></span>| <span data-ttu-id="98ec4-p101">Disponibilidade do organizador da reunião para essa sugestão de reunião. Os possíveis valores são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="98ec4-p101">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="98ec4-127">suggestionHint</span><span class="sxs-lookup"><span data-stu-id="98ec4-127">suggestionHint</span></span>|<span data-ttu-id="98ec4-128">String</span><span class="sxs-lookup"><span data-stu-id="98ec4-128">String</span></span>|<span data-ttu-id="98ec4-129">Razão da sugestão de horário da reunião.</span><span class="sxs-lookup"><span data-stu-id="98ec4-129">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeCandidate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimecandidate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
