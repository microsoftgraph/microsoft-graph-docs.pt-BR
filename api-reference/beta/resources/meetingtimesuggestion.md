---
title: Tipo de recurso meetingTimeSuggestion
description: 'Uma sugestão de reunião que inclui informações sobre como tempo de reunião, a probabilidade de presença, indivíduo '
ms.openlocfilehash: 04b7996292decab5330cb17b8aada82d58cf759f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040721"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="ea265-103">Tipo de recurso meetingTimeSuggestion</span><span class="sxs-lookup"><span data-stu-id="ea265-103">meetingTimeSuggestion resource type</span></span>

> <span data-ttu-id="ea265-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ea265-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea265-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ea265-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ea265-106">Uma sugestão de reunião que inclui informações como o horário da reunião, a probabilidade de presença, a disponibilidade individual e os locais de reunião disponíveis.</span><span class="sxs-lookup"><span data-stu-id="ea265-106">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea265-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea265-107">JSON representation</span></span>

<span data-ttu-id="ea265-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ea265-108">Here is a JSON representation of the resource</span></span>

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
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="ea265-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea265-109">Properties</span></span>
| <span data-ttu-id="ea265-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea265-110">Property</span></span>     | <span data-ttu-id="ea265-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea265-111">Type</span></span>   |<span data-ttu-id="ea265-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea265-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea265-113">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="ea265-113">attendeeAvailability</span></span>|<span data-ttu-id="ea265-114">[attendeeAvailability](attendeeavailability.md) collection</span><span class="sxs-lookup"><span data-stu-id="ea265-114">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="ea265-115">Uma matriz que mostra o status de disponibilidade de cada participante para essa sugestão da reunião.</span><span class="sxs-lookup"><span data-stu-id="ea265-115">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="ea265-116">confidence</span><span class="sxs-lookup"><span data-stu-id="ea265-116">confidence</span></span>|<span data-ttu-id="ea265-117">Double</span><span class="sxs-lookup"><span data-stu-id="ea265-117">Double</span></span>|<span data-ttu-id="ea265-118">Uma porcentagem que representa a probabilidade de todos os participantes comparecerem.</span><span class="sxs-lookup"><span data-stu-id="ea265-118">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="ea265-119">locations</span><span class="sxs-lookup"><span data-stu-id="ea265-119">locations</span></span>|<span data-ttu-id="ea265-120">Coleção [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="ea265-120">[location](location.md) collection</span></span>|<span data-ttu-id="ea265-121">Uma matriz que especifica o nome e a localização geográfica de cada local da reunião para esta sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="ea265-121">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="ea265-122">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="ea265-122">meetingTimeSlot</span></span>|[<span data-ttu-id="ea265-123">timeSlot</span><span class="sxs-lookup"><span data-stu-id="ea265-123">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="ea265-124">Um período de tempo sugerido para a reunião.</span><span class="sxs-lookup"><span data-stu-id="ea265-124">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="ea265-125">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="ea265-125">organizerAvailability</span></span>|<span data-ttu-id="ea265-126">String</span><span class="sxs-lookup"><span data-stu-id="ea265-126">String</span></span>| <span data-ttu-id="ea265-p102">Disponibilidade do organizador da reunião para essa sugestão de reunião. Os possíveis valores são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ea265-p102">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="ea265-129">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="ea265-129">suggestionReason</span></span>|<span data-ttu-id="ea265-130">String</span><span class="sxs-lookup"><span data-stu-id="ea265-130">String</span></span>|<span data-ttu-id="ea265-131">Razão da sugestão de horário da reunião.</span><span class="sxs-lookup"><span data-stu-id="ea265-131">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->