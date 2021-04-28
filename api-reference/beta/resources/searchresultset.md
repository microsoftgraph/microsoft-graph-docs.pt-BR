---
title: Tipo de recurso searchResultSet
description: Descrição da pesquisaResultSet
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5d17791a618f1d587520f23524da9ce19241d3b1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067802"
---
# <a name="searchresultset-resource-type"></a><span data-ttu-id="962a0-103">Tipo de recurso searchResultSet</span><span class="sxs-lookup"><span data-stu-id="962a0-103">searchResultSet resource type</span></span>

<span data-ttu-id="962a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="962a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="962a0-105">Representa os resultados de uma consulta de pesquisa e os termos usados para a consulta.</span><span class="sxs-lookup"><span data-stu-id="962a0-105">Represents results from a search query, and the terms used for the query.</span></span> 

## <a name="properties"></a><span data-ttu-id="962a0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="962a0-106">Properties</span></span>

| <span data-ttu-id="962a0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="962a0-107">Property</span></span>     | <span data-ttu-id="962a0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="962a0-108">Type</span></span>        | <span data-ttu-id="962a0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="962a0-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="962a0-110">hitsContainers</span><span class="sxs-lookup"><span data-stu-id="962a0-110">hitsContainers</span></span>|<span data-ttu-id="962a0-111">[coleção searchHitsContainer](searchhitscontainer.md)</span><span class="sxs-lookup"><span data-stu-id="962a0-111">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="962a0-112">Uma coleção de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="962a0-112">A collection of search results.</span></span>|
|<span data-ttu-id="962a0-113">searchTerms</span><span class="sxs-lookup"><span data-stu-id="962a0-113">searchTerms</span></span>|<span data-ttu-id="962a0-114">Coleção String</span><span class="sxs-lookup"><span data-stu-id="962a0-114">String collection</span></span>|<span data-ttu-id="962a0-115">Contém os termos de pesquisa enviados na consulta de pesquisa inicial.</span><span class="sxs-lookup"><span data-stu-id="962a0-115">Contains the search terms sent in the initial search query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="962a0-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="962a0-116">JSON representation</span></span>

<span data-ttu-id="962a0-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="962a0-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResultSet",
  "baseType": null
}-->

```json
{
  "hitsContainers": [{"@odata.type": "microsoft.graph.searchHitsContainer"}],
  "searchTerms": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchResultSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

