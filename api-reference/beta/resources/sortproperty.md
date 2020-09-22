---
title: tipo de recurso SortProperty
description: Oferece a opção de classificar os resultados da pesquisa.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1f1288b2dc9ec05fe8aaedb5871c3bda68714f90
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193832"
---
# <a name="sortproperty-resource-type"></a><span data-ttu-id="129df-103">tipo de recurso SortProperty</span><span class="sxs-lookup"><span data-stu-id="129df-103">sortProperty resource type</span></span>

<span data-ttu-id="129df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="129df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="129df-105">Representa as opções de classificação para ordenar os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="129df-105">Represents the sort options to order search results.</span></span>

## <a name="properties"></a><span data-ttu-id="129df-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="129df-106">Properties</span></span>

| <span data-ttu-id="129df-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="129df-107">Property</span></span>     | <span data-ttu-id="129df-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="129df-108">Type</span></span>        | <span data-ttu-id="129df-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="129df-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="129df-110">nome</span><span class="sxs-lookup"><span data-stu-id="129df-110">name</span></span>|<span data-ttu-id="129df-111">String</span><span class="sxs-lookup"><span data-stu-id="129df-111">String</span></span>|<span data-ttu-id="129df-112">O nome da propriedade a ser classificada.</span><span class="sxs-lookup"><span data-stu-id="129df-112">The name of the property to sort on.</span></span> <span data-ttu-id="129df-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="129df-113">Required.</span></span>|
|<span data-ttu-id="129df-114">isDescending</span><span class="sxs-lookup"><span data-stu-id="129df-114">isDescending</span></span>|<span data-ttu-id="129df-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="129df-115">Boolean</span></span>|<span data-ttu-id="129df-116">`True` se a ordem de classificação for decrescente.</span><span class="sxs-lookup"><span data-stu-id="129df-116">`True` if the sort order is descending.</span></span> <span data-ttu-id="129df-117">O padrão é `false` , com a ordem de classificação como crescente.</span><span class="sxs-lookup"><span data-stu-id="129df-117">Default is `false`, with the sort order as ascending.</span></span> <span data-ttu-id="129df-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="129df-118">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="129df-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="129df-119">JSON representation</span></span>

<span data-ttu-id="129df-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="129df-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sortProperty",
  "baseType": null
}-->

```json
{
  "name": "String",
  "isDescending": "true"
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