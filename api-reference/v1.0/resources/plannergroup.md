---
title: Tipo de recurso plannerGroup
description: O recurso de **plannerGroup** fornece acesso aos recursos de Planejador para um grupo. Não contém todas as propriedades utilizáveis.
localization_priority: Normal
ms.openlocfilehash: ac55c0acd3561205654383cbb1b3d264c219d1a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871964"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="5e5a4-104">Tipo de recurso plannerGroup</span><span class="sxs-lookup"><span data-stu-id="5e5a4-104">plannerGroup resource type</span></span>

<span data-ttu-id="5e5a4-p102">O recurso **plannerGroup** oferece acesso aos recursos do Planner para um [grupo](group.md). Ele não contém quaisquer propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="5e5a4-p102">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="5e5a4-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5e5a4-107">Methods</span></span>

| <span data-ttu-id="5e5a4-108">Método</span><span class="sxs-lookup"><span data-stu-id="5e5a4-108">Method</span></span>           | <span data-ttu-id="5e5a4-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5e5a4-109">Return Type</span></span>    |<span data-ttu-id="5e5a4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e5a4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e5a4-111">Listar planos</span><span class="sxs-lookup"><span data-stu-id="5e5a4-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="5e5a4-112">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="5e5a4-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="5e5a4-113">Obtenha uma coleção de objetos **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="5e5a4-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e5a4-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e5a4-114">Properties</span></span>
| <span data-ttu-id="5e5a4-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e5a4-115">Property</span></span>     | <span data-ttu-id="5e5a4-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e5a4-116">Type</span></span>   |<span data-ttu-id="5e5a4-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e5a4-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e5a4-118">id</span><span class="sxs-lookup"><span data-stu-id="5e5a4-118">id</span></span>|<span data-ttu-id="5e5a4-119">String</span><span class="sxs-lookup"><span data-stu-id="5e5a4-119">String</span></span>| <span data-ttu-id="5e5a4-p103">Somente leitura. O identificador do **plannerGroup**</span><span class="sxs-lookup"><span data-stu-id="5e5a4-p103">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e5a4-122">Relações</span><span class="sxs-lookup"><span data-stu-id="5e5a4-122">Relationships</span></span>
| <span data-ttu-id="5e5a4-123">Relação</span><span class="sxs-lookup"><span data-stu-id="5e5a4-123">Relationship</span></span> | <span data-ttu-id="5e5a4-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e5a4-124">Type</span></span>   |<span data-ttu-id="5e5a4-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e5a4-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e5a4-126">plans</span><span class="sxs-lookup"><span data-stu-id="5e5a4-126">plans</span></span>|<span data-ttu-id="5e5a4-127">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="5e5a4-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="5e5a4-p104">Somente leitura. Anulável. Retorna o [plannerPlans](plannerplan.md) que pertence ao grupo.</span><span class="sxs-lookup"><span data-stu-id="5e5a4-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e5a4-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e5a4-131">JSON representation</span></span>
<span data-ttu-id="5e5a4-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e5a4-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
