---
title: tipo de recurso searchAlteration
description: Fornece os detalhes da alteração de pesquisa para correção ortográfica.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5caab3a3fbd8f8487e6893c5f5f530cc8471bb80
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067885"
---
# <a name="searchalteration-resource-type"></a><span data-ttu-id="f1f8b-103">tipo de recurso searchAlteration</span><span class="sxs-lookup"><span data-stu-id="f1f8b-103">searchAlteration resource type</span></span>

<span data-ttu-id="f1f8b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1f8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1f8b-105">Fornece os detalhes da alteração de pesquisa para correção ortográfica.</span><span class="sxs-lookup"><span data-stu-id="f1f8b-105">Provides the details of search alteration for spelling correction.</span></span>

## <a name="properties"></a><span data-ttu-id="f1f8b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1f8b-106">Properties</span></span>

| <span data-ttu-id="f1f8b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1f8b-107">Property</span></span>     | <span data-ttu-id="f1f8b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1f8b-108">Type</span></span>        | <span data-ttu-id="f1f8b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1f8b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f1f8b-110">alteredQueryString</span><span class="sxs-lookup"><span data-stu-id="f1f8b-110">alteredQueryString</span></span>|<span data-ttu-id="f1f8b-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f8b-111">String</span></span>| <span data-ttu-id="f1f8b-112">Define a cadeia de caracteres de consulta alterada com correção ortográfica.</span><span class="sxs-lookup"><span data-stu-id="f1f8b-112">Defines the altered query string with spelling correction.</span></span>|
|<span data-ttu-id="f1f8b-113">alteredHighlightedQueryString</span><span class="sxs-lookup"><span data-stu-id="f1f8b-113">alteredHighlightedQueryString</span></span>|<span data-ttu-id="f1f8b-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f8b-114">String</span></span>| <span data-ttu-id="f1f8b-115">Define a cadeia de caracteres de consulta realçada alterada com correção ortográfica.</span><span class="sxs-lookup"><span data-stu-id="f1f8b-115">Defines the altered highlighted query string with spelling correction.</span></span> <span data-ttu-id="f1f8b-116">A anotação em torno do segmento corrigido é (\ue000, \ue001)</span><span class="sxs-lookup"><span data-stu-id="f1f8b-116">The annotation around the corrected segment is (\ue000, \ue001)</span></span>|
|<span data-ttu-id="f1f8b-117">alteredQueryTokens</span><span class="sxs-lookup"><span data-stu-id="f1f8b-117">alteredQueryTokens</span></span>|<span data-ttu-id="f1f8b-118">[Coleção alteredQueryToken](alteredquerytoken.md)</span><span class="sxs-lookup"><span data-stu-id="f1f8b-118">[alteredQueryToken](alteredquerytoken.md) collection</span></span>| <span data-ttu-id="f1f8b-119">Representa segmentos alterados em relação à consulta original.</span><span class="sxs-lookup"><span data-stu-id="f1f8b-119">Represents changed segments with respect to original query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1f8b-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1f8b-120">JSON representation</span></span>

<span data-ttu-id="f1f8b-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1f8b-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAlteration",
  "baseType": null
}-->

```json
{
  "alteredQueryString": "String",
  "alteredHighlightedQueryString": "String",
  "alteredQueryTokens": [{"@odata.type": "microsoft.graph.alteredQueryToken"}]
}
```