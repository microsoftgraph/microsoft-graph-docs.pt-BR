---
title: tipo de recurso searchAlterationOptions
description: Fornece as opções de alteração de pesquisa para correção ortográfica.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: dc17698715b4ea6e894ae13f1999e78ab361cc5e
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067886"
---
# <a name="searchalterationoptions-resource-type"></a><span data-ttu-id="1d40b-103">tipo de recurso searchAlterationOptions</span><span class="sxs-lookup"><span data-stu-id="1d40b-103">searchAlterationOptions resource type</span></span>

<span data-ttu-id="1d40b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d40b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d40b-105">Fornece as opções de alteração de pesquisa para correção ortográfica.</span><span class="sxs-lookup"><span data-stu-id="1d40b-105">Provides the search alteration options for spelling correction.</span></span>

## <a name="properties"></a><span data-ttu-id="1d40b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d40b-106">Properties</span></span>

| <span data-ttu-id="1d40b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d40b-107">Property</span></span>     | <span data-ttu-id="1d40b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d40b-108">Type</span></span>        | <span data-ttu-id="1d40b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d40b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1d40b-110">enableSuggestion</span><span class="sxs-lookup"><span data-stu-id="1d40b-110">enableSuggestion</span></span>|<span data-ttu-id="1d40b-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d40b-111">Boolean</span></span>|<span data-ttu-id="1d40b-112">Indica se as sugestões ortográficas estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="1d40b-112">Indicates whether spelling suggestions are enabled.</span></span> <span data-ttu-id="1d40b-113">Se habilitado, o usuário receberá os resultados da pesquisa para consulta de pesquisa original e [](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true) sugerirá correção ortográfica na **propriedade queryAlterationResponse** da resposta para erros de digitação na consulta.</span><span class="sxs-lookup"><span data-stu-id="1d40b-113">If enabled, user will get the search results for original search query and suggesting spelling correction in **queryAlterationResponse** property of the [response](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true) for typos in query.</span></span> <span data-ttu-id="1d40b-114">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1d40b-114">Optional.</span></span>|
|<span data-ttu-id="1d40b-115">enableModification</span><span class="sxs-lookup"><span data-stu-id="1d40b-115">enableModification</span></span>|<span data-ttu-id="1d40b-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d40b-116">Boolean</span></span>|<span data-ttu-id="1d40b-117">Indica se as modificações ortográficas estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="1d40b-117">Indicates whether spelling modifications are enabled.</span></span> <span data-ttu-id="1d40b-118">Se habilitado, o usuário receberá os resultados  da pesquisa para consulta corrigida quando não houver resultados para a consulta original com erros de digitação e obterá as informações de modificação ortográfica na propriedade **queryAlterationResponse** da resposta [.](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="1d40b-118">If enabled, user will get the search results for corrected query **when there are no results** for the original query with typos and get the spelling modification information in **queryAlterationResponse** property of the [response](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="1d40b-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1d40b-119">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d40b-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d40b-120">JSON representation</span></span>

<span data-ttu-id="1d40b-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d40b-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAlterationOptions",
  "baseType": null
}-->

```json
{
  "enableSuggestion": true,
  "enableModification": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchAlterationOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
