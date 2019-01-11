---
title: Tipo de recurso RangeSort
description: Gerencia as operações de classificação em objetos Range.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: c52b4c6cc50bce7d518d26798db9f3d3da49cd1c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816422"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="827b3-103">Tipo de recurso RangeSort</span><span class="sxs-lookup"><span data-stu-id="827b3-103">RangeSort resource type</span></span>

<span data-ttu-id="827b3-104">Gerencia as operações de classificação em objetos Range.</span><span class="sxs-lookup"><span data-stu-id="827b3-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="827b3-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="827b3-105">Methods</span></span>

| <span data-ttu-id="827b3-106">Método</span><span class="sxs-lookup"><span data-stu-id="827b3-106">Method</span></span>           | <span data-ttu-id="827b3-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="827b3-107">Return Type</span></span>    |<span data-ttu-id="827b3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="827b3-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="827b3-109">Aplicar</span><span class="sxs-lookup"><span data-stu-id="827b3-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="827b3-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="827b3-110">None</span></span>|<span data-ttu-id="827b3-111">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="827b3-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="827b3-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="827b3-112">Properties</span></span>
<span data-ttu-id="827b3-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="827b3-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="827b3-114">Relações</span><span class="sxs-lookup"><span data-stu-id="827b3-114">Relationships</span></span>
<span data-ttu-id="827b3-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="827b3-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="827b3-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="827b3-116">JSON representation</span></span>

<span data-ttu-id="827b3-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="827b3-117">Here is a JSON representation of the resource.</span></span>

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

##### <a name="request"></a><span data-ttu-id="827b3-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="827b3-118">Request</span></span>
<span data-ttu-id="827b3-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="827b3-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="827b3-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="827b3-120">Response</span></span>
<span data-ttu-id="827b3-121">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="827b3-121">Here is an example of the response.</span></span> 
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
