---
title: Tipo de recurso filterGroup
description: Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerado no escopo.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 6338ae4b02b79d1512d5e9f695a69155197e2f4a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131912"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="02fc9-103">Tipo de recurso filterGroup</span><span class="sxs-lookup"><span data-stu-id="02fc9-103">filterGroup resource type</span></span>

<span data-ttu-id="02fc9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02fc9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02fc9-105">Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerado no escopo.</span><span class="sxs-lookup"><span data-stu-id="02fc9-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="02fc9-106">Um objeto é considerado no escopo do grupo (o grupo é avaliado para ) somente se todas as cláusulas do grupo são `true` avaliadas para `true` .</span><span class="sxs-lookup"><span data-stu-id="02fc9-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="02fc9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="02fc9-107">Properties</span></span>
| <span data-ttu-id="02fc9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02fc9-108">Property</span></span>     | <span data-ttu-id="02fc9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="02fc9-109">Type</span></span>   |<span data-ttu-id="02fc9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="02fc9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02fc9-111">clauses</span><span class="sxs-lookup"><span data-stu-id="02fc9-111">clauses</span></span>|<span data-ttu-id="02fc9-112">[Coleção filterClause](synchronization-filterclause.md)</span><span class="sxs-lookup"><span data-stu-id="02fc9-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="02fc9-113">Cláusulas de filtro (condições) desse grupo.</span><span class="sxs-lookup"><span data-stu-id="02fc9-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="02fc9-114">Todas as cláusulas em um grupo devem ser atendidas para que o grupo de filtros seja avaliada como `true` .</span><span class="sxs-lookup"><span data-stu-id="02fc9-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="02fc9-115">nome</span><span class="sxs-lookup"><span data-stu-id="02fc9-115">name</span></span>|<span data-ttu-id="02fc9-116">String</span><span class="sxs-lookup"><span data-stu-id="02fc9-116">String</span></span>|<span data-ttu-id="02fc9-117">Nome acessível para humanos do grupo de filtros.</span><span class="sxs-lookup"><span data-stu-id="02fc9-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02fc9-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="02fc9-118">JSON representation</span></span>

<span data-ttu-id="02fc9-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="02fc9-119">The following is a JSON representation of the resource.</span></span>

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


