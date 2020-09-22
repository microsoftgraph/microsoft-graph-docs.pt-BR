---
title: Tipo de recurso RangeSort
description: Gerencia operações de classificação em objetos Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 4964162d6c3380f3dcbe12ef0ed6ce0009149bb3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028249"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="18755-103">Tipo de recurso RangeSort</span><span class="sxs-lookup"><span data-stu-id="18755-103">RangeSort resource type</span></span>

<span data-ttu-id="18755-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18755-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18755-105">Gerencia operações de classificação em objetos Range.</span><span class="sxs-lookup"><span data-stu-id="18755-105">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="18755-106">Methods</span><span class="sxs-lookup"><span data-stu-id="18755-106">Methods</span></span>

| <span data-ttu-id="18755-107">Método</span><span class="sxs-lookup"><span data-stu-id="18755-107">Method</span></span>           | <span data-ttu-id="18755-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="18755-108">Return Type</span></span>    |<span data-ttu-id="18755-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="18755-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="18755-110">Apply</span><span class="sxs-lookup"><span data-stu-id="18755-110">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="18755-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18755-111">None</span></span>|<span data-ttu-id="18755-112">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="18755-112">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="18755-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18755-113">Properties</span></span>
<span data-ttu-id="18755-114">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="18755-114">None</span></span>

## <a name="relationships"></a><span data-ttu-id="18755-115">Relações</span><span class="sxs-lookup"><span data-stu-id="18755-115">Relationships</span></span>
<span data-ttu-id="18755-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18755-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18755-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18755-117">JSON representation</span></span>

<span data-ttu-id="18755-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18755-118">Here is a JSON representation of the resource.</span></span>


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

##### <a name="request"></a><span data-ttu-id="18755-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18755-119">Request</span></span>
<span data-ttu-id="18755-120">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18755-120">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="18755-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="18755-121">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```
# <a name="c"></a>[<span data-ttu-id="18755-122">C#</span><span class="sxs-lookup"><span data-stu-id="18755-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-sort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18755-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18755-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-sort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18755-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18755-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-sort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18755-125">Java</span><span class="sxs-lookup"><span data-stu-id="18755-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-sort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="18755-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="18755-126">Response</span></span>
<span data-ttu-id="18755-127">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18755-127">Here is an example of the response.</span></span> 
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

