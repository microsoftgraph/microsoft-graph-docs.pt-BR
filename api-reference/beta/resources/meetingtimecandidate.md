---
title: tipo de recurso de meetingTimeCandidate
description: 'Uma sugestão de reunião que inclui informações sobre como tempo de reunião, a probabilidade de presença, indivíduo '
localization_priority: Normal
ms.openlocfilehash: bbd237e9bfebac0b6d3f27b343ec1294d9e21881
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853029"
---
# <a name="meetingtimecandidate-resource-type"></a><span data-ttu-id="d2a35-103">tipo de recurso de meetingTimeCandidate</span><span class="sxs-lookup"><span data-stu-id="d2a35-103">meetingTimeCandidate resource type</span></span>

> <span data-ttu-id="d2a35-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d2a35-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2a35-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d2a35-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2a35-106">Uma sugestão de reunião que inclui informações como o horário da reunião, a probabilidade de presença, a disponibilidade individual e os locais de reunião disponíveis.</span><span class="sxs-lookup"><span data-stu-id="d2a35-106">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2a35-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2a35-107">JSON representation</span></span>

<span data-ttu-id="d2a35-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d2a35-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="d2a35-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2a35-109">Properties</span></span>
| <span data-ttu-id="d2a35-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2a35-110">Property</span></span>     | <span data-ttu-id="d2a35-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2a35-111">Type</span></span>   |<span data-ttu-id="d2a35-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2a35-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2a35-113">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="d2a35-113">attendeeAvailability</span></span>|<span data-ttu-id="d2a35-114">[attendeeAvailability](attendeeavailability.md) collection</span><span class="sxs-lookup"><span data-stu-id="d2a35-114">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="d2a35-115">Uma matriz que mostra o status de disponibilidade de cada participante para essa sugestão da reunião.</span><span class="sxs-lookup"><span data-stu-id="d2a35-115">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="d2a35-116">confidence</span><span class="sxs-lookup"><span data-stu-id="d2a35-116">confidence</span></span>|<span data-ttu-id="d2a35-117">Double</span><span class="sxs-lookup"><span data-stu-id="d2a35-117">Double</span></span>|<span data-ttu-id="d2a35-118">Uma porcentagem que representa a probabilidade de todos os participantes comparecerem.</span><span class="sxs-lookup"><span data-stu-id="d2a35-118">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="d2a35-119">locations</span><span class="sxs-lookup"><span data-stu-id="d2a35-119">locations</span></span>|<span data-ttu-id="d2a35-120">Coleção [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="d2a35-120">[location](location.md) collection</span></span>|<span data-ttu-id="d2a35-121">Uma matriz que especifica o nome e a localização geográfica de cada local da reunião para esta sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="d2a35-121">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="d2a35-122">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="d2a35-122">meetingTimeSlot</span></span>|[<span data-ttu-id="d2a35-123">timeSlot</span><span class="sxs-lookup"><span data-stu-id="d2a35-123">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="d2a35-124">Um período de tempo sugerido para a reunião.</span><span class="sxs-lookup"><span data-stu-id="d2a35-124">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="d2a35-125">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="d2a35-125">organizerAvailability</span></span>|<span data-ttu-id="d2a35-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2a35-126">String</span></span>| <span data-ttu-id="d2a35-p102">Disponibilidade do organizador da reunião para essa sugestão de reunião. Os possíveis valores são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d2a35-p102">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="d2a35-129">suggestionHint</span><span class="sxs-lookup"><span data-stu-id="d2a35-129">suggestionHint</span></span>|<span data-ttu-id="d2a35-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2a35-130">String</span></span>|<span data-ttu-id="d2a35-131">Razão da sugestão de horário da reunião.</span><span class="sxs-lookup"><span data-stu-id="d2a35-131">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeCandidate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
