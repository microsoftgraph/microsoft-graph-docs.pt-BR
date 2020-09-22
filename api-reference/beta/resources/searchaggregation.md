---
title: tipo de recurso searchAggregation
description: Fornece os detalhes da agregação de pesquisa na resposta de pesquisa.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 480a6f70a2815a174697ff22fc217057053e1f4b
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193828"
---
# <a name="searchaggregation-resource-type"></a><span data-ttu-id="5a8e1-103">tipo de recurso searchAggregation</span><span class="sxs-lookup"><span data-stu-id="5a8e1-103">searchAggregation resource type</span></span>

<span data-ttu-id="5a8e1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a8e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a8e1-105">Fornece os detalhes da agregação de pesquisa na resposta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="5a8e1-105">Provides the details of the search aggregation in the search response.</span></span>

## <a name="properties"></a><span data-ttu-id="5a8e1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a8e1-106">Properties</span></span>

| <span data-ttu-id="5a8e1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a8e1-107">Property</span></span>     | <span data-ttu-id="5a8e1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a8e1-108">Type</span></span>        | <span data-ttu-id="5a8e1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a8e1-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5a8e1-110">displayName</span><span class="sxs-lookup"><span data-stu-id="5a8e1-110">displayName</span></span>|<span data-ttu-id="5a8e1-111">String</span><span class="sxs-lookup"><span data-stu-id="5a8e1-111">String</span></span>| <span data-ttu-id="5a8e1-112">O nome amigável da agregação.</span><span class="sxs-lookup"><span data-stu-id="5a8e1-112">The friendly name of the aggregation.</span></span> <span data-ttu-id="5a8e1-113">Esse valor foi fornecido na entrada.</span><span class="sxs-lookup"><span data-stu-id="5a8e1-113">This value was provided in the input.</span></span>|
|<span data-ttu-id="5a8e1-114">campo</span><span class="sxs-lookup"><span data-stu-id="5a8e1-114">field</span></span>|<span data-ttu-id="5a8e1-115">String</span><span class="sxs-lookup"><span data-stu-id="5a8e1-115">String</span></span>| <span data-ttu-id="5a8e1-116">Define em qual campo a agregação foi calculada.</span><span class="sxs-lookup"><span data-stu-id="5a8e1-116">Defines on which field the aggregation was computed on.</span></span>|
|<span data-ttu-id="5a8e1-117">buckets</span><span class="sxs-lookup"><span data-stu-id="5a8e1-117">buckets</span></span>|<span data-ttu-id="5a8e1-118">coleção [searchBucket](searchbucket.md)</span><span class="sxs-lookup"><span data-stu-id="5a8e1-118">[searchBucket](searchbucket.md) collection</span></span>| <span data-ttu-id="5a8e1-119">Define os buckets reais da agregação calculada.</span><span class="sxs-lookup"><span data-stu-id="5a8e1-119">Defines the actual buckets of the computed aggregation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a8e1-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a8e1-120">JSON representation</span></span>

<span data-ttu-id="5a8e1-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a8e1-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAggregation",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "field": "String",  
  "buckets": [{"@odata.type": "microsoft.graph.searchBucket"}]
}
```