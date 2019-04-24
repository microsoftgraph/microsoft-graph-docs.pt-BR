---
title: tipo de recurso do The Planner
description: O recurso **Planner** fornece acesso a recursos do Planner para um grupo. Ele não contém propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 84bb20d0b13f9a99db2f8c59b20e0c9c7c87f93f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457029"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="93578-104">tipo de recurso do The Planner</span><span class="sxs-lookup"><span data-stu-id="93578-104">plannerGroup resource type</span></span>

<span data-ttu-id="93578-105">O recurso **Planner** fornece acesso a recursos do Planner para um [grupo](group.md).</span><span class="sxs-lookup"><span data-stu-id="93578-105">The **plannerGroup** resource provides access to Planner resources for a [group](group.md).</span></span> <span data-ttu-id="93578-106">Ele não contém propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="93578-106">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="93578-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="93578-107">Methods</span></span>

| <span data-ttu-id="93578-108">Método</span><span class="sxs-lookup"><span data-stu-id="93578-108">Method</span></span>           | <span data-ttu-id="93578-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="93578-109">Return Type</span></span>    |<span data-ttu-id="93578-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="93578-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="93578-111">Listar planos</span><span class="sxs-lookup"><span data-stu-id="93578-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="93578-112">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="93578-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="93578-113">Obtenha uma coleção de objetos **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="93578-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="93578-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93578-114">Properties</span></span>
| <span data-ttu-id="93578-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93578-115">Property</span></span>     | <span data-ttu-id="93578-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="93578-116">Type</span></span>   |<span data-ttu-id="93578-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="93578-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93578-118">id</span><span class="sxs-lookup"><span data-stu-id="93578-118">id</span></span>|<span data-ttu-id="93578-119">String</span><span class="sxs-lookup"><span data-stu-id="93578-119">String</span></span>| <span data-ttu-id="93578-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="93578-120">Read-only.</span></span> <span data-ttu-id="93578-121">Identificador do complannerr \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="93578-121">Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="93578-122">Relações</span><span class="sxs-lookup"><span data-stu-id="93578-122">Relationships</span></span>
| <span data-ttu-id="93578-123">Relação</span><span class="sxs-lookup"><span data-stu-id="93578-123">Relationship</span></span> | <span data-ttu-id="93578-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="93578-124">Type</span></span>   |<span data-ttu-id="93578-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="93578-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93578-126">Planeje</span><span class="sxs-lookup"><span data-stu-id="93578-126">plans</span></span>|<span data-ttu-id="93578-127">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="93578-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="93578-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="93578-128">Read-only.</span></span> <span data-ttu-id="93578-129">Anulável.</span><span class="sxs-lookup"><span data-stu-id="93578-129">Nullable.</span></span> <span data-ttu-id="93578-130">Retorna o [plannerPlans](plannerplan.md) de Propriedade do grupo.</span><span class="sxs-lookup"><span data-stu-id="93578-130">Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93578-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93578-131">JSON representation</span></span>
<span data-ttu-id="93578-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93578-132">Here is a JSON representation of the resource.</span></span>

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
