---
title: tipo de recurso de filtro
description: Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerado em escopo. Um objeto é considerado no escopo do grupo (o grupo é avaliado como `true`) somente se todas as cláusulas do grupo são avaliadas. `true`
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 433528d9d663a3dc19cecaa5c2dad68e362dc882
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520181"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="1d5db-104">tipo de recurso de filtro</span><span class="sxs-lookup"><span data-stu-id="1d5db-104">filterGroup resource type</span></span>

<span data-ttu-id="1d5db-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1d5db-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d5db-106">Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerado em escopo.</span><span class="sxs-lookup"><span data-stu-id="1d5db-106">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="1d5db-107">Um objeto é considerado no escopo do grupo (o grupo é avaliado como `true`) somente se todas as cláusulas do grupo são avaliadas. `true`</span><span class="sxs-lookup"><span data-stu-id="1d5db-107">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="1d5db-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d5db-108">Properties</span></span>
| <span data-ttu-id="1d5db-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d5db-109">Property</span></span>     | <span data-ttu-id="1d5db-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d5db-110">Type</span></span>   |<span data-ttu-id="1d5db-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d5db-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d5db-112">cláusulas</span><span class="sxs-lookup"><span data-stu-id="1d5db-112">clauses</span></span>|<span data-ttu-id="1d5db-113">coleção [filterClause](synchronization-filterclause.md)</span><span class="sxs-lookup"><span data-stu-id="1d5db-113">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="1d5db-114">Cláusulas de filtro (condições) desse grupo.</span><span class="sxs-lookup"><span data-stu-id="1d5db-114">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="1d5db-115">Todas as cláusulas em um grupo devem ser atendidas para que o grupo de filtros seja `true`avaliado.</span><span class="sxs-lookup"><span data-stu-id="1d5db-115">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="1d5db-116">nome</span><span class="sxs-lookup"><span data-stu-id="1d5db-116">name</span></span>|<span data-ttu-id="1d5db-117">String</span><span class="sxs-lookup"><span data-stu-id="1d5db-117">String</span></span>|<span data-ttu-id="1d5db-118">Nome legível do grupo de filtros.</span><span class="sxs-lookup"><span data-stu-id="1d5db-118">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d5db-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d5db-119">JSON representation</span></span>

<span data-ttu-id="1d5db-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d5db-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterGroup"
}-->

```json
{
  "clauses": [{"@odata.type": "microsoft.graph.filterClause"}],
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
