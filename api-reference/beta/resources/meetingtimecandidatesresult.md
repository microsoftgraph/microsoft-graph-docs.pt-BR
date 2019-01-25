---
title: tipo de recurso de meetingTimeCandidatesResult
description: Uma coleção de sugestões de reunião, se houver alguma, ou se não houver motivo.
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: e60c0092ca5724e4019a4c3f75f1239a0e7e9c0b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507513"
---
# <a name="meetingtimecandidatesresult-resource-type"></a><span data-ttu-id="68539-103">tipo de recurso de meetingTimeCandidatesResult</span><span class="sxs-lookup"><span data-stu-id="68539-103">meetingTimeCandidatesResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68539-104">Uma coleção de sugestões de reunião, se houver alguma, ou se não houver motivo.</span><span class="sxs-lookup"><span data-stu-id="68539-104">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="68539-105">A seguir estão os possíveis motivos que [findMeetingTimes](../api/user-findmeetingtimes.md) não retorna as sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="68539-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="68539-106">**valor de emptySuggestionsHint**</span><span class="sxs-lookup"><span data-stu-id="68539-106">**emptySuggestionsHint value**</span></span>|<span data-ttu-id="68539-107">**Motivos**</span><span class="sxs-lookup"><span data-stu-id="68539-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="68539-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="68539-108">attendeesUnavailable</span></span> | <span data-ttu-id="68539-109">A disponibilidade de todos os participantes é conhecida, mas não há participantes suficientes disponíveis para alcançar o limite de confiança da reunião, que é de 50% por padrão, para qualquer período de tempo.</span><span class="sxs-lookup"><span data-stu-id="68539-109">All of the attendees' availability is known, but not enough attendees are available to reach the meeting confidence threshold, which is 50% by default, for any time period.</span></span> <span data-ttu-id="68539-110">Esse limite é baseado no status dos participantes livre/ocupado para uma reunião sugerida período de tempo, com o status livre de um participante correspondente a chance de 100% de presença, o status desconhecido 50% e o status ocupado 0%.</span><span class="sxs-lookup"><span data-stu-id="68539-110">This threshold is based on the attendees' free/busy status for a suggested meeting time period, with an attendee's free status corresponding to 100% chance of attendance, unknown status 50%, and busy status 0%.</span></span>|
| <span data-ttu-id="68539-111">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="68539-111">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="68539-p102">Alguns ou todos os participantes têm disponibilidade desconhecida, fazendo com que a confiança na reunião caia para abaixo o limite definido, que é de 50% por padrão. A disponibilidade do participante poderá se tornar desconhecida se ele não for da organização ou se houver um erro ao obter informações sobre a disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="68539-p102">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="68539-114">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="68539-114">locationsUnavailable</span></span> | <span data-ttu-id="68539-115">A propriedade **isRequired** do parâmetro [locationConstraint](locationconstraint.md) é especificada como obrigatória, e ainda não existem locais disponíveis nos intervalos de tempo calculados.</span><span class="sxs-lookup"><span data-stu-id="68539-115">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="68539-116">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="68539-116">organizerUnavailable</span></span> | <span data-ttu-id="68539-117">O parâmetro **isOrganizerOptional** é falso, e o organizador não está disponível durante a janela de tempo solicitada.</span><span class="sxs-lookup"><span data-stu-id="68539-117">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="68539-118">unknown</span><span class="sxs-lookup"><span data-stu-id="68539-118">unknown</span></span> | <span data-ttu-id="68539-119">O motivo para não retornar qualquer sugestão de reunião não é conhecido.</span><span class="sxs-lookup"><span data-stu-id="68539-119">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68539-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68539-120">JSON representation</span></span>

<span data-ttu-id="68539-121">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="68539-121">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeCandidatesResult"
}-->

```json
{
  "emptySuggestionsHint": "String",
  "meetingTimeSlots": [{"@odata.type": "microsoft.graph.meetingTimeCandidate"}]
}

```
## <a name="properties"></a><span data-ttu-id="68539-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68539-122">Properties</span></span>
| <span data-ttu-id="68539-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68539-123">Property</span></span>     | <span data-ttu-id="68539-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="68539-124">Type</span></span>   |<span data-ttu-id="68539-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="68539-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68539-126">emptySuggestionsHint</span><span class="sxs-lookup"><span data-stu-id="68539-126">emptySuggestionsHint</span></span>|<span data-ttu-id="68539-127">String</span><span class="sxs-lookup"><span data-stu-id="68539-127">String</span></span>|<span data-ttu-id="68539-p103">Um motivo para não retornar qualquer sugestão de reunião. Os valores possíveis são: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` ou `unknown`.</span><span class="sxs-lookup"><span data-stu-id="68539-p103">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span>|
|<span data-ttu-id="68539-130">meetingTimeSlots</span><span class="sxs-lookup"><span data-stu-id="68539-130">meetingTimeSlots</span></span>|<span data-ttu-id="68539-131">coleção [meetingTimeCandidate](meetingtimecandidate.md)</span><span class="sxs-lookup"><span data-stu-id="68539-131">[meetingTimeCandidate](meetingtimecandidate.md) collection</span></span>|<span data-ttu-id="68539-132">Uma matriz de sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="68539-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeCandidatesResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimecandidatesresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
