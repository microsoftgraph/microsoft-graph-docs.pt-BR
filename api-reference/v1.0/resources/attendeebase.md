# <a name="attendeebase-resource-type"></a><span data-ttu-id="6c0b3-101">Tipo de recurso attendeeBase</span><span class="sxs-lookup"><span data-stu-id="6c0b3-101">attendeeBase resource type</span></span>

<span data-ttu-id="6c0b3-102">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="6c0b3-102">The type of attendee.</span></span>

<span data-ttu-id="6c0b3-103">Derivado do [destinatário](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="6c0b3-103">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c0b3-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c0b3-104">JSON representation</span></span>

<span data-ttu-id="6c0b3-105">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6c0b3-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="6c0b3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c0b3-106">Properties</span></span>
| <span data-ttu-id="6c0b3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c0b3-107">Property</span></span>     | <span data-ttu-id="6c0b3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c0b3-108">Type</span></span>   |<span data-ttu-id="6c0b3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c0b3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c0b3-110">type</span><span class="sxs-lookup"><span data-stu-id="6c0b3-110">type</span></span>|<span data-ttu-id="6c0b3-111">attendeeType</span><span class="sxs-lookup"><span data-stu-id="6c0b3-111">AttendeeType</span></span>| <span data-ttu-id="6c0b3-112">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="6c0b3-112">The type of attendee.</span></span> <span data-ttu-id="6c0b3-113">Os valores possíveis são: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="6c0b3-113">The possible values are:</span></span> <span data-ttu-id="6c0b3-114">Atualmente, se o participante for uma pessoa, [findMeetingTimes](../api/user_findmeetingtimes.md) sempre considera que a pessoa é do tipo `Required`.</span><span class="sxs-lookup"><span data-stu-id="6c0b3-114">The type of attendee. Possible values are: , , . Currently if the attendee is a person, [findMeetingTimes](../api/user_findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="6c0b3-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6c0b3-115">emailAddress</span></span>|[<span data-ttu-id="6c0b3-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6c0b3-116">emailAddress</span></span>](emailAddress.md)|<span data-ttu-id="6c0b3-117">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="6c0b3-117">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
