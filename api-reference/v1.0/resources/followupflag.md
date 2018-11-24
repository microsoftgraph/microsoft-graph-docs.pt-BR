# <a name="followupflag-resource-type"></a><span data-ttu-id="4b7a4-101">Tipo de recurso followupFlag</span><span class="sxs-lookup"><span data-stu-id="4b7a4-101">followupFlag resource type</span></span>


<span data-ttu-id="4b7a4-102">Permite a definição de um sinalizador em um item para o usuário acompanhar posteriormente.</span><span class="sxs-lookup"><span data-stu-id="4b7a4-102">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="4b7a4-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b7a4-103">Properties</span></span>
| <span data-ttu-id="4b7a4-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b7a4-104">Property</span></span>     | <span data-ttu-id="4b7a4-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b7a4-105">Type</span></span>   |<span data-ttu-id="4b7a4-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b7a4-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b7a4-107">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b7a4-107">completedDateTime</span></span>|[<span data-ttu-id="4b7a4-108">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="4b7a4-108">dateTimeTimeZone</span></span>](dateTimeTimeZone.md)|<span data-ttu-id="4b7a4-109">Data e hora em que o acompanhamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="4b7a4-109">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="4b7a4-110">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="4b7a4-110">dueDateTime</span></span>|<span data-ttu-id="4b7a4-111">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="4b7a4-111">**dateTimeTimeZone**</span></span>|<span data-ttu-id="4b7a4-112">Data e hora em que o acompanhamento deve ser concluído.</span><span class="sxs-lookup"><span data-stu-id="4b7a4-112">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="4b7a4-113">flagStatus</span><span class="sxs-lookup"><span data-stu-id="4b7a4-113">flagStatus</span></span>|<span data-ttu-id="4b7a4-114">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="4b7a4-114">followupFlagStatus</span></span>|<span data-ttu-id="4b7a4-115">O status de acompanhamento de um item.</span><span class="sxs-lookup"><span data-stu-id="4b7a4-115">The status for follow-up for an item.</span></span> <span data-ttu-id="4b7a4-116">Os valores possíveis são: `notFlagged`, `complete` e `flagged`.</span><span class="sxs-lookup"><span data-stu-id="4b7a4-116">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="4b7a4-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4b7a4-117">startDateTime</span></span>|<span data-ttu-id="4b7a4-118">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="4b7a4-118">**dateTimeTimeZone**</span></span>|<span data-ttu-id="4b7a4-119">Data e hora em que o acompanhamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="4b7a4-119">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b7a4-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b7a4-120">JSON representation</span></span>

<span data-ttu-id="4b7a4-121">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="4b7a4-121">Here is a JSON representation of the resource</span></span>

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
