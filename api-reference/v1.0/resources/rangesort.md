---
title: Tipo de recurso RangeSort
description: Gerencia operações de classificação em objetos Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3204a72fe51d3afd3771c0e6775138277ef450e2
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601141"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="5ca14-103">Tipo de recurso RangeSort</span><span class="sxs-lookup"><span data-stu-id="5ca14-103">RangeSort resource type</span></span>

<span data-ttu-id="5ca14-104">Gerencia operações de classificação em objetos Range.</span><span class="sxs-lookup"><span data-stu-id="5ca14-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="5ca14-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="5ca14-105">Methods</span></span>

| <span data-ttu-id="5ca14-106">Método</span><span class="sxs-lookup"><span data-stu-id="5ca14-106">Method</span></span>           | <span data-ttu-id="5ca14-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5ca14-107">Return Type</span></span>    |<span data-ttu-id="5ca14-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ca14-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5ca14-109">Apply</span><span class="sxs-lookup"><span data-stu-id="5ca14-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="5ca14-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5ca14-110">None</span></span>|<span data-ttu-id="5ca14-111">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="5ca14-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="5ca14-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ca14-112">Properties</span></span>
<span data-ttu-id="5ca14-113">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="5ca14-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="5ca14-114">Relações</span><span class="sxs-lookup"><span data-stu-id="5ca14-114">Relationships</span></span>
<span data-ttu-id="5ca14-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5ca14-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ca14-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ca14-116">JSON representation</span></span>

<span data-ttu-id="5ca14-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ca14-117">Here is a JSON representation of the resource.</span></span>

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

##### <a name="request"></a><span data-ttu-id="5ca14-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca14-118">Request</span></span>
<span data-ttu-id="5ca14-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ca14-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="5ca14-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ca14-120">Response</span></span>
<span data-ttu-id="5ca14-121">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ca14-121">Here is an example of the response.</span></span> 
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5ca14-122">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5ca14-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5ca14-123">Basic</span><span class="sxs-lookup"><span data-stu-id="5ca14-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_sort-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5ca14-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ca14-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_sort-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/resources/rangesort.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/resources/rangesort.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
