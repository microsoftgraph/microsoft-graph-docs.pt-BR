---
title: tipo de recurso do The Planner
description: O recurso **Planner** fornece acesso a recursos do Planner para um grupo. Ele não contém propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 65d0e81eede4f5edf75a43eaa662e9c044674624
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035235"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="ce426-104">tipo de recurso do The Planner</span><span class="sxs-lookup"><span data-stu-id="ce426-104">plannerGroup resource type</span></span>

<span data-ttu-id="ce426-105">O recurso **Planner** fornece acesso a recursos do Planner para um [grupo](group.md).</span><span class="sxs-lookup"><span data-stu-id="ce426-105">The **plannerGroup** resource provides access to Planner resources for a [group](group.md).</span></span> <span data-ttu-id="ce426-106">Ele não contém propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="ce426-106">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="ce426-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ce426-107">Methods</span></span>

| <span data-ttu-id="ce426-108">Método</span><span class="sxs-lookup"><span data-stu-id="ce426-108">Method</span></span>           | <span data-ttu-id="ce426-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ce426-109">Return Type</span></span>    |<span data-ttu-id="ce426-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce426-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ce426-111">Listar planos</span><span class="sxs-lookup"><span data-stu-id="ce426-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="ce426-112">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="ce426-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ce426-113">Obtenha uma coleção de objetos **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="ce426-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="ce426-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce426-114">Properties</span></span>
| <span data-ttu-id="ce426-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce426-115">Property</span></span>     | <span data-ttu-id="ce426-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce426-116">Type</span></span>   |<span data-ttu-id="ce426-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce426-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce426-118">id</span><span class="sxs-lookup"><span data-stu-id="ce426-118">id</span></span>|<span data-ttu-id="ce426-119">String</span><span class="sxs-lookup"><span data-stu-id="ce426-119">String</span></span>| <span data-ttu-id="ce426-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce426-120">Read-only.</span></span> <span data-ttu-id="ce426-121">Identificador do complannerr \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="ce426-121">Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce426-122">Relações</span><span class="sxs-lookup"><span data-stu-id="ce426-122">Relationships</span></span>
| <span data-ttu-id="ce426-123">Relação</span><span class="sxs-lookup"><span data-stu-id="ce426-123">Relationship</span></span> | <span data-ttu-id="ce426-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce426-124">Type</span></span>   |<span data-ttu-id="ce426-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce426-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce426-126">Planeje</span><span class="sxs-lookup"><span data-stu-id="ce426-126">plans</span></span>|<span data-ttu-id="ce426-127">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="ce426-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ce426-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce426-128">Read-only.</span></span> <span data-ttu-id="ce426-129">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ce426-129">Nullable.</span></span> <span data-ttu-id="ce426-130">Retorna o [plannerPlans](plannerplan.md) de Propriedade do grupo.</span><span class="sxs-lookup"><span data-stu-id="ce426-130">Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ce426-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce426-131">JSON representation</span></span>
<span data-ttu-id="ce426-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce426-132">Here is a JSON representation of the resource.</span></span>

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
