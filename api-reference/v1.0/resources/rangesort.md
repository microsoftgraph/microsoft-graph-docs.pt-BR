---
title: Tipo de recurso RangeSort
description: Gerencia operações de classificação em objetos Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f4b5ffac155542615d17db0f6e511cf77c72cc82
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36730306"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="f585e-103">Tipo de recurso RangeSort</span><span class="sxs-lookup"><span data-stu-id="f585e-103">RangeSort resource type</span></span>

<span data-ttu-id="f585e-104">Gerencia operações de classificação em objetos Range.</span><span class="sxs-lookup"><span data-stu-id="f585e-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="f585e-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f585e-105">Methods</span></span>

| <span data-ttu-id="f585e-106">Método</span><span class="sxs-lookup"><span data-stu-id="f585e-106">Method</span></span>           | <span data-ttu-id="f585e-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f585e-107">Return Type</span></span>    |<span data-ttu-id="f585e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f585e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f585e-109">Apply</span><span class="sxs-lookup"><span data-stu-id="f585e-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="f585e-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f585e-110">None</span></span>|<span data-ttu-id="f585e-111">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="f585e-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="f585e-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f585e-112">Properties</span></span>
<span data-ttu-id="f585e-113">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f585e-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="f585e-114">Relações</span><span class="sxs-lookup"><span data-stu-id="f585e-114">Relationships</span></span>
<span data-ttu-id="f585e-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f585e-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f585e-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f585e-116">JSON representation</span></span>

<span data-ttu-id="f585e-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f585e-117">Here is a JSON representation of the resource.</span></span>


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

##### <a name="request"></a><span data-ttu-id="f585e-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f585e-118">Request</span></span>
<span data-ttu-id="f585e-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f585e-119">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f585e-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="f585e-120">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f585e-121">C#</span><span class="sxs-lookup"><span data-stu-id="f585e-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-sort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f585e-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f585e-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-sort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f585e-123">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f585e-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-sort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f585e-124">Java</span><span class="sxs-lookup"><span data-stu-id="f585e-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-sort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f585e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f585e-125">Response</span></span>
<span data-ttu-id="f585e-126">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f585e-126">Here is an example of the response.</span></span> 
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
