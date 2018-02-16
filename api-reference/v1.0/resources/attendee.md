# <a name="attendee-resource-type"></a><span data-ttu-id="af04d-101">Tipo de recurso attendee</span><span class="sxs-lookup"><span data-stu-id="af04d-101">attendee resource type</span></span>

<span data-ttu-id="af04d-102">Um participante do evento.</span><span class="sxs-lookup"><span data-stu-id="af04d-102">An event attendee.</span></span> <span data-ttu-id="af04d-103">Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.</span><span class="sxs-lookup"><span data-stu-id="af04d-103">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="af04d-104">Derivado de [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="af04d-104">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="af04d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af04d-105">Properties</span></span>
| <span data-ttu-id="af04d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af04d-106">Property</span></span>     | <span data-ttu-id="af04d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="af04d-107">Type</span></span>   |<span data-ttu-id="af04d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="af04d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af04d-109">status</span><span class="sxs-lookup"><span data-stu-id="af04d-109">status</span></span>|[<span data-ttu-id="af04d-110">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="af04d-110">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="af04d-111">A resposta do participante (nenhum, aceito, recusado, etc.) para o evento e a data e a hora em que a resposta foi enviada.</span><span class="sxs-lookup"><span data-stu-id="af04d-111">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="af04d-112">type</span><span class="sxs-lookup"><span data-stu-id="af04d-112">type</span></span>|<span data-ttu-id="af04d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af04d-113">String</span></span>|<span data-ttu-id="af04d-114">O tipo de participante: `required`, `optional` ou `resource`.</span><span class="sxs-lookup"><span data-stu-id="af04d-114">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="af04d-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="af04d-115">emailAddress</span></span>|[<span data-ttu-id="af04d-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="af04d-116">emailAddress</span></span>](emailAddress.md)|<span data-ttu-id="af04d-117">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="af04d-117">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af04d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af04d-118">JSON representation</span></span>

<span data-ttu-id="af04d-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="af04d-119">Here is a JSON representation of the resource</span></span>

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