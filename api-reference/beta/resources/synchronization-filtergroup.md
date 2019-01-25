---
title: tipo de recurso de filterGroup
description: Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerados no escopo. Um objeto é considerado no escopo do grupo (o grupo é avaliado para `true`) somente se todas as cláusulas do grupo são avaliadas para `true`.
localization_priority: Normal
ms.openlocfilehash: b71bdf16d6639b5ecc8512565ccf56d592a0da58
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514184"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="66144-104">tipo de recurso de filterGroup</span><span class="sxs-lookup"><span data-stu-id="66144-104">filterGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66144-105">Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerados no escopo.</span><span class="sxs-lookup"><span data-stu-id="66144-105">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="66144-106">Um objeto é considerado no escopo do grupo (o grupo é avaliado para `true`) somente se todas as cláusulas do grupo são avaliadas para `true`.</span><span class="sxs-lookup"><span data-stu-id="66144-106">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="66144-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66144-107">Properties</span></span>
| <span data-ttu-id="66144-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66144-108">Property</span></span>     | <span data-ttu-id="66144-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="66144-109">Type</span></span>   |<span data-ttu-id="66144-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="66144-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66144-111">Cláusulas</span><span class="sxs-lookup"><span data-stu-id="66144-111">clauses</span></span>|<span data-ttu-id="66144-112">coleção [filterClause](synchronization-filterclause.md)</span><span class="sxs-lookup"><span data-stu-id="66144-112">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="66144-113">Filtre cláusulas (condições) desse grupo.</span><span class="sxs-lookup"><span data-stu-id="66144-113">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="66144-114">Todas as cláusulas em um grupo devem ser atendidas para o grupo de filtro a ser avaliada como `true`.</span><span class="sxs-lookup"><span data-stu-id="66144-114">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="66144-115">name</span><span class="sxs-lookup"><span data-stu-id="66144-115">name</span></span>|<span data-ttu-id="66144-116">String</span><span class="sxs-lookup"><span data-stu-id="66144-116">String</span></span>|<span data-ttu-id="66144-117">Legíveis nome do grupo de filtro.</span><span class="sxs-lookup"><span data-stu-id="66144-117">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66144-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66144-118">JSON representation</span></span>

<span data-ttu-id="66144-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66144-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filtergroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
