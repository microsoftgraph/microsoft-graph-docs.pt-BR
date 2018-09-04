# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="01398-101">Tipo de recurso attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="01398-101">attendeeAvailability resource type</span></span>

<span data-ttu-id="01398-102">O tipo e a disponibilidade dos participantes.</span><span class="sxs-lookup"><span data-stu-id="01398-102">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="01398-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="01398-103">JSON representation</span></span>

<span data-ttu-id="01398-104">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="01398-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="01398-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="01398-105">Properties</span></span>
| <span data-ttu-id="01398-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01398-106">Property</span></span>     | <span data-ttu-id="01398-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="01398-107">Type</span></span>   |<span data-ttu-id="01398-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="01398-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01398-109">attendee</span><span class="sxs-lookup"><span data-stu-id="01398-109">attendee</span></span>|[<span data-ttu-id="01398-110">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="01398-110">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="01398-111">O tipo de participante, ou seja, se é um recurso ou uma pessoa e, no caso de uma pessoa, se é obrigatório ou opcional.</span><span class="sxs-lookup"><span data-stu-id="01398-111">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="01398-112">availability</span><span class="sxs-lookup"><span data-stu-id="01398-112">availability</span></span>|<span data-ttu-id="01398-113">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="01398-113">FreeBusyStatus</span></span>| <span data-ttu-id="01398-114">O status de disponibilidade do participante.</span><span class="sxs-lookup"><span data-stu-id="01398-114">The availability status of the attendee. Possible values are: , , , , , .</span></span> <span data-ttu-id="01398-115">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="01398-115">The possible values are `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`, , , , , , or .</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
