---
title: Tipo de recurso meetingTimeSuggestionsResult
description: Uma coleção de sugestões de reunião, se houver alguma, ou se não houver motivo.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1b30f2ad3d6ebe84ad733b7136cd14f30fef1ea9
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472633"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="bca5f-103">Tipo de recurso meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="bca5f-103">meetingTimeSuggestionsResult resource type</span></span>

<span data-ttu-id="bca5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bca5f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bca5f-105">Uma coleção de sugestões de reunião, se houver alguma, ou se não houver motivo.</span><span class="sxs-lookup"><span data-stu-id="bca5f-105">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="bca5f-106">A seguir estão os possíveis motivos que [findMeetingTimes](../api/user-findmeetingtimes.md) não retorna as sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="bca5f-106">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="bca5f-107">**valor de emptySuggestionsReason**</span><span class="sxs-lookup"><span data-stu-id="bca5f-107">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="bca5f-108">**Motivos**</span><span class="sxs-lookup"><span data-stu-id="bca5f-108">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="bca5f-109">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="bca5f-109">attendeesUnavailable</span></span> | <span data-ttu-id="bca5f-110">Toda a disponibilidade dos participantes é conhecida, mas não há participantes [](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) suficientes disponíveis para alcançar o limite de confiança da reunião, que é de 50% por padrão, para qualquer período de tempo.</span><span class="sxs-lookup"><span data-stu-id="bca5f-110">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="bca5f-111">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="bca5f-111">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="bca5f-p101">Alguns ou todos os participantes têm disponibilidade desconhecida, fazendo com que a confiança na reunião caia para abaixo o limite definido, que é de 50% por padrão. A disponibilidade do participante poderá se tornar desconhecida se ele não for da organização ou se houver um erro ao obter informações sobre a disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="bca5f-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="bca5f-114">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="bca5f-114">locationsUnavailable</span></span> | <span data-ttu-id="bca5f-115">A propriedade **isRequired** do parâmetro [locationConstraint](locationconstraint.md) é especificada como obrigatória, e ainda não existem locais disponíveis nos intervalos de tempo calculados.</span><span class="sxs-lookup"><span data-stu-id="bca5f-115">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="bca5f-116">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="bca5f-116">organizerUnavailable</span></span> | <span data-ttu-id="bca5f-117">O parâmetro **isOrganizerOptional** é falso, e o organizador não está disponível durante a janela de tempo solicitada.</span><span class="sxs-lookup"><span data-stu-id="bca5f-117">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="bca5f-118">desconhecido</span><span class="sxs-lookup"><span data-stu-id="bca5f-118">unknown</span></span> | <span data-ttu-id="bca5f-119">O motivo para não retornar qualquer sugestão de reunião não é conhecido.</span><span class="sxs-lookup"><span data-stu-id="bca5f-119">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bca5f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bca5f-120">JSON representation</span></span>

<span data-ttu-id="bca5f-121">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bca5f-121">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult"
}-->

```json
{
  "emptySuggestionsReason": "String",
  "meetingTimeSuggestions": [{"@odata.type": "microsoft.graph.meetingTimeSuggestion"}]
}

```
## <a name="properties"></a><span data-ttu-id="bca5f-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bca5f-122">Properties</span></span>
| <span data-ttu-id="bca5f-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bca5f-123">Property</span></span>     | <span data-ttu-id="bca5f-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="bca5f-124">Type</span></span>   |<span data-ttu-id="bca5f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="bca5f-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bca5f-126">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="bca5f-126">emptySuggestionsReason</span></span>|<span data-ttu-id="bca5f-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bca5f-127">String</span></span>|<span data-ttu-id="bca5f-128">Um motivo para não retornar qualquer sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="bca5f-128">A reason for not returning any meeting suggestions.</span></span> <span data-ttu-id="bca5f-129">Os valores possíveis são: `attendeesUnavailable` , , , , ou `attendeesUnavailableOrUnknown` `locationsUnavailable` `organizerUnavailable` `unknown` .</span><span class="sxs-lookup"><span data-stu-id="bca5f-129">The possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span> <span data-ttu-id="bca5f-130">Essa propriedade será uma cadeia de caracteres vazia se a **propriedade meetingTimeSuggestions** incluir sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="bca5f-130">This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="bca5f-131">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="bca5f-131">meetingTimeSuggestions</span></span>|<span data-ttu-id="bca5f-132">Coleção [meetingTimeSuggestion](meetingtimesuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="bca5f-132">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="bca5f-133">Uma matriz de sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="bca5f-133">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

