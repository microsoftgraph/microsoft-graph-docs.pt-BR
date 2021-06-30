---
title: Tipo de recurso searchResultSet
description: Descrição da pesquisaResultSet
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: ee5ac6d892b6562ca5c1053b474135f1dd745ba5
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210203"
---
# <a name="searchresultset-resource-type"></a><span data-ttu-id="a94e9-103">Tipo de recurso searchResultSet</span><span class="sxs-lookup"><span data-stu-id="a94e9-103">searchResultSet resource type</span></span>

<span data-ttu-id="a94e9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a94e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a94e9-105">Representa os resultados de uma consulta de pesquisa e os termos usados para a consulta.</span><span class="sxs-lookup"><span data-stu-id="a94e9-105">Represents results from a search query, and the terms used for the query.</span></span> 

## <a name="properties"></a><span data-ttu-id="a94e9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a94e9-106">Properties</span></span>

| <span data-ttu-id="a94e9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a94e9-107">Property</span></span>     | <span data-ttu-id="a94e9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a94e9-108">Type</span></span>        | <span data-ttu-id="a94e9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a94e9-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a94e9-110">hitsContainers</span><span class="sxs-lookup"><span data-stu-id="a94e9-110">hitsContainers</span></span>|<span data-ttu-id="a94e9-111">[coleção searchHitsContainer](searchhitscontainer.md)</span><span class="sxs-lookup"><span data-stu-id="a94e9-111">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="a94e9-112">Uma coleção de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a94e9-112">A collection of search results.</span></span>|
|<span data-ttu-id="a94e9-113">searchTerms</span><span class="sxs-lookup"><span data-stu-id="a94e9-113">searchTerms</span></span>|<span data-ttu-id="a94e9-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a94e9-114">String collection</span></span>|<span data-ttu-id="a94e9-115">Contém os termos de pesquisa enviados na consulta de pesquisa inicial.</span><span class="sxs-lookup"><span data-stu-id="a94e9-115">Contains the search terms sent in the initial search query.</span></span>|
|<span data-ttu-id="a94e9-116">resultTemplates</span><span class="sxs-lookup"><span data-stu-id="a94e9-116">resultTemplates</span></span>|<span data-ttu-id="a94e9-117">[coleção resultTemplate](resultTemplate.md)</span><span class="sxs-lookup"><span data-stu-id="a94e9-117">[resultTemplate](resultTemplate.md) collection</span></span>|<span data-ttu-id="a94e9-118">Um dicionário de resultTemplateIds e valores associados, que incluem o nome e o esquema JSON dos modelos de resultado.</span><span class="sxs-lookup"><span data-stu-id="a94e9-118">A dictionary of resultTemplateIds and associated values, which include the name and JSON schema of the result templates.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a94e9-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a94e9-119">JSON representation</span></span>

<span data-ttu-id="a94e9-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a94e9-120">The following is a JSON representation of the resource.</span></span>

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
  "searchTerms": ["String"],
  "resultTemplates": [{"@odata.type":"microsoft.graph.resultTemplateDictionary"}]
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

