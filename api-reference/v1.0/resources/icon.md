# <a name="icon-resource-type"></a><span data-ttu-id="631a2-101">Tipo de recurso Icon</span><span class="sxs-lookup"><span data-stu-id="631a2-101">Icon resource type</span></span>

<span data-ttu-id="631a2-102">Representa um ícone de célula.</span><span class="sxs-lookup"><span data-stu-id="631a2-102">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="631a2-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="631a2-103">Methods</span></span>

| <span data-ttu-id="631a2-104">Método</span><span class="sxs-lookup"><span data-stu-id="631a2-104">Method</span></span>           | <span data-ttu-id="631a2-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="631a2-105">Return Type</span></span>    |<span data-ttu-id="631a2-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="631a2-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="631a2-107">Obter ícone</span><span class="sxs-lookup"><span data-stu-id="631a2-107">Get Icon</span></span>](../api/icon_get.md) | [<span data-ttu-id="631a2-108">Ícone</span><span class="sxs-lookup"><span data-stu-id="631a2-108">Icon</span></span>](icon.md) |<span data-ttu-id="631a2-109">Propriedades de leitura e relacionamentos do objeto de ícone.</span><span class="sxs-lookup"><span data-stu-id="631a2-109">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="631a2-110">Atualizar</span><span class="sxs-lookup"><span data-stu-id="631a2-110">Update</span></span>](../api/icon_update.md) | [<span data-ttu-id="631a2-111">Ícone</span><span class="sxs-lookup"><span data-stu-id="631a2-111">Icon</span></span>](icon.md)  |<span data-ttu-id="631a2-112">Atualizar o objeto ícone.</span><span class="sxs-lookup"><span data-stu-id="631a2-112">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="631a2-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="631a2-113">Properties</span></span>
| <span data-ttu-id="631a2-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="631a2-114">Property</span></span>     | <span data-ttu-id="631a2-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="631a2-115">Type</span></span>   |<span data-ttu-id="631a2-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="631a2-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="631a2-117">índice</span><span class="sxs-lookup"><span data-stu-id="631a2-117">index</span></span>|<span data-ttu-id="631a2-118">int</span><span class="sxs-lookup"><span data-stu-id="631a2-118">int</span></span>|<span data-ttu-id="631a2-119">Representa o índice do ícone em determinado conjunto.</span><span class="sxs-lookup"><span data-stu-id="631a2-119">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="631a2-120">set</span><span class="sxs-lookup"><span data-stu-id="631a2-120">set</span></span>|<span data-ttu-id="631a2-121">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="631a2-121">string</span></span>|<span data-ttu-id="631a2-122">Representa o conjunto do qual o ícone faz parte.</span><span class="sxs-lookup"><span data-stu-id="631a2-122">Represents the set that the icon is part of. Possible values are: , , , , , , , , , , , , , , , , , , , , .</span></span> <span data-ttu-id="631a2-123">Os valores possíveis são: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="631a2-123">The possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="631a2-124">Relações</span><span class="sxs-lookup"><span data-stu-id="631a2-124">Relationships</span></span>
<span data-ttu-id="631a2-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="631a2-125">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="631a2-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="631a2-126">JSON representation</span></span>

<span data-ttu-id="631a2-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="631a2-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookIcon"
}-->

```json
{
  "index": 1024,
  "set": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->