# <a name="rangesort-resource-type"></a><span data-ttu-id="f6b0e-101">Tipo de recurso RangeSort</span><span class="sxs-lookup"><span data-stu-id="f6b0e-101">RangeSort resource type</span></span>

<span data-ttu-id="f6b0e-102">Gerencia as operações de classificação em objetos Range.</span><span class="sxs-lookup"><span data-stu-id="f6b0e-102">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="f6b0e-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="f6b0e-103">Methods</span></span>

| <span data-ttu-id="f6b0e-104">Método</span><span class="sxs-lookup"><span data-stu-id="f6b0e-104">Method</span></span>           | <span data-ttu-id="f6b0e-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f6b0e-105">Return Type</span></span>    |<span data-ttu-id="f6b0e-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6b0e-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f6b0e-107">Aplicar</span><span class="sxs-lookup"><span data-stu-id="f6b0e-107">Apply</span></span>](../api/rangesort_apply.md)|<span data-ttu-id="f6b0e-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f6b0e-108">None</span></span>|<span data-ttu-id="f6b0e-109">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="f6b0e-109">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="f6b0e-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6b0e-110">Properties</span></span>
<span data-ttu-id="f6b0e-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f6b0e-111">None</span></span>

## <a name="relationships"></a><span data-ttu-id="f6b0e-112">Relações</span><span class="sxs-lookup"><span data-stu-id="f6b0e-112">Relationships</span></span>
<span data-ttu-id="f6b0e-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f6b0e-113">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6b0e-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6b0e-114">JSON representation</span></span>

<span data-ttu-id="f6b0e-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f6b0e-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeSort"
}-->

```json
{
}
```

##### <a name="request"></a><span data-ttu-id="f6b0e-116">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6b0e-116">Request</span></span>
<span data-ttu-id="f6b0e-117">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6b0e-117">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="f6b0e-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6b0e-118">Response</span></span>
<span data-ttu-id="f6b0e-119">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6b0e-119">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeSort"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->