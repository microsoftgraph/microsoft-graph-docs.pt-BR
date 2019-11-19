---
title: tipo de recurso searchQueryString
description: searchQueryString
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 59809860bd2d0954ee8323f9c8e4fe982fb4faa7
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703823"
---
# <a name="searchquerystring-resource-type"></a><span data-ttu-id="f1250-103">tipo de recurso searchQueryString</span><span class="sxs-lookup"><span data-stu-id="f1250-103">searchQueryString resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1250-104">Os termos de pesquisa da consulta.</span><span class="sxs-lookup"><span data-stu-id="f1250-104">The search terms for the query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="f1250-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1250-105">Properties</span></span>

| <span data-ttu-id="f1250-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1250-106">Property</span></span>     | <span data-ttu-id="f1250-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1250-107">Type</span></span>        | <span data-ttu-id="f1250-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1250-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f1250-109">consulta</span><span class="sxs-lookup"><span data-stu-id="f1250-109">query</span></span>|<span data-ttu-id="f1250-110">String</span><span class="sxs-lookup"><span data-stu-id="f1250-110">String</span></span>|<span data-ttu-id="f1250-111">Contém os termos de pesquisa reais da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1250-111">Contains the actual search terms of the request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1250-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1250-112">JSON representation</span></span>

<span data-ttu-id="f1250-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1250-113">The following is a JSON representation of the resource.</span></span>

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