# <a name="sortfield-resource-type"></a><span data-ttu-id="ae901-101">Tipo de recurso SortField</span><span class="sxs-lookup"><span data-stu-id="ae901-101">SortField resource type</span></span>

<span data-ttu-id="ae901-102">Representa uma condição em uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="ae901-102">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="ae901-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae901-103">Properties</span></span>
| <span data-ttu-id="ae901-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae901-104">Property</span></span>     | <span data-ttu-id="ae901-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae901-105">Type</span></span>   |<span data-ttu-id="ae901-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae901-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae901-107">ascendente</span><span class="sxs-lookup"><span data-stu-id="ae901-107">ascending</span></span>|<span data-ttu-id="ae901-108">booliano</span><span class="sxs-lookup"><span data-stu-id="ae901-108">boolean</span></span>|<span data-ttu-id="ae901-109">Indica se a classificação é feita de forma crescente.</span><span class="sxs-lookup"><span data-stu-id="ae901-109">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="ae901-110">cor</span><span class="sxs-lookup"><span data-stu-id="ae901-110">color</span></span>|<span data-ttu-id="ae901-111">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae901-111">string</span></span>|<span data-ttu-id="ae901-112">Representa a cor que é o destino da condição se a classificação estiver na cor da fonte ou da célula.</span><span class="sxs-lookup"><span data-stu-id="ae901-112">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="ae901-113">dataOption</span><span class="sxs-lookup"><span data-stu-id="ae901-113">dataOption</span></span>|<span data-ttu-id="ae901-114">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae901-114">string</span></span>|<span data-ttu-id="ae901-115">Representa as opções de classificação adicionais para esse campo.</span><span class="sxs-lookup"><span data-stu-id="ae901-115">Represents additional sorting options for this field. Possible values are: , .</span></span> <span data-ttu-id="ae901-116">Os valores possíveis são: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="ae901-116">The possible values are:</span></span>|
|<span data-ttu-id="ae901-117">chave</span><span class="sxs-lookup"><span data-stu-id="ae901-117">key</span></span>|<span data-ttu-id="ae901-118">int</span><span class="sxs-lookup"><span data-stu-id="ae901-118">int</span></span>|<span data-ttu-id="ae901-p102">Representa a coluna (ou linha, dependendo da orientação da classificação) em que a condição está. Representado como um deslocamento da primeira coluna (ou linha).</span><span class="sxs-lookup"><span data-stu-id="ae901-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="ae901-121">sortOn</span><span class="sxs-lookup"><span data-stu-id="ae901-121">sortOn</span></span>|<span data-ttu-id="ae901-122">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae901-122">string</span></span>|<span data-ttu-id="ae901-123">Representa o tipo de classificação dessa condição.</span><span class="sxs-lookup"><span data-stu-id="ae901-123">Represents the type of sorting of this condition. Possible values are: , , , .</span></span> <span data-ttu-id="ae901-124">Os valores possíveis são: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="ae901-124">The possible values are `Value`, `CellColor`, `FontColor`, `Icon`, , , , , , , , or .</span></span>|
|<span data-ttu-id="ae901-125">ícone</span><span class="sxs-lookup"><span data-stu-id="ae901-125">icon</span></span>|[<span data-ttu-id="ae901-126">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="ae901-126">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="ae901-127">Representa o ícone que é o destino da condição, se a classificação estiver no ícone da célula.</span><span class="sxs-lookup"><span data-stu-id="ae901-127">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae901-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae901-128">JSON representation</span></span>

<span data-ttu-id="ae901-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae901-129">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->