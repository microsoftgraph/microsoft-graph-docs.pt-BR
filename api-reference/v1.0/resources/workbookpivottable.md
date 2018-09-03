# <a name="pivottable-resource-type"></a><span data-ttu-id="b6d3b-101">tipo de recurso de tabela dinâmica</span><span class="sxs-lookup"><span data-stu-id="b6d3b-101">pivotTable resource type</span></span>

<span data-ttu-id="b6d3b-102">Representa uma Tabela Dinâmica do Excel.</span><span class="sxs-lookup"><span data-stu-id="b6d3b-102">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="b6d3b-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="b6d3b-103">Methods</span></span>

| <span data-ttu-id="b6d3b-104">Método</span><span class="sxs-lookup"><span data-stu-id="b6d3b-104">Method</span></span>           | <span data-ttu-id="b6d3b-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b6d3b-105">Return Type</span></span>    |<span data-ttu-id="b6d3b-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6d3b-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b6d3b-107">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="b6d3b-107">Get workbookPivotTable</span></span>](../api/workbookpivottable_get.md) | [<span data-ttu-id="b6d3b-108">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="b6d3b-108">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="b6d3b-109">Leia as propriedades e relacionamentos do objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="b6d3b-109">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="b6d3b-110">Refresh</span><span class="sxs-lookup"><span data-stu-id="b6d3b-110">Refresh</span></span>](../api/workbookpivottable_refresh.md)|<span data-ttu-id="b6d3b-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6d3b-111">None</span></span>|<span data-ttu-id="b6d3b-112">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="b6d3b-112">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="b6d3b-113">Refreshall</span><span class="sxs-lookup"><span data-stu-id="b6d3b-113">Refreshall</span></span>](../api/workbookpivottable_refreshall.md)|<span data-ttu-id="b6d3b-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6d3b-114">None</span></span>|<span data-ttu-id="b6d3b-p101">Atualização de todas as tabelas dentro de uma determinada planilha. Observe que esta ação está disponível somente na coleção de tabela dinâmica.</span><span class="sxs-lookup"><span data-stu-id="b6d3b-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="b6d3b-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6d3b-117">Properties</span></span>
| <span data-ttu-id="b6d3b-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6d3b-118">Property</span></span>     | <span data-ttu-id="b6d3b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6d3b-119">Type</span></span>   |<span data-ttu-id="b6d3b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6d3b-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6d3b-121">id</span><span class="sxs-lookup"><span data-stu-id="b6d3b-121">id</span></span>|<span data-ttu-id="b6d3b-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6d3b-122">String</span></span>| <span data-ttu-id="b6d3b-p102">Id da Tabela Dinâmica.   Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6d3b-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="b6d3b-125">name</span><span class="sxs-lookup"><span data-stu-id="b6d3b-125">name</span></span>|<span data-ttu-id="b6d3b-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6d3b-126">String</span></span>|<span data-ttu-id="b6d3b-127">Nome da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="b6d3b-127">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="b6d3b-128">Relações</span><span class="sxs-lookup"><span data-stu-id="b6d3b-128">Relationships</span></span>
| <span data-ttu-id="b6d3b-129">Relação</span><span class="sxs-lookup"><span data-stu-id="b6d3b-129">Relationship</span></span> | <span data-ttu-id="b6d3b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6d3b-130">Type</span></span>   |<span data-ttu-id="b6d3b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6d3b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6d3b-132">planilha</span><span class="sxs-lookup"><span data-stu-id="b6d3b-132">worksheet</span></span>|[<span data-ttu-id="b6d3b-133">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="b6d3b-133">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="b6d3b-p103">A planilha que contém a Tabela Dinâmica atual. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6d3b-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="b6d3b-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6d3b-136">JSON representation</span></span>
<span data-ttu-id="b6d3b-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6d3b-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
