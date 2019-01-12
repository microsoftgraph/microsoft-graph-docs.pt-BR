---
title: Tipo de recurso meetingTimeSuggestionsResult
description: Uma coleção de sugestões de reunião, se houver alguma, ou se não houver motivo.
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: ed3af37ba48a48f3bc864dc8d9ad67e729999398
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914182"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="c10a0-103">Tipo de recurso meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="c10a0-103">meetingTimeSuggestionsResult resource type</span></span>

<span data-ttu-id="c10a0-104">Uma coleção de sugestões de reunião, se houver alguma, ou se não houver motivo.</span><span class="sxs-lookup"><span data-stu-id="c10a0-104">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="c10a0-105">A seguir estão os possíveis motivos que [findMeetingTimes](../api/user-findmeetingtimes.md) não retorna as sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="c10a0-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="c10a0-106">**valor de emptySuggestionsReason**</span><span class="sxs-lookup"><span data-stu-id="c10a0-106">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="c10a0-107">**Motivos**</span><span class="sxs-lookup"><span data-stu-id="c10a0-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="c10a0-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="c10a0-108">attendeesUnavailable</span></span> | <span data-ttu-id="c10a0-109">A disponibilidade de todos os participantes é conhecida, mas não há participantes suficientes disponíveis para alcançar o limite de [confiança da reunião](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion), que é de 50% por padrão, para qualquer período de tempo.</span><span class="sxs-lookup"><span data-stu-id="c10a0-109">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="c10a0-110">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="c10a0-110">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="c10a0-p101">Alguns ou todos os participantes têm disponibilidade desconhecida, fazendo com que a confiança na reunião caia para abaixo o limite definido, que é de 50% por padrão. A disponibilidade do participante poderá se tornar desconhecida se ele não for da organização ou se houver um erro ao obter informações sobre a disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="c10a0-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="c10a0-113">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="c10a0-113">locationsUnavailable</span></span> | <span data-ttu-id="c10a0-114">A propriedade **isRequired** do parâmetro [locationConstraint](locationconstraint.md) é especificada como obrigatória, e ainda não existem locais disponíveis nos intervalos de tempo calculados.</span><span class="sxs-lookup"><span data-stu-id="c10a0-114">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="c10a0-115">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="c10a0-115">organizerUnavailable</span></span> | <span data-ttu-id="c10a0-116">O parâmetro **isOrganizerOptional** é falso, e o organizador não está disponível durante a janela de tempo solicitada.</span><span class="sxs-lookup"><span data-stu-id="c10a0-116">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="c10a0-117">unknown</span><span class="sxs-lookup"><span data-stu-id="c10a0-117">unknown</span></span> | <span data-ttu-id="c10a0-118">O motivo para não retornar qualquer sugestão de reunião não é conhecido.</span><span class="sxs-lookup"><span data-stu-id="c10a0-118">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c10a0-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c10a0-119">JSON representation</span></span>

<span data-ttu-id="c10a0-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c10a0-120">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="c10a0-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c10a0-121">Properties</span></span>
| <span data-ttu-id="c10a0-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c10a0-122">Property</span></span>     | <span data-ttu-id="c10a0-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c10a0-123">Type</span></span>   |<span data-ttu-id="c10a0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c10a0-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c10a0-125">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="c10a0-125">emptySuggestionsReason</span></span>|<span data-ttu-id="c10a0-126">String</span><span class="sxs-lookup"><span data-stu-id="c10a0-126">String</span></span>|<span data-ttu-id="c10a0-127">Um motivo para não retornando alguma sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="c10a0-127">A reason for not returning any meeting suggestions.</span></span> <span data-ttu-id="c10a0-128">Os valores possíveis são: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, ou `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c10a0-128">The possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span> <span data-ttu-id="c10a0-129">Essa propriedade será uma sequência vazia se a propriedade **meetingTimeSuggestions** incluir quaisquer sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="c10a0-129">This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="c10a0-130">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="c10a0-130">meetingTimeSuggestions</span></span>|<span data-ttu-id="c10a0-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span><span class="sxs-lookup"><span data-stu-id="c10a0-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="c10a0-132">Uma matriz de sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="c10a0-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
