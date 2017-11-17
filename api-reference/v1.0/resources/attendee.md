# <a name="attendee-resource-type"></a><span data-ttu-id="1cd2a-101">Tipo de recurso attendee</span><span class="sxs-lookup"><span data-stu-id="1cd2a-101">attendee resource type</span></span>

<span data-ttu-id="1cd2a-102">Um participante do evento.</span><span class="sxs-lookup"><span data-stu-id="1cd2a-102">An event attendee.</span></span>

<span data-ttu-id="1cd2a-103">Derivado de [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="1cd2a-103">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1cd2a-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1cd2a-104">Properties</span></span>
| <span data-ttu-id="1cd2a-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1cd2a-105">Property</span></span>     | <span data-ttu-id="1cd2a-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cd2a-106">Type</span></span>   |<span data-ttu-id="1cd2a-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cd2a-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cd2a-108">status</span><span class="sxs-lookup"><span data-stu-id="1cd2a-108">status</span></span>|[<span data-ttu-id="1cd2a-109">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="1cd2a-109">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="1cd2a-110">A resposta do participante (nenhum, aceito, recusado, etc.) para o evento e a data e a hora em que a resposta foi enviada.</span><span class="sxs-lookup"><span data-stu-id="1cd2a-110">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="1cd2a-111">type</span><span class="sxs-lookup"><span data-stu-id="1cd2a-111">type</span></span>|<span data-ttu-id="1cd2a-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1cd2a-112">String</span></span>|<span data-ttu-id="1cd2a-113">O tipo de participante: `Required`, `Optional` ou `Resource`.</span><span class="sxs-lookup"><span data-stu-id="1cd2a-113">The attendee type: `Required`, `Optional`, `Resource`.</span></span>|
|<span data-ttu-id="1cd2a-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1cd2a-114">emailAddress</span></span>|[<span data-ttu-id="1cd2a-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1cd2a-115">emailAddress</span></span>](emailAddress.md)|<span data-ttu-id="1cd2a-116">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="1cd2a-116">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1cd2a-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1cd2a-117">JSON representation</span></span>

<span data-ttu-id="1cd2a-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1cd2a-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->