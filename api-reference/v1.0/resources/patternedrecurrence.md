# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="9f017-101">Tipo de recurso patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="9f017-101">patternedRecurrence resource type</span></span>

<span data-ttu-id="9f017-102">O padrão e o intervalo da recorrência.</span><span class="sxs-lookup"><span data-stu-id="9f017-102">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="9f017-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f017-103">Properties</span></span>
| <span data-ttu-id="9f017-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f017-104">Property</span></span>     | <span data-ttu-id="9f017-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f017-105">Type</span></span>   |<span data-ttu-id="9f017-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f017-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f017-107">pattern</span><span class="sxs-lookup"><span data-stu-id="9f017-107">pattern</span></span>|[<span data-ttu-id="9f017-108">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="9f017-108">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="9f017-109">A frequência de um evento.</span><span class="sxs-lookup"><span data-stu-id="9f017-109">The frequency of an event.</span></span>|
|<span data-ttu-id="9f017-110">range</span><span class="sxs-lookup"><span data-stu-id="9f017-110">range</span></span>|[<span data-ttu-id="9f017-111">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="9f017-111">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="9f017-112">A duração de um evento.</span><span class="sxs-lookup"><span data-stu-id="9f017-112">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f017-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f017-113">JSON representation</span></span>

<span data-ttu-id="9f017-114">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9f017-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedrecurrence"
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