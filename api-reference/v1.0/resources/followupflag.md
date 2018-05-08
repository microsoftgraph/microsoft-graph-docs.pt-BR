# <a name="followupflag-resource-type"></a><span data-ttu-id="ba9a4-101">Tipo de recurso followupFlag</span><span class="sxs-lookup"><span data-stu-id="ba9a4-101">followupFlag resource type</span></span>


<span data-ttu-id="ba9a4-102">Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente.</span><span class="sxs-lookup"><span data-stu-id="ba9a4-102">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="ba9a4-103">Os itens com suporte incluem [message](message.md) e [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="ba9a4-103">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ba9a4-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba9a4-104">Properties</span></span>
| <span data-ttu-id="ba9a4-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba9a4-105">Property</span></span>     | <span data-ttu-id="ba9a4-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba9a4-106">Type</span></span>   |<span data-ttu-id="ba9a4-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba9a4-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba9a4-108">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba9a4-108">completedDateTime</span></span>|[<span data-ttu-id="ba9a4-109">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ba9a4-109">dateTimeTimeZone</span></span>](dateTimeTimeZone.md)|<span data-ttu-id="ba9a4-110">Data e hora em que o acompanhamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="ba9a4-110">The date and time that the response was returned.</span></span>|
|<span data-ttu-id="ba9a4-111">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="ba9a4-111">dueDateTime</span></span>|<span data-ttu-id="ba9a4-112">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="ba9a4-112">**dateTimeTimeZone**</span></span>|<span data-ttu-id="ba9a4-113">Data e hora em que o acompanhamento deve ser concluído.</span><span class="sxs-lookup"><span data-stu-id="ba9a4-113">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="ba9a4-114">flagStatus</span><span class="sxs-lookup"><span data-stu-id="ba9a4-114">flagStatus</span></span>|<span data-ttu-id="ba9a4-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba9a4-115">String</span></span>|<span data-ttu-id="ba9a4-116">O status de acompanhamento de um item.</span><span class="sxs-lookup"><span data-stu-id="ba9a4-116">The status for follow-up for an item.</span></span> <span data-ttu-id="ba9a4-117">Os valores possíveis são: `notFlagged`, `complete` e `flagged`.</span><span class="sxs-lookup"><span data-stu-id="ba9a4-117">Possible values are: `notFlagged`, `complete`, `flagged`, .</span></span>|
|<span data-ttu-id="ba9a4-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ba9a4-118">startDateTime</span></span>|<span data-ttu-id="ba9a4-119">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="ba9a4-119">**dateTimeTimeZone**</span></span>|<span data-ttu-id="ba9a4-120">Data e hora em que o acompanhamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="ba9a4-120">Gets or sets the date and time that the appointment is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba9a4-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba9a4-121">JSON representation</span></span>

<span data-ttu-id="ba9a4-122">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ba9a4-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
