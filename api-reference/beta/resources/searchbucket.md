---
title: tipo de recurso searchBucket
description: Fornece uma agregação específica na resposta, o valor de um Bucket específico.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3fe375ca2e9695a237b60e30cdd9e98a9e545d35
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193822"
---
# <a name="searchbucket-resource-type"></a><span data-ttu-id="a7f7d-103">tipo de recurso searchBucket</span><span class="sxs-lookup"><span data-stu-id="a7f7d-103">searchBucket resource type</span></span>

<span data-ttu-id="a7f7d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7f7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7f7d-105">Representa um contêiner para um ou mais resultados de pesquisa que compartilham o mesmo valor para o campo de entidade que os agrega.</span><span class="sxs-lookup"><span data-stu-id="a7f7d-105">Represents a container for one or more search results that share the same value for the entity field that aggregates them.</span></span> 



## <a name="properties"></a><span data-ttu-id="a7f7d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7f7d-106">Properties</span></span>

| <span data-ttu-id="a7f7d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7f7d-107">Property</span></span>     | <span data-ttu-id="a7f7d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7f7d-108">Type</span></span>        | <span data-ttu-id="a7f7d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7f7d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a7f7d-110">key</span><span class="sxs-lookup"><span data-stu-id="a7f7d-110">key</span></span>|<span data-ttu-id="a7f7d-111">String</span><span class="sxs-lookup"><span data-stu-id="a7f7d-111">String</span></span>| <span data-ttu-id="a7f7d-112">O valor discreto do campo no qual uma agregação foi calculada.</span><span class="sxs-lookup"><span data-stu-id="a7f7d-112">The discrete value of the field that an aggregation was computed on.</span></span>|
|<span data-ttu-id="a7f7d-113">Count</span><span class="sxs-lookup"><span data-stu-id="a7f7d-113">count</span></span>|<span data-ttu-id="a7f7d-114">Int32</span><span class="sxs-lookup"><span data-stu-id="a7f7d-114">Int32</span></span>| <span data-ttu-id="a7f7d-115">O número de correspondências de pesquisa que compartilham o mesmo valor especificado na propriedade **Key** .</span><span class="sxs-lookup"><span data-stu-id="a7f7d-115">The number of search matches that share the same value specified in the **key** property.</span></span> |
|<span data-ttu-id="a7f7d-116">aggregationFilterToken</span><span class="sxs-lookup"><span data-stu-id="a7f7d-116">aggregationFilterToken</span></span>|<span data-ttu-id="a7f7d-117">String</span><span class="sxs-lookup"><span data-stu-id="a7f7d-117">String</span></span>| <span data-ttu-id="a7f7d-118">Um token contendo o filtro codificado para agregar correspondências de pesquisa pelo valor da **chave** específica.</span><span class="sxs-lookup"><span data-stu-id="a7f7d-118">A token containing the encoded filter to aggregate search matches by the specific **key** value.</span></span> <span data-ttu-id="a7f7d-119">Para usar o filtro, passe o token como parte da propriedade **aggregationFilter** em um objeto **searchRequest** , no formato **"{Field}: \\ " {aggregationFilterToken} \\ ""**.</span><span class="sxs-lookup"><span data-stu-id="a7f7d-119">To use the filter, pass the token as part of the **aggregationFilter** property in a **searchRequest** object, in the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span> <span data-ttu-id="a7f7d-120">Veja um [exemplo](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request).</span><span class="sxs-lookup"><span data-stu-id="a7f7d-120">See an [example](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7f7d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7f7d-121">JSON representation</span></span>

<span data-ttu-id="a7f7d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a7f7d-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchBucket",
  "baseType": null
}-->

```json
{
  "key": "String",
  "count": "10",  
  "aggregationFilterToken": "String"
}
```
