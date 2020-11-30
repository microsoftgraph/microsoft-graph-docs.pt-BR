---
title: tipo de recurso searchQuery
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3745083b404a8de6f68844af9b1767ac2319059f
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377955"
---
# <a name="searchquery-resource-type"></a><span data-ttu-id="e676e-103">tipo de recurso searchQuery</span><span class="sxs-lookup"><span data-stu-id="e676e-103">searchQuery resource type</span></span>

<span data-ttu-id="e676e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e676e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e676e-105">Representa uma consulta de pesquisa que contém termos de pesquisa e filtros opcionais.</span><span class="sxs-lookup"><span data-stu-id="e676e-105">Represents a search query that contains search terms and optional filters.</span></span>

## <a name="properties"></a><span data-ttu-id="e676e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e676e-106">Properties</span></span>

| <span data-ttu-id="e676e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e676e-107">Property</span></span>     | <span data-ttu-id="e676e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e676e-108">Type</span></span>        | <span data-ttu-id="e676e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e676e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e676e-110">queryString</span><span class="sxs-lookup"><span data-stu-id="e676e-110">queryString</span></span>|<span data-ttu-id="e676e-111">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e676e-111">String</span></span>|<span data-ttu-id="e676e-112">A consulta de pesquisa que contém os termos da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="e676e-112">The search query containing the search terms.</span></span> <span data-ttu-id="e676e-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e676e-113">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e676e-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e676e-114">JSON representation</span></span>

<span data-ttu-id="e676e-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e676e-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQuery",
  "baseType": null
}-->

```json
{
  "queryString": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

