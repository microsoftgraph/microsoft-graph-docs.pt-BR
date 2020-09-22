---
title: tipo de recurso aggregationOption
description: Especifica a entidade aggregationOption
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c18cc1801e5eac76d2fa4396f809ff68f59a78fe
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193831"
---
# <a name="aggregationoption-resource-type"></a><span data-ttu-id="d3579-103">tipo de recurso aggregationOption</span><span class="sxs-lookup"><span data-stu-id="d3579-103">aggregationOption resource type</span></span>

<span data-ttu-id="d3579-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3579-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3579-105">Especifica quais agregações devem ser retornadas junto com os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="d3579-105">Specifies which aggregations should be returned alongside the search results.</span></span>

## <a name="properties"></a><span data-ttu-id="d3579-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3579-106">Properties</span></span>

| <span data-ttu-id="d3579-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3579-107">Property</span></span>     | <span data-ttu-id="d3579-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3579-108">Type</span></span>        | <span data-ttu-id="d3579-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3579-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d3579-110">campo</span><span class="sxs-lookup"><span data-stu-id="d3579-110">field</span></span>|<span data-ttu-id="d3579-111">String</span><span class="sxs-lookup"><span data-stu-id="d3579-111">String</span></span>|<span data-ttu-id="d3579-112">Especifica o campo no esquema do tipo de entidade especificado em que a agregação deve ser calculada.</span><span class="sxs-lookup"><span data-stu-id="d3579-112">Specifies the field in the schema of the specified entity type that aggregation should be computed on.</span></span> <span data-ttu-id="d3579-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3579-113">Required.</span></span>|
|<span data-ttu-id="d3579-114">size</span><span class="sxs-lookup"><span data-stu-id="d3579-114">size</span></span>|<span data-ttu-id="d3579-115">Int32</span><span class="sxs-lookup"><span data-stu-id="d3579-115">Int32</span></span>|<span data-ttu-id="d3579-116">O número de recursos [searchBucket](searchBucket.md) a serem retornados.</span><span class="sxs-lookup"><span data-stu-id="d3579-116">The number of [searchBucket](searchBucket.md) resources to be returned.</span></span> <span data-ttu-id="d3579-117">Isso não é necessário quando o intervalo é fornecido manualmente na solicitação de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="d3579-117">This is not required when the range is provided manually in the search request.</span></span> <span data-ttu-id="d3579-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d3579-118">Optional.</span></span>|
|<span data-ttu-id="d3579-119">bucketDefinition</span><span class="sxs-lookup"><span data-stu-id="d3579-119">bucketDefinition</span></span>|[<span data-ttu-id="d3579-120">bucketAggregationDefinition</span><span class="sxs-lookup"><span data-stu-id="d3579-120">bucketAggregationDefinition</span></span>](bucketaggregationdefinition.md)|<span data-ttu-id="d3579-121">Especifica os critérios para calcular uma agregação.</span><span class="sxs-lookup"><span data-stu-id="d3579-121">Specifies the criteria to compute an aggregation.</span></span> <span data-ttu-id="d3579-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d3579-122">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3579-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3579-123">JSON representation</span></span>

<span data-ttu-id="d3579-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3579-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.aggregationOption",
  "baseType": null
}-->

```json
{
  "field": "String",
  "size": 1024,
  "bucketDefinition": {"@odata.type": "microsoft.graph.bucketAggregationDefinition"}
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