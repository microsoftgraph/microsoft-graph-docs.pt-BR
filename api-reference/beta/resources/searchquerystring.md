---
title: tipo de recurso searchQueryString
description: searchQueryString
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b273d9ec15b949019b780dd5ce9f1a6184191763
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520903"
---
# <a name="searchquerystring-resource-type"></a><span data-ttu-id="47653-103">tipo de recurso searchQueryString</span><span class="sxs-lookup"><span data-stu-id="47653-103">searchQueryString resource type</span></span>

<span data-ttu-id="47653-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="47653-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47653-105">Os termos de pesquisa da consulta.</span><span class="sxs-lookup"><span data-stu-id="47653-105">The search terms for the query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="47653-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47653-106">Properties</span></span>

| <span data-ttu-id="47653-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47653-107">Property</span></span>     | <span data-ttu-id="47653-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="47653-108">Type</span></span>        | <span data-ttu-id="47653-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="47653-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="47653-110">consulta</span><span class="sxs-lookup"><span data-stu-id="47653-110">query</span></span>|<span data-ttu-id="47653-111">String</span><span class="sxs-lookup"><span data-stu-id="47653-111">String</span></span>|<span data-ttu-id="47653-112">Contém os termos de pesquisa reais da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47653-112">Contains the actual search terms of the request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47653-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47653-113">JSON representation</span></span>

<span data-ttu-id="47653-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47653-114">The following is a JSON representation of the resource.</span></span>

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