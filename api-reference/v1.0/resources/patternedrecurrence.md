# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="e7c04-101">Tipo de recurso patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="e7c04-101">patternedRecurrence resource type</span></span>

<span data-ttu-id="e7c04-102">O padrão e o intervalo da recorrência.</span><span class="sxs-lookup"><span data-stu-id="e7c04-102">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="e7c04-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e7c04-103">Properties</span></span>
| <span data-ttu-id="e7c04-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7c04-104">Property</span></span>     | <span data-ttu-id="e7c04-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7c04-105">Type</span></span>   |<span data-ttu-id="e7c04-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7c04-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7c04-107">pattern</span><span class="sxs-lookup"><span data-stu-id="e7c04-107">pattern</span></span>|[<span data-ttu-id="e7c04-108">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="e7c04-108">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="e7c04-109">A frequência de um evento.</span><span class="sxs-lookup"><span data-stu-id="e7c04-109">The frequency of an event.</span></span>|
|<span data-ttu-id="e7c04-110">range</span><span class="sxs-lookup"><span data-stu-id="e7c04-110">range</span></span>|[<span data-ttu-id="e7c04-111">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="e7c04-111">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="e7c04-112">A duração de um evento.</span><span class="sxs-lookup"><span data-stu-id="e7c04-112">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7c04-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e7c04-113">JSON representation</span></span>

<span data-ttu-id="e7c04-114">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e7c04-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedRecurrence"
}-->

```json
{
  "pattern": {"@odata.type": "microsoft.graph.recurrencePattern"},
  "range": {"@odata.type": "microsoft.graph.recurrenceRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->