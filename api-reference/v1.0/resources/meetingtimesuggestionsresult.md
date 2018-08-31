# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="14ea6-101">Tipo de recurso meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="14ea6-101">meetingTimeSuggestionsResult resource type</span></span>

<span data-ttu-id="14ea6-102">Uma coleção de sugestões de reunião, se houver alguma, ou se não houver motivo.</span><span class="sxs-lookup"><span data-stu-id="14ea6-102">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="14ea6-103">A seguir estão os possíveis motivos que [findMeetingTimes](../api/user_findmeetingtimes.md) não retorna as sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="14ea6-103">The following are the possible reasons that [findMeetingTimes](../api/user_findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="14ea6-104">**valor de emptySuggestionsReason**</span><span class="sxs-lookup"><span data-stu-id="14ea6-104">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="14ea6-105">**Motivos**</span><span class="sxs-lookup"><span data-stu-id="14ea6-105">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="14ea6-106">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="14ea6-106">attendeesUnavailable</span></span> | <span data-ttu-id="14ea6-107">A disponibilidade de todos os participantes é conhecida, mas não há participantes suficientes disponíveis para alcançar o limite de [confiança da reunião](../api/user_findmeetingtimes.md#the-confidence-of-a-meeting-suggestion), que é de 50% por padrão, para qualquer período de tempo.</span><span class="sxs-lookup"><span data-stu-id="14ea6-107">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user_findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="14ea6-108">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="14ea6-108">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="14ea6-p101">Alguns ou todos os participantes têm disponibilidade desconhecida, fazendo com que a confiança na reunião caia para abaixo o limite definido, que é de 50% por padrão. A disponibilidade do participante poderá se tornar desconhecida se ele não for da organização ou se houver um erro ao obter informações sobre a disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="14ea6-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="14ea6-111">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="14ea6-111">locationsUnavailable</span></span> | <span data-ttu-id="14ea6-112">A propriedade **isRequired** do parâmetro [locationConstraint](locationconstraint.md) é especificada como obrigatória, e ainda não existem locais disponíveis nos intervalos de tempo calculados.</span><span class="sxs-lookup"><span data-stu-id="14ea6-112">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="14ea6-113">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="14ea6-113">organizerUnavailable</span></span> | <span data-ttu-id="14ea6-114">O parâmetro **isOrganizerOptional** é falso, e o organizador não está disponível durante a janela de tempo solicitada.</span><span class="sxs-lookup"><span data-stu-id="14ea6-114">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="14ea6-115">unknown</span><span class="sxs-lookup"><span data-stu-id="14ea6-115">unknown</span></span> | <span data-ttu-id="14ea6-116">O motivo para não retornar qualquer sugestão de reunião não é conhecido.</span><span class="sxs-lookup"><span data-stu-id="14ea6-116">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14ea6-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14ea6-117">JSON representation</span></span>

<span data-ttu-id="14ea6-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="14ea6-118">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="14ea6-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14ea6-119">Properties</span></span>
| <span data-ttu-id="14ea6-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14ea6-120">Property</span></span>     | <span data-ttu-id="14ea6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="14ea6-121">Type</span></span>   |<span data-ttu-id="14ea6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="14ea6-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14ea6-123">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="14ea6-123">emptySuggestionsReason</span></span>|<span data-ttu-id="14ea6-124">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="14ea6-124">String</span></span>|<span data-ttu-id="14ea6-125">Um motivo para não retornar sugestões de reuniões.</span><span class="sxs-lookup"><span data-stu-id="14ea6-125">A reason for not returning any meeting suggestions. Possible values are: , , , , or .</span></span> <span data-ttu-id="14ea6-126">Os valores possíveis são: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` ou `unknown`.</span><span class="sxs-lookup"><span data-stu-id="14ea6-126">The possible values are `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, , , , , , , , or `unknown`.</span></span> <span data-ttu-id="14ea6-127">Essa propriedade é uma sequência de caracteres vazia se a propriedade **meetingTimeSuggestions** incluir qualquer sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="14ea6-127">A reason for not returning any meeting suggestions. Possible values are: , , , , or . This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="14ea6-128">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="14ea6-128">meetingTimeSuggestions</span></span>|<span data-ttu-id="14ea6-129">coleção [meetingTimeSuggestion](meetingTimeSuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="14ea6-129">[meetingTimeSuggestion](meetingTimeSuggestion.md) collection</span></span>|<span data-ttu-id="14ea6-130">Uma matriz de sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="14ea6-130">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->