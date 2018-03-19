# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="a00e7-101">Tipo de recurso meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="a00e7-101">meetingTimeSuggestionsResult resource type</span></span>

<span data-ttu-id="a00e7-102">Uma coleção de sugestões de reunião, se houver alguma, ou se não houver motivo.</span><span class="sxs-lookup"><span data-stu-id="a00e7-102">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="a00e7-103">A seguir estão os possíveis motivos que [findMeetingTimes](../api/user_findmeetingtimes.md) não retorna as sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="a00e7-103">The following are the possible reasons that [findMeetingTimes](../api/user_findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="a00e7-104">**valor de emptySuggestionsReason**</span><span class="sxs-lookup"><span data-stu-id="a00e7-104">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="a00e7-105">**Motivos**</span><span class="sxs-lookup"><span data-stu-id="a00e7-105">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="a00e7-106">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="a00e7-106">attendeesUnavailable</span></span> | <span data-ttu-id="a00e7-107">A disponibilidade de todos os participantes é conhecida, mas não há participantes suficientes disponíveis para alcançar o limite de [confiança da reunião](../api/user_findmeetingtimes.md#the-confidence-of-a-meeting-suggestion), que é de 50% por padrão, para qualquer período de tempo.</span><span class="sxs-lookup"><span data-stu-id="a00e7-107">All of the attendees' availability is known, but not enough attendees are available to reach the meeting confidence threshold, which is 50% by default, for any time period. This threshold is based on the attendees' free/busy status for a suggested meeting time period, with an attendee's free status corresponding to 100% chance of attendance, unknown status 49%, and busy status 0%.</span></span>|
| <span data-ttu-id="a00e7-108">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="a00e7-108">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="a00e7-p101">Alguns ou todos os participantes têm disponibilidade desconhecida, fazendo com que a confiança na reunião caia para abaixo o limite definido, que é de 50% por padrão. A disponibilidade do participante poderá se tornar desconhecida se ele não for da organização ou se houver um erro ao obter informações sobre a disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="a00e7-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="a00e7-111">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="a00e7-111">locationsUnavailable</span></span> | <span data-ttu-id="a00e7-112">A propriedade **isRequired** do parâmetro [locationConstraint](locationconstraint.md) é especificada como obrigatória, e ainda não existem locais disponíveis nos intervalos de tempo calculados.</span><span class="sxs-lookup"><span data-stu-id="a00e7-112">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="a00e7-113">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="a00e7-113">organizerUnavailable</span></span> | <span data-ttu-id="a00e7-114">O parâmetro **isOrganizerOptional** é falso, e o organizador não está disponível durante a janela de tempo solicitada.</span><span class="sxs-lookup"><span data-stu-id="a00e7-114">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="a00e7-115">unknown</span><span class="sxs-lookup"><span data-stu-id="a00e7-115">unknown</span></span> | <span data-ttu-id="a00e7-116">O motivo para não retornar qualquer sugestão de reunião não é conhecido.</span><span class="sxs-lookup"><span data-stu-id="a00e7-116">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a00e7-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a00e7-117">JSON representation</span></span>

<span data-ttu-id="a00e7-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a00e7-118">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="a00e7-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a00e7-119">Properties</span></span>
| <span data-ttu-id="a00e7-120">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="a00e7-120">Property</span></span>       | <span data-ttu-id="a00e7-121">Tipo	</span><span class="sxs-lookup"><span data-stu-id="a00e7-121">Type</span></span>    |<span data-ttu-id="a00e7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a00e7-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a00e7-123">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="a00e7-123">emptySuggestionsReason</span></span>|<span data-ttu-id="a00e7-124">String</span><span class="sxs-lookup"><span data-stu-id="a00e7-124">String</span></span>|<span data-ttu-id="a00e7-p102">Um motivo para não retornar qualquer sugestão de reunião. Os valores possíveis são: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` ou `unknown`. Essa propriedade será uma cadeia de caracteres vazia se a propriedade **meetingTimeSuggestions** incluir sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="a00e7-p102">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`. This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="a00e7-128">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="a00e7-128">meetingTimeSuggestions</span></span>|<span data-ttu-id="a00e7-129">[meetingTimeSuggestion](meetingTimeSuggestion.md) collection</span><span class="sxs-lookup"><span data-stu-id="a00e7-129">[meetingTimeSuggestion](meetingTimeSuggestion.md) collection</span></span>|<span data-ttu-id="a00e7-130">Uma matriz de sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="a00e7-130">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->