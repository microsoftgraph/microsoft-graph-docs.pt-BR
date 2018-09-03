# <a name="filter-resource-type"></a><span data-ttu-id="03415-101">Tipo de recurso Filter</span><span class="sxs-lookup"><span data-stu-id="03415-101">Filter resource type</span></span>

<span data-ttu-id="03415-102">Gerencia a filtragem da coluna de uma tabela.</span><span class="sxs-lookup"><span data-stu-id="03415-102">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="03415-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="03415-103">Methods</span></span>

| <span data-ttu-id="03415-104">Método</span><span class="sxs-lookup"><span data-stu-id="03415-104">Method</span></span>           | <span data-ttu-id="03415-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="03415-105">Return Type</span></span>    |<span data-ttu-id="03415-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="03415-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="03415-107">Aplicar</span><span class="sxs-lookup"><span data-stu-id="03415-107">Apply</span></span>](../api/filter_apply.md)|<span data-ttu-id="03415-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03415-108">None</span></span>|<span data-ttu-id="03415-109">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="03415-109">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="03415-110">Limpar</span><span class="sxs-lookup"><span data-stu-id="03415-110">Clear</span></span>](../api/filter_clear.md)|<span data-ttu-id="03415-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03415-111">None</span></span>|<span data-ttu-id="03415-112">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="03415-112">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="03415-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03415-113">Properties</span></span>

| <span data-ttu-id="03415-114">Nome</span><span class="sxs-lookup"><span data-stu-id="03415-114">Name</span></span> | <span data-ttu-id="03415-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="03415-115">Type</span></span>   |<span data-ttu-id="03415-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="03415-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03415-117">critérios</span><span class="sxs-lookup"><span data-stu-id="03415-117">criteria</span></span>|[<span data-ttu-id="03415-118">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="03415-118">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="03415-p101">O filtro aplicado no momento à coluna fornecida. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03415-p101">The currently applied filter on the given column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03415-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03415-121">JSON representation</span></span>

<span data-ttu-id="03415-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03415-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->