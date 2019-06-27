---
title: Tipo de recurso RangeSort
description: Gerencia operações de classificação em objetos Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8f917cb2fa7c8ade81fef2d713e368cc43ab40b3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275142"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="711bd-103">Tipo de recurso RangeSort</span><span class="sxs-lookup"><span data-stu-id="711bd-103">RangeSort resource type</span></span>

<span data-ttu-id="711bd-104">Gerencia operações de classificação em objetos Range.</span><span class="sxs-lookup"><span data-stu-id="711bd-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="711bd-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="711bd-105">Methods</span></span>

| <span data-ttu-id="711bd-106">Método</span><span class="sxs-lookup"><span data-stu-id="711bd-106">Method</span></span>           | <span data-ttu-id="711bd-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="711bd-107">Return Type</span></span>    |<span data-ttu-id="711bd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="711bd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="711bd-109">Apply</span><span class="sxs-lookup"><span data-stu-id="711bd-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="711bd-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="711bd-110">None</span></span>|<span data-ttu-id="711bd-111">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="711bd-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="711bd-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="711bd-112">Properties</span></span>
<span data-ttu-id="711bd-113">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="711bd-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="711bd-114">Relações</span><span class="sxs-lookup"><span data-stu-id="711bd-114">Relationships</span></span>
<span data-ttu-id="711bd-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="711bd-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="711bd-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="711bd-116">JSON representation</span></span>

<span data-ttu-id="711bd-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="711bd-117">Here is a JSON representation of the resource.</span></span>

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

##### <a name="request"></a><span data-ttu-id="711bd-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="711bd-118">Request</span></span>
<span data-ttu-id="711bd-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="711bd-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="711bd-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="711bd-120">Response</span></span>
<span data-ttu-id="711bd-121">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="711bd-121">Here is an example of the response.</span></span> 
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="711bd-122">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="711bd-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="711bd-123">C#</span><span class="sxs-lookup"><span data-stu-id="711bd-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_sort-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="711bd-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="711bd-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_sort-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="711bd-125">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="711bd-125">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/range_sort-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/resources/rangesort.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/resources/rangesort.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/resources/rangesort.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
