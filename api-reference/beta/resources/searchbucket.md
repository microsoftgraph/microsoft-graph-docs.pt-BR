---
title: tipo de recurso searchBucket
description: Fornece uma agregação específica na resposta, o valor de um Bucket específico.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a6b26c01133f519b0308ffee430d85c9df6d868b
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373850"
---
# <a name="searchbucket-resource-type"></a><span data-ttu-id="a4327-103">tipo de recurso searchBucket</span><span class="sxs-lookup"><span data-stu-id="a4327-103">searchBucket resource type</span></span>

<span data-ttu-id="a4327-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4327-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4327-105">Representa um contêiner para um ou mais resultados de pesquisa que compartilham o mesmo valor para o campo de entidade que os agrega.</span><span class="sxs-lookup"><span data-stu-id="a4327-105">Represents a container for one or more search results that share the same value for the entity field that aggregates them.</span></span> 

## <a name="properties"></a><span data-ttu-id="a4327-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4327-106">Properties</span></span>

| <span data-ttu-id="a4327-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4327-107">Property</span></span>     | <span data-ttu-id="a4327-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4327-108">Type</span></span>        | <span data-ttu-id="a4327-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4327-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a4327-110">key</span><span class="sxs-lookup"><span data-stu-id="a4327-110">key</span></span>|<span data-ttu-id="a4327-111">String</span><span class="sxs-lookup"><span data-stu-id="a4327-111">String</span></span>| <span data-ttu-id="a4327-112">O valor discreto do campo no qual uma agregação foi calculada.</span><span class="sxs-lookup"><span data-stu-id="a4327-112">The discrete value of the field that an aggregation was computed on.</span></span>|
|<span data-ttu-id="a4327-113">Count</span><span class="sxs-lookup"><span data-stu-id="a4327-113">count</span></span>|<span data-ttu-id="a4327-114">Int32</span><span class="sxs-lookup"><span data-stu-id="a4327-114">Int32</span></span>| <span data-ttu-id="a4327-115">O número aproximado de correspondências de pesquisa que compartilham o mesmo valor especificado na propriedade **Key** .</span><span class="sxs-lookup"><span data-stu-id="a4327-115">The approximate number of search matches that share the same value specified in the **key** property.</span></span> <span data-ttu-id="a4327-116">Observe que esse número não é o número exato de correspondências.</span><span class="sxs-lookup"><span data-stu-id="a4327-116">Note that this number is not the exact number of matches.</span></span>|
|<span data-ttu-id="a4327-117">aggregationFilterToken</span><span class="sxs-lookup"><span data-stu-id="a4327-117">aggregationFilterToken</span></span>|<span data-ttu-id="a4327-118">String</span><span class="sxs-lookup"><span data-stu-id="a4327-118">String</span></span>| <span data-ttu-id="a4327-119">Um token contendo o filtro codificado para agregar correspondências de pesquisa pelo valor da **chave** específica.</span><span class="sxs-lookup"><span data-stu-id="a4327-119">A token containing the encoded filter to aggregate search matches by the specific **key** value.</span></span> <span data-ttu-id="a4327-120">Para usar o filtro, passe o token como parte da propriedade **aggregationFilter** em um objeto **searchRequest** , no formato **"{Field}: \\ " {aggregationFilterToken} \\ ""**.</span><span class="sxs-lookup"><span data-stu-id="a4327-120">To use the filter, pass the token as part of the **aggregationFilter** property in a **searchRequest** object, in the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span> <span data-ttu-id="a4327-121">Veja um [exemplo](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request).</span><span class="sxs-lookup"><span data-stu-id="a4327-121">See an [example](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4327-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4327-122">JSON representation</span></span>

<span data-ttu-id="a4327-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a4327-123">The following is a JSON representation of the resource.</span></span>

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
