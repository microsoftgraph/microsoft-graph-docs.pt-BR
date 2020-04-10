---
title: tipo de recurso de filtro
description: Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerado em escopo.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6e7933bf2fef6240dd0dc53d7da975074225aa30
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217887"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="6c709-103">tipo de recurso de filtro</span><span class="sxs-lookup"><span data-stu-id="6c709-103">filterGroup resource type</span></span>

<span data-ttu-id="6c709-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c709-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c709-105">Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerado em escopo.</span><span class="sxs-lookup"><span data-stu-id="6c709-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="6c709-106">Um objeto é considerado no escopo do grupo (o grupo é avaliado como `true`) somente se todas as cláusulas do grupo são avaliadas. `true`</span><span class="sxs-lookup"><span data-stu-id="6c709-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="6c709-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c709-107">Properties</span></span>
| <span data-ttu-id="6c709-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c709-108">Property</span></span>     | <span data-ttu-id="6c709-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c709-109">Type</span></span>   |<span data-ttu-id="6c709-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c709-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c709-111">cláusulas</span><span class="sxs-lookup"><span data-stu-id="6c709-111">clauses</span></span>|<span data-ttu-id="6c709-112">coleção [filterClause](synchronization-filterclause.md)</span><span class="sxs-lookup"><span data-stu-id="6c709-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="6c709-113">Cláusulas de filtro (condições) desse grupo.</span><span class="sxs-lookup"><span data-stu-id="6c709-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="6c709-114">Todas as cláusulas em um grupo devem ser atendidas para que o grupo de filtros seja `true`avaliado.</span><span class="sxs-lookup"><span data-stu-id="6c709-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="6c709-115">nome</span><span class="sxs-lookup"><span data-stu-id="6c709-115">name</span></span>|<span data-ttu-id="6c709-116">String</span><span class="sxs-lookup"><span data-stu-id="6c709-116">String</span></span>|<span data-ttu-id="6c709-117">Nome legível do grupo de filtros.</span><span class="sxs-lookup"><span data-stu-id="6c709-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c709-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c709-118">JSON representation</span></span>

<span data-ttu-id="6c709-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c709-119">The following is a JSON representation of the resource.</span></span>

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
