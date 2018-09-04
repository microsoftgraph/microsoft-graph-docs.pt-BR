# <a name="tablesort-resource-type"></a><span data-ttu-id="6894d-101">Tipo de recurso TableSort</span><span class="sxs-lookup"><span data-stu-id="6894d-101">TableSort resource type</span></span>

<span data-ttu-id="6894d-102">Gerencia operações de classificação em objetos Table.</span><span class="sxs-lookup"><span data-stu-id="6894d-102">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="6894d-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="6894d-103">Methods</span></span>

| <span data-ttu-id="6894d-104">Método</span><span class="sxs-lookup"><span data-stu-id="6894d-104">Method</span></span>           | <span data-ttu-id="6894d-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6894d-105">Return Type</span></span>    |<span data-ttu-id="6894d-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="6894d-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6894d-107">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="6894d-107">Get TableSort</span></span>](../api/tablesort_get.md) | [<span data-ttu-id="6894d-108">WorkbookTableSort</span><span class="sxs-lookup"><span data-stu-id="6894d-108">WorkbookTableSort</span></span>](tablesort.md) |<span data-ttu-id="6894d-109">Lê as propriedades e os relacionamentos do objeto tableSort.</span><span class="sxs-lookup"><span data-stu-id="6894d-109">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="6894d-110">Apply</span><span class="sxs-lookup"><span data-stu-id="6894d-110">Apply</span></span>](../api/tablesort_apply.md)|<span data-ttu-id="6894d-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6894d-111">None</span></span>|<span data-ttu-id="6894d-112">Executa uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="6894d-112">Perform a sort operation.</span></span>|
|[<span data-ttu-id="6894d-113">Clear</span><span class="sxs-lookup"><span data-stu-id="6894d-113">Clear</span></span>](../api/tablesort_clear.md)|<span data-ttu-id="6894d-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6894d-114">None</span></span>|<span data-ttu-id="6894d-p101">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="6894d-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="6894d-117">Reapply</span><span class="sxs-lookup"><span data-stu-id="6894d-117">Reapply</span></span>](../api/tablesort_reapply.md)|<span data-ttu-id="6894d-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6894d-118">None</span></span>|<span data-ttu-id="6894d-119">Reaplica os parâmetros de classificação atuais à tabela.</span><span class="sxs-lookup"><span data-stu-id="6894d-119">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="6894d-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6894d-120">Properties</span></span>
| <span data-ttu-id="6894d-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6894d-121">Property</span></span>     | <span data-ttu-id="6894d-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="6894d-122">Type</span></span>   |<span data-ttu-id="6894d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6894d-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6894d-124">fields</span><span class="sxs-lookup"><span data-stu-id="6894d-124">fields</span></span>|<span data-ttu-id="6894d-125">Coleção [WorkbookSortField](sortfield.md)</span><span class="sxs-lookup"><span data-stu-id="6894d-125">[WorkbookSortField](sortfield.md) collection</span></span>|<span data-ttu-id="6894d-p102">Representa as condições atuais usadas para a última classificação da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6894d-p102">Represents the current conditions used to last sort the table. Read-only.</span></span>|
|<span data-ttu-id="6894d-128">matchCase</span><span class="sxs-lookup"><span data-stu-id="6894d-128">matchCase</span></span>|<span data-ttu-id="6894d-129">booliano</span><span class="sxs-lookup"><span data-stu-id="6894d-129">boolean</span></span>|<span data-ttu-id="6894d-p103">Indica se o uso de maiúsculas ou minúsculas afetou a última classificação da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6894d-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="6894d-132">method</span><span class="sxs-lookup"><span data-stu-id="6894d-132">method</span></span>|<span data-ttu-id="6894d-133">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="6894d-133">string</span></span>|<span data-ttu-id="6894d-134">Indica o último método de ordenação de caracteres chineses usado para classificar a tabela.</span><span class="sxs-lookup"><span data-stu-id="6894d-134">Represents Chinese character ordering method last used to sort the table. Possible values are: , . Read-only.</span></span> <span data-ttu-id="6894d-135">Os valores possíveis são: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="6894d-135">The possible values are:</span></span> <span data-ttu-id="6894d-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6894d-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6894d-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6894d-137">JSON representation</span></span>

<span data-ttu-id="6894d-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6894d-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->