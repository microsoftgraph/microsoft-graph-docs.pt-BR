---
title: tipo de recurso do The Planner
description: O recurso **Planner** fornece acesso a recursos do Planner para um grupo. Ele não contém propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 4d20a6d5c4918f729189e95a27bad18d9f872c8a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521724"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="7c024-104">tipo de recurso do The Planner</span><span class="sxs-lookup"><span data-stu-id="7c024-104">plannerGroup resource type</span></span>

<span data-ttu-id="7c024-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7c024-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c024-106">O recurso **Planner** fornece acesso a recursos do Planner para um [grupo](group.md).</span><span class="sxs-lookup"><span data-stu-id="7c024-106">The **plannerGroup** resource provides access to Planner resources for a [group](group.md).</span></span> <span data-ttu-id="7c024-107">Ele não contém propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="7c024-107">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="7c024-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="7c024-108">Methods</span></span>

| <span data-ttu-id="7c024-109">Método</span><span class="sxs-lookup"><span data-stu-id="7c024-109">Method</span></span>           | <span data-ttu-id="7c024-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7c024-110">Return Type</span></span>    |<span data-ttu-id="7c024-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c024-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7c024-112">Listar planos</span><span class="sxs-lookup"><span data-stu-id="7c024-112">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="7c024-113">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="7c024-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="7c024-114">Obtenha uma coleção de objetos **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="7c024-114">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="7c024-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c024-115">Properties</span></span>
| <span data-ttu-id="7c024-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c024-116">Property</span></span>     | <span data-ttu-id="7c024-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c024-117">Type</span></span>   |<span data-ttu-id="7c024-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c024-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c024-119">id</span><span class="sxs-lookup"><span data-stu-id="7c024-119">id</span></span>|<span data-ttu-id="7c024-120">String</span><span class="sxs-lookup"><span data-stu-id="7c024-120">String</span></span>| <span data-ttu-id="7c024-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7c024-121">Read-only.</span></span> <span data-ttu-id="7c024-122">Identificador do **complannerr**</span><span class="sxs-lookup"><span data-stu-id="7c024-122">Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c024-123">Relações</span><span class="sxs-lookup"><span data-stu-id="7c024-123">Relationships</span></span>
| <span data-ttu-id="7c024-124">Relação</span><span class="sxs-lookup"><span data-stu-id="7c024-124">Relationship</span></span> | <span data-ttu-id="7c024-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c024-125">Type</span></span>   |<span data-ttu-id="7c024-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c024-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c024-127">Planeje</span><span class="sxs-lookup"><span data-stu-id="7c024-127">plans</span></span>|<span data-ttu-id="7c024-128">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="7c024-128">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="7c024-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7c024-129">Read-only.</span></span> <span data-ttu-id="7c024-130">Anulável.</span><span class="sxs-lookup"><span data-stu-id="7c024-130">Nullable.</span></span> <span data-ttu-id="7c024-131">Retorna o [plannerPlans](plannerplan.md) de Propriedade do grupo.</span><span class="sxs-lookup"><span data-stu-id="7c024-131">Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7c024-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c024-132">JSON representation</span></span>
<span data-ttu-id="7c024-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7c024-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.plannerGroup"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
