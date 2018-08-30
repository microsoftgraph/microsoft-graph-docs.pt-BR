# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="2f017-101">Tipo de recurso meetingTimeSuggestion</span><span class="sxs-lookup"><span data-stu-id="2f017-101">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="2f017-102">Uma sugestão de reunião que inclui informações como o horário da reunião, a probabilidade de presença, a disponibilidade individual e os locais de reunião disponíveis.</span><span class="sxs-lookup"><span data-stu-id="2f017-102">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f017-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2f017-103">JSON representation</span></span>

<span data-ttu-id="2f017-104">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2f017-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 100.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="2f017-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2f017-105">Properties</span></span>
| <span data-ttu-id="2f017-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f017-106">Property</span></span>     | <span data-ttu-id="2f017-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f017-107">Type</span></span>   |<span data-ttu-id="2f017-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f017-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f017-109">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="2f017-109">attendeeAvailability</span></span>|<span data-ttu-id="2f017-110">Coleção de [attendeeAvailability](attendeeavailability.md)</span><span class="sxs-lookup"><span data-stu-id="2f017-110">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="2f017-111">Uma matriz que mostra o status de disponibilidade de cada participante para essa sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="2f017-111">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="2f017-112">confidence</span><span class="sxs-lookup"><span data-stu-id="2f017-112">confidence</span></span>|<span data-ttu-id="2f017-113">Double</span><span class="sxs-lookup"><span data-stu-id="2f017-113">Double</span></span>|<span data-ttu-id="2f017-114">Uma porcentagem que representa a probabilidade de todos os participantes comparecerem.</span><span class="sxs-lookup"><span data-stu-id="2f017-114">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="2f017-115">locations</span><span class="sxs-lookup"><span data-stu-id="2f017-115">locations</span></span>|<span data-ttu-id="2f017-116">Coleção de [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="2f017-116">[location](location.md) collection</span></span>|<span data-ttu-id="2f017-117">Uma matriz que especifica o nome e a localização geográfica de cada local da reunião para essa sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="2f017-117">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="2f017-118">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="2f017-118">meetingTimeSlot</span></span>|[<span data-ttu-id="2f017-119">timeSlot</span><span class="sxs-lookup"><span data-stu-id="2f017-119">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="2f017-120">Um período de tempo sugerido para a reunião.</span><span class="sxs-lookup"><span data-stu-id="2f017-120">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="2f017-121">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="2f017-121">organizerAvailability</span></span>|<span data-ttu-id="2f017-122">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="2f017-122">FreeBusyStatus</span></span>| <span data-ttu-id="2f017-123">Disponibilidade do organizador da reunião para essa sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="2f017-123">Availability of the meeting organizer for this meeting suggestion. Possible values are: , , , , , .</span></span> <span data-ttu-id="2f017-124">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="2f017-124">The possible values are `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`, , , , , , or .</span></span>|
|<span data-ttu-id="2f017-125">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="2f017-125">suggestionReason</span></span>|<span data-ttu-id="2f017-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f017-126">String</span></span>|<span data-ttu-id="2f017-127">Razão da sugestão de horário da reunião.</span><span class="sxs-lookup"><span data-stu-id="2f017-127">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->