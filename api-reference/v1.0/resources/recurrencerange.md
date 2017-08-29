# <a name="recurrencerange-resource-type"></a><span data-ttu-id="642a6-101">Tipo de recurso recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="642a6-101">recurrenceRange resource type</span></span>

<span data-ttu-id="642a6-102">A duração de um evento.</span><span class="sxs-lookup"><span data-stu-id="642a6-102">The duration of an event.</span></span>

## <a name="properties"></a><span data-ttu-id="642a6-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="642a6-103">Properties</span></span>

| <span data-ttu-id="642a6-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="642a6-104">Property</span></span>     | <span data-ttu-id="642a6-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="642a6-105">Type</span></span>   |<span data-ttu-id="642a6-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="642a6-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="642a6-107">endDate</span><span class="sxs-lookup"><span data-stu-id="642a6-107">endDate</span></span>|<span data-ttu-id="642a6-108">Date</span><span class="sxs-lookup"><span data-stu-id="642a6-108">Date</span></span>|<span data-ttu-id="642a6-109">A data de término da série.</span><span class="sxs-lookup"><span data-stu-id="642a6-109">The end date of the series.</span></span>|
|<span data-ttu-id="642a6-110">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="642a6-110">numberOfOccurrences</span></span>|<span data-ttu-id="642a6-111">Int32</span><span class="sxs-lookup"><span data-stu-id="642a6-111">Int32</span></span>|<span data-ttu-id="642a6-112">Quantas vezes o evento deve repetir.</span><span class="sxs-lookup"><span data-stu-id="642a6-112">How many times to repeat the event.</span></span>|
|<span data-ttu-id="642a6-113">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="642a6-113">recurrenceTimeZone</span></span>|<span data-ttu-id="642a6-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="642a6-114">String</span></span> |<span data-ttu-id="642a6-115">Fuso horários das propriedades **startDate** e **endDate**.</span><span class="sxs-lookup"><span data-stu-id="642a6-115">Time zone for the **startDate** and **endDate** properties.</span></span> |
|<span data-ttu-id="642a6-116">startDate</span><span class="sxs-lookup"><span data-stu-id="642a6-116">startDate</span></span>|<span data-ttu-id="642a6-117">Date</span><span class="sxs-lookup"><span data-stu-id="642a6-117">Date</span></span>|<span data-ttu-id="642a6-118">A data de início da série.</span><span class="sxs-lookup"><span data-stu-id="642a6-118">The start date of the series.</span></span>|
|<span data-ttu-id="642a6-119">type</span><span class="sxs-lookup"><span data-stu-id="642a6-119">type</span></span>|<span data-ttu-id="642a6-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="642a6-120">String</span></span>|<span data-ttu-id="642a6-p101">O intervalo de recorrência: EndDate = 0, NoEnd = 1, Numbered = 2. Os valores possíveis são: `EndDate`, `NoEnd` e `Numbered`.</span><span class="sxs-lookup"><span data-stu-id="642a6-p101">The recurrence range: EndDate = 0, NoEnd = 1, Numbered = 2. Possible values are: `EndDate`, `NoEnd`, `Numbered`.</span></span>||

## <a name="json-representation"></a><span data-ttu-id="642a6-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="642a6-123">JSON representation</span></span>

<span data-ttu-id="642a6-124">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="642a6-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencerange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
