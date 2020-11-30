---
title: tipo de recurso searchResponse
description: Descrição do searchResponse
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8582da8daf604952807e05376d98dabf16267052
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377772"
---
# <a name="searchresponse-resource-type"></a><span data-ttu-id="69672-103">tipo de recurso searchResponse</span><span class="sxs-lookup"><span data-stu-id="69672-103">searchResponse resource type</span></span>

<span data-ttu-id="69672-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69672-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69672-105">Representa os resultados de uma consulta de pesquisa e os termos usados para a consulta.</span><span class="sxs-lookup"><span data-stu-id="69672-105">Represents results from a search query, and the terms used for the query.</span></span> 

## <a name="properties"></a><span data-ttu-id="69672-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69672-106">Properties</span></span>

| <span data-ttu-id="69672-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69672-107">Property</span></span>     | <span data-ttu-id="69672-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="69672-108">Type</span></span>        | <span data-ttu-id="69672-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="69672-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="69672-110">hitsContainers</span><span class="sxs-lookup"><span data-stu-id="69672-110">hitsContainers</span></span>|<span data-ttu-id="69672-111">coleção [searchHitsContainer](searchhitscontainer.md)</span><span class="sxs-lookup"><span data-stu-id="69672-111">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="69672-112">Uma coleção de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="69672-112">A collection of search results.</span></span>|
|<span data-ttu-id="69672-113">searchTerms</span><span class="sxs-lookup"><span data-stu-id="69672-113">searchTerms</span></span>|<span data-ttu-id="69672-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="69672-114">String collection</span></span>|<span data-ttu-id="69672-115">Contém os termos de pesquisa enviados na consulta de pesquisa inicial.</span><span class="sxs-lookup"><span data-stu-id="69672-115">Contains the search terms sent in the initial search query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69672-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69672-116">JSON representation</span></span>

<span data-ttu-id="69672-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69672-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResponse",
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
  "description": "searchResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

