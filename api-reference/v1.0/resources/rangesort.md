---
title: Tipo de recurso RangeSort
description: Gerencia as operações de classificação em objetos Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6d1fb0be3feae69ff2cae34f360a0f78d46a6172
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947572"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="e229a-103">Tipo de recurso RangeSort</span><span class="sxs-lookup"><span data-stu-id="e229a-103">RangeSort resource type</span></span>

<span data-ttu-id="e229a-104">Gerencia as operações de classificação em objetos Range.</span><span class="sxs-lookup"><span data-stu-id="e229a-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="e229a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="e229a-105">Methods</span></span>

| <span data-ttu-id="e229a-106">Método</span><span class="sxs-lookup"><span data-stu-id="e229a-106">Method</span></span>           | <span data-ttu-id="e229a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e229a-107">Return Type</span></span>    |<span data-ttu-id="e229a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e229a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e229a-109">Aplicar</span><span class="sxs-lookup"><span data-stu-id="e229a-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="e229a-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e229a-110">None</span></span>|<span data-ttu-id="e229a-111">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="e229a-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="e229a-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e229a-112">Properties</span></span>
<span data-ttu-id="e229a-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e229a-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e229a-114">Relações</span><span class="sxs-lookup"><span data-stu-id="e229a-114">Relationships</span></span>
<span data-ttu-id="e229a-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e229a-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e229a-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e229a-116">JSON representation</span></span>

<span data-ttu-id="e229a-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e229a-117">Here is a JSON representation of the resource.</span></span>

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

##### <a name="request"></a><span data-ttu-id="e229a-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e229a-118">Request</span></span>
<span data-ttu-id="e229a-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e229a-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="e229a-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="e229a-120">Response</span></span>
<span data-ttu-id="e229a-121">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e229a-121">Here is an example of the response.</span></span> 
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
