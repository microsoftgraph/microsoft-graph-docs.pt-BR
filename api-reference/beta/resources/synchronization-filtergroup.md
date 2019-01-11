---
title: tipo de recurso de filterGroup
description: Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerados no escopo. Um objeto é considerado no escopo do grupo (o grupo é avaliado para `true`) somente se todas as cláusulas do grupo são avaliadas para `true`.
localization_priority: Normal
ms.openlocfilehash: 174c02518069e949c49887d9e21e778e8455509a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836110"
---
# <a name="filtergroup-resource-type"></a><span data-ttu-id="36491-104">tipo de recurso de filterGroup</span><span class="sxs-lookup"><span data-stu-id="36491-104">filterGroup resource type</span></span>

> <span data-ttu-id="36491-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="36491-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36491-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="36491-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="36491-107">Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerados no escopo.</span><span class="sxs-lookup"><span data-stu-id="36491-107">Defines a set of clauses that an object must satisfy to be considered in scope.</span></span> <span data-ttu-id="36491-108">Um objeto é considerado no escopo do grupo (o grupo é avaliado para `true`) somente se todas as cláusulas do grupo são avaliadas para `true`.</span><span class="sxs-lookup"><span data-stu-id="36491-108">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

## <a name="properties"></a><span data-ttu-id="36491-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36491-109">Properties</span></span>
| <span data-ttu-id="36491-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36491-110">Property</span></span>     | <span data-ttu-id="36491-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="36491-111">Type</span></span>   |<span data-ttu-id="36491-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="36491-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36491-113">cláusulas</span><span class="sxs-lookup"><span data-stu-id="36491-113">clauses</span></span>|<span data-ttu-id="36491-114">coleção [filterClause](synchronization-filterclause.md)</span><span class="sxs-lookup"><span data-stu-id="36491-114">[filterClause](synchronization-filterclause.md) collection</span></span>|<span data-ttu-id="36491-115">Filtre cláusulas (condições) desse grupo.</span><span class="sxs-lookup"><span data-stu-id="36491-115">Filter clauses (conditions) of this group.</span></span> <span data-ttu-id="36491-116">Todas as cláusulas em um grupo devem ser atendidas para o grupo de filtro a ser avaliada como `true`.</span><span class="sxs-lookup"><span data-stu-id="36491-116">All clauses in a group must be satisfied in order for the filter group to evaluate to `true`.</span></span>|
|<span data-ttu-id="36491-117">name</span><span class="sxs-lookup"><span data-stu-id="36491-117">name</span></span>|<span data-ttu-id="36491-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36491-118">String</span></span>|<span data-ttu-id="36491-119">Legíveis nome do grupo de filtro.</span><span class="sxs-lookup"><span data-stu-id="36491-119">Human-readable name of the filter group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36491-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36491-120">JSON representation</span></span>

<span data-ttu-id="36491-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36491-121">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
