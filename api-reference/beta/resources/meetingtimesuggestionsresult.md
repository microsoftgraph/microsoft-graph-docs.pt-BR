---
title: Tipo de recurso meetingTimeSuggestionsResult
description: Uma coleção de sugestões de reunião, se houver alguma, ou se não houver motivo.
ms.openlocfilehash: 2c6cb28ea0ec899e693300b321c652fb814582f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039774"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="52d89-103">Tipo de recurso meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="52d89-103">meetingTimeSuggestionsResult resource type</span></span>

> <span data-ttu-id="52d89-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="52d89-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52d89-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="52d89-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="52d89-106">Uma coleção de sugestões de reunião, se houver alguma, ou se não houver motivo.</span><span class="sxs-lookup"><span data-stu-id="52d89-106">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="52d89-107">A seguir estão os possíveis motivos que [findMeetingTimes](../api/user-findmeetingtimes.md) não retorna as sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="52d89-107">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="52d89-108">**valor de emptySuggestionsReason**</span><span class="sxs-lookup"><span data-stu-id="52d89-108">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="52d89-109">**Motivos**</span><span class="sxs-lookup"><span data-stu-id="52d89-109">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="52d89-110">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="52d89-110">attendeesUnavailable</span></span> | <span data-ttu-id="52d89-111">A disponibilidade de todos os participantes é conhecida, mas não há participantes suficientes disponíveis para alcançar o limite de [confiança da reunião](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion), que é de 50% por padrão, para qualquer período de tempo.</span><span class="sxs-lookup"><span data-stu-id="52d89-111">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="52d89-112">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="52d89-112">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="52d89-p102">Alguns ou todos os participantes têm disponibilidade desconhecida, fazendo com que a confiança na reunião caia para abaixo o limite definido, que é de 50% por padrão. A disponibilidade do participante poderá se tornar desconhecida se ele não for da organização ou se houver um erro ao obter informações sobre a disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="52d89-p102">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="52d89-115">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="52d89-115">locationsUnavailable</span></span> | <span data-ttu-id="52d89-116">A propriedade **isRequired** do parâmetro [locationConstraint](locationconstraint.md) é especificada como obrigatória, e ainda não existem locais disponíveis nos intervalos de tempo calculados.</span><span class="sxs-lookup"><span data-stu-id="52d89-116">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="52d89-117">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="52d89-117">organizerUnavailable</span></span> | <span data-ttu-id="52d89-118">O parâmetro **isOrganizerOptional** é falso, e o organizador não está disponível durante a janela de tempo solicitada.</span><span class="sxs-lookup"><span data-stu-id="52d89-118">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="52d89-119">unknown</span><span class="sxs-lookup"><span data-stu-id="52d89-119">unknown</span></span> | <span data-ttu-id="52d89-120">O motivo para não retornar qualquer sugestão de reunião não é conhecido.</span><span class="sxs-lookup"><span data-stu-id="52d89-120">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52d89-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52d89-121">JSON representation</span></span>

<span data-ttu-id="52d89-122">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="52d89-122">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="52d89-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52d89-123">Properties</span></span>
| <span data-ttu-id="52d89-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52d89-124">Property</span></span>     | <span data-ttu-id="52d89-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="52d89-125">Type</span></span>   |<span data-ttu-id="52d89-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="52d89-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52d89-127">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="52d89-127">emptySuggestionsReason</span></span>|<span data-ttu-id="52d89-128">String</span><span class="sxs-lookup"><span data-stu-id="52d89-128">String</span></span>|<span data-ttu-id="52d89-p103">Um motivo para não retornar qualquer sugestão de reunião. Os valores possíveis são: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` ou `unknown`. Essa propriedade será uma cadeia de caracteres vazia se a propriedade **meetingTimeSuggestions** incluir sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="52d89-p103">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`. This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="52d89-132">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="52d89-132">meetingTimeSuggestions</span></span>|<span data-ttu-id="52d89-133">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span><span class="sxs-lookup"><span data-stu-id="52d89-133">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="52d89-134">Uma matriz de sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="52d89-134">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->