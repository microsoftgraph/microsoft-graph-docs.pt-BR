---
title: tipo de recurso searchResponse
description: Descrição do searchResponse
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: deb5450017b4ae9db534c30f71dd6da4f1a9b812
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192746"
---
# <a name="searchresponse-resource-type"></a><span data-ttu-id="62c59-103">tipo de recurso searchResponse</span><span class="sxs-lookup"><span data-stu-id="62c59-103">searchResponse resource type</span></span>

<span data-ttu-id="62c59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62c59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62c59-105">Representa os resultados de uma consulta de pesquisa e os termos usados para a consulta.</span><span class="sxs-lookup"><span data-stu-id="62c59-105">Represents results from a search query, and the terms used for the query.</span></span> 

## <a name="properties"></a><span data-ttu-id="62c59-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62c59-106">Properties</span></span>

| <span data-ttu-id="62c59-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62c59-107">Property</span></span>     | <span data-ttu-id="62c59-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="62c59-108">Type</span></span>        | <span data-ttu-id="62c59-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="62c59-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="62c59-110">hitsContainers</span><span class="sxs-lookup"><span data-stu-id="62c59-110">hitsContainers</span></span>|<span data-ttu-id="62c59-111">coleção [searchHitsContainer](searchhitscontainer.md)</span><span class="sxs-lookup"><span data-stu-id="62c59-111">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="62c59-112">Uma coleção de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="62c59-112">A collection of search results.</span></span>|
|<span data-ttu-id="62c59-113">searchTerms</span><span class="sxs-lookup"><span data-stu-id="62c59-113">searchTerms</span></span>|<span data-ttu-id="62c59-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="62c59-114">String collection</span></span>|<span data-ttu-id="62c59-115">Contém os termos de pesquisa enviados na consulta de pesquisa inicial.</span><span class="sxs-lookup"><span data-stu-id="62c59-115">Contains the search terms sent in the initial search query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62c59-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62c59-116">JSON representation</span></span>

<span data-ttu-id="62c59-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62c59-117">The following is a JSON representation of the resource.</span></span>

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

