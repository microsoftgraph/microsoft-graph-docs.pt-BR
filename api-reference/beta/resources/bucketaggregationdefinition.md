---
title: tipo de recurso bucketAggregationDefinition
description: Fornece os detalhes sobre como o agregations deve ser gerado nos resultados
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1f9fdadefc43b99b8772217db9a9b101357a1c9c
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193837"
---
# <a name="bucketaggregationdefinition-resource-type"></a><span data-ttu-id="b4bea-103">tipo de recurso bucketAggregationDefinition</span><span class="sxs-lookup"><span data-stu-id="b4bea-103">bucketAggregationDefinition resource type</span></span>

<span data-ttu-id="b4bea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4bea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4bea-105">Especifica detalhes para agregar resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="b4bea-105">Specifies details to aggregate search results.</span></span>

## <a name="properties"></a><span data-ttu-id="b4bea-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4bea-106">Properties</span></span>

| <span data-ttu-id="b4bea-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4bea-107">Property</span></span>     | <span data-ttu-id="b4bea-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4bea-108">Type</span></span>        | <span data-ttu-id="b4bea-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4bea-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b4bea-110">sortBy</span><span class="sxs-lookup"><span data-stu-id="b4bea-110">sortBy</span></span>|<span data-ttu-id="b4bea-111">bucketAggregationSortProperty</span><span class="sxs-lookup"><span data-stu-id="b4bea-111">bucketAggregationSortProperty</span></span>| <span data-ttu-id="b4bea-112">Os valores possíveis são `count` classificados pelo número de correspondências na agregação `keyAsString` para classificar o alphabeticaly com base na chave da agregação, `keyAsNumber` para a classificação numérica com base na chave da agregação.</span><span class="sxs-lookup"><span data-stu-id="b4bea-112">The possible values are `count` to sort by the number of matches in the aggregation, `keyAsString`to sort alphabeticaly based on the key in the aggregation, `keyAsNumber` for numerical sorting based on the key in the aggregation.</span></span> <span data-ttu-id="b4bea-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4bea-113">Required.</span></span>
|<span data-ttu-id="b4bea-114">isDescending</span><span class="sxs-lookup"><span data-stu-id="b4bea-114">isDescending</span></span>|<span data-ttu-id="b4bea-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="b4bea-115">Boolean</span></span>|<span data-ttu-id="b4bea-116">`True` para especificar a ordem de classificação como decrescente.</span><span class="sxs-lookup"><span data-stu-id="b4bea-116">`True` to specify the sort order as descending.</span></span> <span data-ttu-id="b4bea-117">O padrão é `false` , com a ordem de classificação como crescente.</span><span class="sxs-lookup"><span data-stu-id="b4bea-117">The default is `false`, with the sort order as ascending.</span></span> <span data-ttu-id="b4bea-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b4bea-118">Optional.</span></span>|
|<span data-ttu-id="b4bea-119">prefixFilter</span><span class="sxs-lookup"><span data-stu-id="b4bea-119">prefixFilter</span></span>|<span data-ttu-id="b4bea-120">String</span><span class="sxs-lookup"><span data-stu-id="b4bea-120">String</span></span>|<span data-ttu-id="b4bea-121">Um filtro para definir um critério de correspondência.</span><span class="sxs-lookup"><span data-stu-id="b4bea-121">A filter to define a matching criteria.</span></span> <span data-ttu-id="b4bea-122">A chave deve começar com o prefixo especificado a ser retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="b4bea-122">The key should start with the specified prefix to be returned in the response.</span></span> <span data-ttu-id="b4bea-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b4bea-123">Optional.</span></span>|
|<span data-ttu-id="b4bea-124">minimumCount</span><span class="sxs-lookup"><span data-stu-id="b4bea-124">minimumCount</span></span>|<span data-ttu-id="b4bea-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b4bea-125">Int32</span></span>|<span data-ttu-id="b4bea-126">O número mínimo de itens que devem estar presentes na agregação a serem retornados em um Bucket.</span><span class="sxs-lookup"><span data-stu-id="b4bea-126">The minimum number of items that should be present in the aggregation to be returned in a bucket.</span></span> <span data-ttu-id="b4bea-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b4bea-127">Optional.</span></span>|
|<span data-ttu-id="b4bea-128">ranges</span><span class="sxs-lookup"><span data-stu-id="b4bea-128">ranges</span></span>|<span data-ttu-id="b4bea-129">coleção [bucketAggregationRange](bucketaggregationrange.md)</span><span class="sxs-lookup"><span data-stu-id="b4bea-129">[bucketAggregationRange](bucketaggregationrange.md) collection</span></span>|<span data-ttu-id="b4bea-130">Especifica os intervalos manuais para calcular as agregações.</span><span class="sxs-lookup"><span data-stu-id="b4bea-130">Specifies the manual ranges to compute the aggregations.</span></span> <span data-ttu-id="b4bea-131">Isso é válido apenas para refinadores que não são de cadeia de caracteres do tipo data ou numérico.</span><span class="sxs-lookup"><span data-stu-id="b4bea-131">This is only valid for non-string refiners of date or numeric type.</span></span> <span data-ttu-id="b4bea-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b4bea-132">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4bea-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4bea-133">JSON representation</span></span>

<span data-ttu-id="b4bea-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4bea-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bucketAggregationDefinition",
  "baseType": null
}-->

```json
{
  "sortBy": "String",
  "isDescending": true,
  "prefixFilter": "String",
  "minimumCount": 1024,
  "ranges": [{"@odata.type": "microsoft.graph.bucketAggregationRange"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sortProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->