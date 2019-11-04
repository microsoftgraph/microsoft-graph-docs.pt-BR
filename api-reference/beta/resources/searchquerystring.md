---
title: tipo de recurso searchQueryString
description: searchQueryString
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 93142dcc672c5fee18a5f98d0988352e6c02cbd0
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935062"
---
# <a name="searchquerystring-resource-type"></a><span data-ttu-id="c44e7-103">tipo de recurso searchQueryString</span><span class="sxs-lookup"><span data-stu-id="c44e7-103">searchQueryString resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c44e7-104">Os termos de pesquisa da consulta.</span><span class="sxs-lookup"><span data-stu-id="c44e7-104">The search terms for the query.</span></span>

## <a name="properties"></a><span data-ttu-id="c44e7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c44e7-105">Properties</span></span>

| <span data-ttu-id="c44e7-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c44e7-106">Property</span></span>     | <span data-ttu-id="c44e7-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c44e7-107">Type</span></span>        | <span data-ttu-id="c44e7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c44e7-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c44e7-109">consulta</span><span class="sxs-lookup"><span data-stu-id="c44e7-109">query</span></span>|<span data-ttu-id="c44e7-110">String</span><span class="sxs-lookup"><span data-stu-id="c44e7-110">String</span></span>|<span data-ttu-id="c44e7-111">Contém os termos de pesquisa reais da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c44e7-111">Contains the actual search terms of the request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c44e7-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c44e7-112">JSON representation</span></span>

<span data-ttu-id="c44e7-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c44e7-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQueryString",
  "baseType": null
}-->

```json
{
  "query": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchQueryString resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->