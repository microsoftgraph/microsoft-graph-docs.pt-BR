---
title: Tipo de recurso searchResponse
description: Descrição da pesquisaResponse
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5778d82c0c4718b9f34c686a613270eebfcc56e1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067086"
---
# <a name="searchresponse-resource-type"></a><span data-ttu-id="0c867-103">Tipo de recurso searchResponse</span><span class="sxs-lookup"><span data-stu-id="0c867-103">searchResponse resource type</span></span>

<span data-ttu-id="0c867-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c867-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c867-105">Representa a resposta de uma consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="0c867-105">Represents the response from a search query.</span></span> 

## <a name="properties"></a><span data-ttu-id="0c867-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c867-106">Properties</span></span>

| <span data-ttu-id="0c867-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c867-107">Property</span></span>     | <span data-ttu-id="0c867-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c867-108">Type</span></span>        | <span data-ttu-id="0c867-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c867-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0c867-110">queryAlterationResponse</span><span class="sxs-lookup"><span data-stu-id="0c867-110">queryAlterationResponse</span></span>|[<span data-ttu-id="0c867-111">alterationResponse</span><span class="sxs-lookup"><span data-stu-id="0c867-111">alterationResponse</span></span>](alterationResponse.md)|<span data-ttu-id="0c867-112">Fornece detalhes da resposta de alteração de consulta para correção ortográfica.</span><span class="sxs-lookup"><span data-stu-id="0c867-112">Provides details of query alteration response for spelling correction.</span></span>|
|<span data-ttu-id="0c867-113">valor</span><span class="sxs-lookup"><span data-stu-id="0c867-113">value</span></span>|<span data-ttu-id="0c867-114">[Coleção searchResultSet](searchResultSet.md)</span><span class="sxs-lookup"><span data-stu-id="0c867-114">[searchResultSet](searchResultSet.md) collection</span></span>|<span data-ttu-id="0c867-115">Representa os resultados de uma consulta de pesquisa e os termos usados para a consulta.</span><span class="sxs-lookup"><span data-stu-id="0c867-115">Represents results from a search query, and the terms used for the query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c867-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c867-116">JSON representation</span></span>

<span data-ttu-id="0c867-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c867-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResponse",
  "baseType": null
}-->

```json
{
  "queryAlterationResponse": {"@odata.type": "microsoft.graph.alterationResponse"},
  "value": [{"@odata.type": "microsoft.graph.searchResultSet"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

