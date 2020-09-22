---
title: tipo de recurso bucketAggregationRange
description: 'Permite especificar alguns intervalos manuais na solicitação de agregação. Isso só é aplicável a refinadores não cadeias de caracteres: numéricos e datas.'
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 77f89503a8f19bd8b057575643ebf89e6dbc43a8
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193836"
---
# <a name="bucketaggregationrange-resource-type"></a><span data-ttu-id="71324-104">tipo de recurso bucketAggregationRange</span><span class="sxs-lookup"><span data-stu-id="71324-104">bucketAggregationRange resource type</span></span>

<span data-ttu-id="71324-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71324-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71324-106">Especifica o limite inferior e superior para um intervalo de agregação de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="71324-106">Specifies the lower and upper limit to a range for aggregating search results.</span></span> <span data-ttu-id="71324-107">Aplica-se somente a refinadores da data ou tipo numérico.</span><span class="sxs-lookup"><span data-stu-id="71324-107">Applies to only refiners of the date or numeric type.</span></span>

## <a name="properties"></a><span data-ttu-id="71324-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71324-108">Properties</span></span>

| <span data-ttu-id="71324-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71324-109">Property</span></span>     | <span data-ttu-id="71324-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="71324-110">Type</span></span>        | <span data-ttu-id="71324-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="71324-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="71324-112">from</span><span class="sxs-lookup"><span data-stu-id="71324-112">from</span></span>|<span data-ttu-id="71324-113">String</span><span class="sxs-lookup"><span data-stu-id="71324-113">String</span></span>| <span data-ttu-id="71324-114">Define o limite inferior a partir do qual a agregação será calculada.</span><span class="sxs-lookup"><span data-stu-id="71324-114">Defines the lower bound from which to compute the aggregation.</span></span> <span data-ttu-id="71324-115">Pode ser um valor numérico ou uma representação de cadeia de caracteres de uma data usando o `YYYY-MM-DDTHH:mm:ss.sssZ` formato.</span><span class="sxs-lookup"><span data-stu-id="71324-115">This can be a numeric value or a string representation of a date using the `YYYY-MM-DDTHH:mm:ss.sssZ` format.</span></span> <span data-ttu-id="71324-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71324-116">Required.</span></span>|
|<span data-ttu-id="71324-117">para</span><span class="sxs-lookup"><span data-stu-id="71324-117">to</span></span>|<span data-ttu-id="71324-118">String</span><span class="sxs-lookup"><span data-stu-id="71324-118">String</span></span>| <span data-ttu-id="71324-119">Define o limite superior até o qual calcular a agregação.</span><span class="sxs-lookup"><span data-stu-id="71324-119">Defines the upper bound up to which to compute the aggregation.</span></span> <span data-ttu-id="71324-120">Pode ser um valor numérico ou uma representação de cadeia de caracteres de uma data usando o `YYYY-MM-DDTHH:mm:ss.sssZ` formato.</span><span class="sxs-lookup"><span data-stu-id="71324-120">This can be a numeric value or a string representation of a date using the `YYYY-MM-DDTHH:mm:ss.sssZ` format.</span></span> <span data-ttu-id="71324-121">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71324-121">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71324-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71324-122">JSON representation</span></span>

<span data-ttu-id="71324-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71324-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bucketAggregationRange",
  "baseType": null
}-->

```json
{
  "from": "String",
  "to": "String"
}
```
