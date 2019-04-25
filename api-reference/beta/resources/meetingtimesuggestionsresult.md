---
title: Tipo de recurso meetingTimeSuggestionsResult
description: Uma coleção de sugestões de reunião, se houver alguma, e a razão se não houver.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 654e53c5a3a329774e1b78065bb8cbcd41d6721f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581550"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="5e0c7-103">Tipo de recurso meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="5e0c7-103">meetingTimeSuggestionsResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e0c7-104">Uma coleção de sugestões de reunião, se houver alguma, e a razão se não houver.</span><span class="sxs-lookup"><span data-stu-id="5e0c7-104">A collection of meeting suggestions if there is any, and the reason if there isn't.</span></span>

<span data-ttu-id="5e0c7-105">A seguir estão os possíveis motivos que [findMeetingTimes](../api/user-findmeetingtimes.md) não retorna as sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="5e0c7-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="5e0c7-106">**valor de emptySuggestionsReason**</span><span class="sxs-lookup"><span data-stu-id="5e0c7-106">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="5e0c7-107">**Motivos**</span><span class="sxs-lookup"><span data-stu-id="5e0c7-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="5e0c7-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="5e0c7-108">attendeesUnavailable</span></span> | <span data-ttu-id="5e0c7-109">A disponibilidade de todos os participantes é conhecida, mas não há participantes suficientes disponíveis para alcançar o limite de [confiança da reunião](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) , que é de 50% por padrão, para qualquer período de tempo.</span><span class="sxs-lookup"><span data-stu-id="5e0c7-109">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="5e0c7-110">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="5e0c7-110">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="5e0c7-p101">Alguns ou todos os participantes têm disponibilidade desconhecida, fazendo com que a confiança na reunião caia para abaixo o limite definido, que é de 50% por padrão. A disponibilidade do participante poderá se tornar desconhecida se ele não for da organização ou se houver um erro ao obter informações sobre a disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="5e0c7-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="5e0c7-113">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="5e0c7-113">locationsUnavailable</span></span> | <span data-ttu-id="5e0c7-114">A \*\*\*\* propriedade IsRequired do parâmetro **locationConstraint** é especificada como true e, ainda, não há locais disponíveis nos intervalos de tempo calculados.</span><span class="sxs-lookup"><span data-stu-id="5e0c7-114">The **isRequired** property of the **locationConstraint** parameter is specified as true, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="5e0c7-115">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="5e0c7-115">organizerUnavailable</span></span> | <span data-ttu-id="5e0c7-116">O parâmetro **isOrganizerOptional** é falso, e o organizador não está disponível durante a janela de tempo solicitada.</span><span class="sxs-lookup"><span data-stu-id="5e0c7-116">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="5e0c7-117">desconhecido</span><span class="sxs-lookup"><span data-stu-id="5e0c7-117">unknown</span></span> | <span data-ttu-id="5e0c7-118">O motivo para não retornar qualquer sugestão de reunião não é conhecido.</span><span class="sxs-lookup"><span data-stu-id="5e0c7-118">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e0c7-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e0c7-119">JSON representation</span></span>

<span data-ttu-id="5e0c7-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5e0c7-120">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="5e0c7-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e0c7-121">Properties</span></span>
| <span data-ttu-id="5e0c7-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e0c7-122">Property</span></span>     | <span data-ttu-id="5e0c7-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e0c7-123">Type</span></span>   |<span data-ttu-id="5e0c7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e0c7-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e0c7-125">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="5e0c7-125">emptySuggestionsReason</span></span>|<span data-ttu-id="5e0c7-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e0c7-126">String</span></span>|<span data-ttu-id="5e0c7-127">Um motivo para não retornar qualquer sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="5e0c7-127">A reason for not returning any meeting suggestions.</span></span> <span data-ttu-id="5e0c7-128">Os valores possíveis são: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` ou `unknown`.</span><span class="sxs-lookup"><span data-stu-id="5e0c7-128">Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span> <span data-ttu-id="5e0c7-129">Esta propriedade é uma cadeia de caracteres vazia se a propriedade **meetingTimeSuggestions** inclui qualquer sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="5e0c7-129">This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="5e0c7-130">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="5e0c7-130">meetingTimeSuggestions</span></span>|<span data-ttu-id="5e0c7-131">Coleção [meetingTimeSuggestion](meetingtimesuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="5e0c7-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="5e0c7-132">Uma matriz de sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="5e0c7-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimesuggestionsresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->