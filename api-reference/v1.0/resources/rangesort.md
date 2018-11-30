---
title: Tipo de recurso RangeSort
description: Gerencia as operações de classificação em objetos Range.
ms.openlocfilehash: 09f9a6763c634ee12251651a650d29528a534084
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004440"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="7b301-103">Tipo de recurso RangeSort</span><span class="sxs-lookup"><span data-stu-id="7b301-103">RangeSort resource type</span></span>

<span data-ttu-id="7b301-104">Gerencia as operações de classificação em objetos Range.</span><span class="sxs-lookup"><span data-stu-id="7b301-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="7b301-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="7b301-105">Methods</span></span>

| <span data-ttu-id="7b301-106">Método</span><span class="sxs-lookup"><span data-stu-id="7b301-106">Method</span></span>           | <span data-ttu-id="7b301-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7b301-107">Return Type</span></span>    |<span data-ttu-id="7b301-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b301-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7b301-109">Aplicar</span><span class="sxs-lookup"><span data-stu-id="7b301-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="7b301-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b301-110">None</span></span>|<span data-ttu-id="7b301-111">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="7b301-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b301-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b301-112">Properties</span></span>
<span data-ttu-id="7b301-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b301-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="7b301-114">Relações</span><span class="sxs-lookup"><span data-stu-id="7b301-114">Relationships</span></span>
<span data-ttu-id="7b301-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b301-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b301-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b301-116">JSON representation</span></span>

<span data-ttu-id="7b301-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b301-117">Here is a JSON representation of the resource.</span></span>

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

##### <a name="request"></a><span data-ttu-id="7b301-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b301-118">Request</span></span>
<span data-ttu-id="7b301-119">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b301-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="7b301-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b301-120">Response</span></span>
<span data-ttu-id="7b301-121">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b301-121">Here is an example of the response.</span></span> 
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