---
title: Tipo de recurso RangeSort
description: Gerencia operações de classificação em objetos Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6d1fb0be3feae69ff2cae34f360a0f78d46a6172
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579505"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="907a9-103">Tipo de recurso RangeSort</span><span class="sxs-lookup"><span data-stu-id="907a9-103">RangeSort resource type</span></span>

<span data-ttu-id="907a9-104">Gerencia operações de classificação em objetos Range.</span><span class="sxs-lookup"><span data-stu-id="907a9-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="907a9-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="907a9-105">Methods</span></span>

| <span data-ttu-id="907a9-106">Método</span><span class="sxs-lookup"><span data-stu-id="907a9-106">Method</span></span>           | <span data-ttu-id="907a9-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="907a9-107">Return Type</span></span>    |<span data-ttu-id="907a9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="907a9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="907a9-109">Apply</span><span class="sxs-lookup"><span data-stu-id="907a9-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="907a9-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="907a9-110">None</span></span>|<span data-ttu-id="907a9-111">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="907a9-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="907a9-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="907a9-112">Properties</span></span>
<span data-ttu-id="907a9-113">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="907a9-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="907a9-114">Relações</span><span class="sxs-lookup"><span data-stu-id="907a9-114">Relationships</span></span>
<span data-ttu-id="907a9-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="907a9-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="907a9-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="907a9-116">JSON representation</span></span>

<span data-ttu-id="907a9-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="907a9-117">Here is a JSON representation of the resource.</span></span>

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

##### <a name="request"></a><span data-ttu-id="907a9-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="907a9-118">Request</span></span>
<span data-ttu-id="907a9-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="907a9-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="907a9-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="907a9-120">Response</span></span>
<span data-ttu-id="907a9-121">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="907a9-121">Here is an example of the response.</span></span> 
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
