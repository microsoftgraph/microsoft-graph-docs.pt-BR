---
title: tipo de recurso de meetingTimeCandidatesResult
description: Uma coleção de sugestões de reunião, se houver alguma, ou se não houver motivo.
localization_priority: Normal
ms.openlocfilehash: 5b261295de43dcb0bfb94f85c833559430365002
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810651"
---
# <a name="meetingtimecandidatesresult-resource-type"></a><span data-ttu-id="276cd-103">tipo de recurso de meetingTimeCandidatesResult</span><span class="sxs-lookup"><span data-stu-id="276cd-103">meetingTimeCandidatesResult resource type</span></span>

> <span data-ttu-id="276cd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="276cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="276cd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="276cd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="276cd-106">Uma coleção de sugestões de reunião, se houver alguma, ou se não houver motivo.</span><span class="sxs-lookup"><span data-stu-id="276cd-106">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="276cd-107">A seguir estão os possíveis motivos que [findMeetingTimes](../api/user-findmeetingtimes.md) não retorna as sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="276cd-107">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="276cd-108">**valor de emptySuggestionsHint**</span><span class="sxs-lookup"><span data-stu-id="276cd-108">**emptySuggestionsHint value**</span></span>|<span data-ttu-id="276cd-109">**Motivos**</span><span class="sxs-lookup"><span data-stu-id="276cd-109">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="276cd-110">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="276cd-110">attendeesUnavailable</span></span> | <span data-ttu-id="276cd-111">A disponibilidade de todos os participantes é conhecida, mas não há participantes suficientes disponíveis para alcançar o limite de confiança da reunião, que é de 50% por padrão, para qualquer período de tempo.</span><span class="sxs-lookup"><span data-stu-id="276cd-111">All of the attendees' availability is known, but not enough attendees are available to reach the meeting confidence threshold, which is 50% by default, for any time period.</span></span> <span data-ttu-id="276cd-112">Esse limite é baseado no status dos participantes livre/ocupado para uma reunião sugerida período de tempo, com o status livre de um participante correspondente a chance de 100% de presença, o status desconhecido 50% e o status ocupado 0%.</span><span class="sxs-lookup"><span data-stu-id="276cd-112">This threshold is based on the attendees' free/busy status for a suggested meeting time period, with an attendee's free status corresponding to 100% chance of attendance, unknown status 50%, and busy status 0%.</span></span>|
| <span data-ttu-id="276cd-113">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="276cd-113">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="276cd-p103">Alguns ou todos os participantes têm disponibilidade desconhecida, fazendo com que a confiança na reunião caia para abaixo o limite definido, que é de 50% por padrão. A disponibilidade do participante poderá se tornar desconhecida se ele não for da organização ou se houver um erro ao obter informações sobre a disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="276cd-p103">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="276cd-116">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="276cd-116">locationsUnavailable</span></span> | <span data-ttu-id="276cd-117">A propriedade **isRequired** do parâmetro [locationConstraint](locationconstraint.md) é especificada como obrigatória, e ainda não existem locais disponíveis nos intervalos de tempo calculados.</span><span class="sxs-lookup"><span data-stu-id="276cd-117">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="276cd-118">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="276cd-118">organizerUnavailable</span></span> | <span data-ttu-id="276cd-119">O parâmetro **isOrganizerOptional** é falso, e o organizador não está disponível durante a janela de tempo solicitada.</span><span class="sxs-lookup"><span data-stu-id="276cd-119">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="276cd-120">unknown</span><span class="sxs-lookup"><span data-stu-id="276cd-120">unknown</span></span> | <span data-ttu-id="276cd-121">O motivo para não retornar qualquer sugestão de reunião não é conhecido.</span><span class="sxs-lookup"><span data-stu-id="276cd-121">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="276cd-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="276cd-122">JSON representation</span></span>

<span data-ttu-id="276cd-123">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="276cd-123">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="276cd-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="276cd-124">Properties</span></span>
| <span data-ttu-id="276cd-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="276cd-125">Property</span></span>     | <span data-ttu-id="276cd-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="276cd-126">Type</span></span>   |<span data-ttu-id="276cd-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="276cd-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="276cd-128">emptySuggestionsHint</span><span class="sxs-lookup"><span data-stu-id="276cd-128">emptySuggestionsHint</span></span>|<span data-ttu-id="276cd-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="276cd-129">String</span></span>|<span data-ttu-id="276cd-p104">Um motivo para não retornar qualquer sugestão de reunião. Os valores possíveis são: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` ou `unknown`.</span><span class="sxs-lookup"><span data-stu-id="276cd-p104">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span>|
|<span data-ttu-id="276cd-132">meetingTimeSlots</span><span class="sxs-lookup"><span data-stu-id="276cd-132">meetingTimeSlots</span></span>|<span data-ttu-id="276cd-133">coleção [meetingTimeCandidate](meetingtimecandidate.md)</span><span class="sxs-lookup"><span data-stu-id="276cd-133">[meetingTimeCandidate](meetingtimecandidate.md) collection</span></span>|<span data-ttu-id="276cd-134">Uma matriz de sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="276cd-134">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeCandidatesResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
