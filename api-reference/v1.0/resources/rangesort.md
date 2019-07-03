---
title: Tipo de recurso RangeSort
description: Gerencia operações de classificação em objetos Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fb7f99cc1d7dbdf3ecb81de6bd3e08f87b329642
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460872"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="fc5d6-103">Tipo de recurso RangeSort</span><span class="sxs-lookup"><span data-stu-id="fc5d6-103">RangeSort resource type</span></span>

<span data-ttu-id="fc5d6-104">Gerencia operações de classificação em objetos Range.</span><span class="sxs-lookup"><span data-stu-id="fc5d6-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="fc5d6-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="fc5d6-105">Methods</span></span>

| <span data-ttu-id="fc5d6-106">Método</span><span class="sxs-lookup"><span data-stu-id="fc5d6-106">Method</span></span>           | <span data-ttu-id="fc5d6-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fc5d6-107">Return Type</span></span>    |<span data-ttu-id="fc5d6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc5d6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fc5d6-109">Apply</span><span class="sxs-lookup"><span data-stu-id="fc5d6-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="fc5d6-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc5d6-110">None</span></span>|<span data-ttu-id="fc5d6-111">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="fc5d6-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="fc5d6-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc5d6-112">Properties</span></span>
<span data-ttu-id="fc5d6-113">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="fc5d6-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="fc5d6-114">Relações</span><span class="sxs-lookup"><span data-stu-id="fc5d6-114">Relationships</span></span>
<span data-ttu-id="fc5d6-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc5d6-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc5d6-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc5d6-116">JSON representation</span></span>

<span data-ttu-id="fc5d6-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc5d6-117">Here is a JSON representation of the resource.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fc5d6-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc5d6-118">HTTP</span></span>](#tab/http)
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

##### <a name="request"></a><span data-ttu-id="fc5d6-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc5d6-119">Request</span></span>
<span data-ttu-id="fc5d6-120">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc5d6-120">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fc5d6-121">C#</span><span class="sxs-lookup"><span data-stu-id="fc5d6-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-sort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc5d6-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="fc5d6-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-sort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fc5d6-123">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fc5d6-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-sort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fc5d6-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc5d6-124">Response</span></span>
<span data-ttu-id="fc5d6-125">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc5d6-125">Here is an example of the response.</span></span> 
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
