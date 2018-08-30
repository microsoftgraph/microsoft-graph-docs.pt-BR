# <a name="formatprotection-resource-type"></a><span data-ttu-id="e3c88-101">Tipo de recurso FormatProtection</span><span class="sxs-lookup"><span data-stu-id="e3c88-101">FormatProtection resource type</span></span>

<span data-ttu-id="e3c88-102">Representa a proteção de formatação de um objeto de intervalo.</span><span class="sxs-lookup"><span data-stu-id="e3c88-102">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="e3c88-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="e3c88-103">Methods</span></span>

| <span data-ttu-id="e3c88-104">Método</span><span class="sxs-lookup"><span data-stu-id="e3c88-104">Method</span></span>           | <span data-ttu-id="e3c88-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e3c88-105">Return Type</span></span>    |<span data-ttu-id="e3c88-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3c88-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e3c88-107">Obter FormatProtection</span><span class="sxs-lookup"><span data-stu-id="e3c88-107">Get FormatProtection</span></span>](../api/formatprotection_get.md) | [<span data-ttu-id="e3c88-108">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="e3c88-108">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="e3c88-109">Leia as propriedades e os relacionamentos do objeto formatProtection.</span><span class="sxs-lookup"><span data-stu-id="e3c88-109">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="e3c88-110">Atualizar</span><span class="sxs-lookup"><span data-stu-id="e3c88-110">Update</span></span>](../api/formatprotection_update.md) | [<span data-ttu-id="e3c88-111">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="e3c88-111">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="e3c88-112">Atualize o objeto FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="e3c88-112">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e3c88-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3c88-113">Properties</span></span>
| <span data-ttu-id="e3c88-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3c88-114">Property</span></span>     | <span data-ttu-id="e3c88-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3c88-115">Type</span></span>   |<span data-ttu-id="e3c88-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3c88-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3c88-117">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="e3c88-117">formulaHidden</span></span>|<span data-ttu-id="e3c88-118">booliano</span><span class="sxs-lookup"><span data-stu-id="e3c88-118">boolean</span></span>|<span data-ttu-id="e3c88-p101">Indica se o Excel ocultará a fórmula para as células no intervalo. Um valor nulo indica que o intervalo inteiro não tem configuração uniforme de fórmula oculta.</span><span class="sxs-lookup"><span data-stu-id="e3c88-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="e3c88-121">locked</span><span class="sxs-lookup"><span data-stu-id="e3c88-121">locked</span></span>|<span data-ttu-id="e3c88-122">booliano</span><span class="sxs-lookup"><span data-stu-id="e3c88-122">boolean</span></span>|<span data-ttu-id="e3c88-p102">Indica se o Excel bloqueia as células no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de bloqueio uniforme.</span><span class="sxs-lookup"><span data-stu-id="e3c88-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3c88-125">Relações</span><span class="sxs-lookup"><span data-stu-id="e3c88-125">Relationships</span></span>
<span data-ttu-id="e3c88-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3c88-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e3c88-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3c88-127">JSON representation</span></span>

<span data-ttu-id="e3c88-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3c88-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFormatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->