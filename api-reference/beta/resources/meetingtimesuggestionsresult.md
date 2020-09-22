---
title: Tipo de recurso meetingTimeSuggestionsResult
description: Uma coleção de sugestões de reunião, se houver alguma, e a razão se não houver.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e12bcb2e75a85b33f0968d13b9f9a38dbc026cfe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971612"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="c9449-103">Tipo de recurso meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="c9449-103">meetingTimeSuggestionsResult resource type</span></span>

<span data-ttu-id="c9449-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9449-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9449-105">Uma coleção de sugestões de reunião, se houver alguma, e a razão se não houver.</span><span class="sxs-lookup"><span data-stu-id="c9449-105">A collection of meeting suggestions if there is any, and the reason if there isn't.</span></span>

<span data-ttu-id="c9449-106">A seguir estão os possíveis motivos que [findMeetingTimes](../api/user-findmeetingtimes.md) não retorna as sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="c9449-106">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="c9449-107">**valor de emptySuggestionsReason**</span><span class="sxs-lookup"><span data-stu-id="c9449-107">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="c9449-108">**Motivos**</span><span class="sxs-lookup"><span data-stu-id="c9449-108">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="c9449-109">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="c9449-109">attendeesUnavailable</span></span> | <span data-ttu-id="c9449-110">A disponibilidade de todos os participantes é conhecida, mas não há participantes suficientes disponíveis para alcançar o limite de [confiança da reunião](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) , que é de 50% por padrão, para qualquer período de tempo.</span><span class="sxs-lookup"><span data-stu-id="c9449-110">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="c9449-111">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="c9449-111">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="c9449-p101">Alguns ou todos os participantes têm disponibilidade desconhecida, fazendo com que a confiança na reunião caia para abaixo o limite definido, que é de 50% por padrão. A disponibilidade do participante poderá se tornar desconhecida se ele não for da organização ou se houver um erro ao obter informações sobre a disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="c9449-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="c9449-114">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="c9449-114">locationsUnavailable</span></span> | <span data-ttu-id="c9449-115">A propriedade **IsRequired** do parâmetro **locationConstraint** é especificada como true e, ainda, não há locais disponíveis nos intervalos de tempo calculados.</span><span class="sxs-lookup"><span data-stu-id="c9449-115">The **isRequired** property of the **locationConstraint** parameter is specified as true, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="c9449-116">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="c9449-116">organizerUnavailable</span></span> | <span data-ttu-id="c9449-117">O parâmetro **isOrganizerOptional** é falso, e o organizador não está disponível durante a janela de tempo solicitada.</span><span class="sxs-lookup"><span data-stu-id="c9449-117">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="c9449-118">desconhecido</span><span class="sxs-lookup"><span data-stu-id="c9449-118">unknown</span></span> | <span data-ttu-id="c9449-119">O motivo para não retornar qualquer sugestão de reunião não é conhecido.</span><span class="sxs-lookup"><span data-stu-id="c9449-119">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9449-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9449-120">JSON representation</span></span>

<span data-ttu-id="c9449-121">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c9449-121">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="c9449-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9449-122">Properties</span></span>
| <span data-ttu-id="c9449-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9449-123">Property</span></span>     | <span data-ttu-id="c9449-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9449-124">Type</span></span>   |<span data-ttu-id="c9449-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9449-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9449-126">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="c9449-126">emptySuggestionsReason</span></span>|<span data-ttu-id="c9449-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9449-127">String</span></span>|<span data-ttu-id="c9449-128">Um motivo para não retornar qualquer sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="c9449-128">A reason for not returning any meeting suggestions.</span></span> <span data-ttu-id="c9449-129">Os valores possíveis são: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` ou `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c9449-129">Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span> <span data-ttu-id="c9449-130">Esta propriedade é uma cadeia de caracteres vazia se a propriedade **meetingTimeSuggestions** inclui qualquer sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="c9449-130">This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="c9449-131">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="c9449-131">meetingTimeSuggestions</span></span>|<span data-ttu-id="c9449-132">Coleção [meetingTimeSuggestion](meetingtimesuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="c9449-132">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="c9449-133">Uma matriz de sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="c9449-133">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


