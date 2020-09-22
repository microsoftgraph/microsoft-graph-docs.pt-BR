---
title: tipo de recurso do The Planner
description: O recurso **Planner** fornece acesso a recursos do Planner para um grupo. Ele não contém propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 6b4a282dcefe06ade0d4af1bb911449b168ac00c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067220"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="3a10e-104">tipo de recurso do The Planner</span><span class="sxs-lookup"><span data-stu-id="3a10e-104">plannerGroup resource type</span></span>

<span data-ttu-id="3a10e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a10e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a10e-106">O recurso **Planner** fornece acesso a recursos do Planner para um [grupo](group.md).</span><span class="sxs-lookup"><span data-stu-id="3a10e-106">The **plannerGroup** resource provides access to Planner resources for a [group](group.md).</span></span> <span data-ttu-id="3a10e-107">Ele não contém propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="3a10e-107">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="3a10e-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="3a10e-108">Methods</span></span>

| <span data-ttu-id="3a10e-109">Método</span><span class="sxs-lookup"><span data-stu-id="3a10e-109">Method</span></span>           | <span data-ttu-id="3a10e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3a10e-110">Return Type</span></span>    |<span data-ttu-id="3a10e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a10e-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3a10e-112">Listar planos</span><span class="sxs-lookup"><span data-stu-id="3a10e-112">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="3a10e-113">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="3a10e-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="3a10e-114">Obtenha uma coleção de objetos **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="3a10e-114">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="3a10e-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a10e-115">Properties</span></span>
| <span data-ttu-id="3a10e-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a10e-116">Property</span></span>     | <span data-ttu-id="3a10e-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a10e-117">Type</span></span>   |<span data-ttu-id="3a10e-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a10e-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a10e-119">id</span><span class="sxs-lookup"><span data-stu-id="3a10e-119">id</span></span>|<span data-ttu-id="3a10e-120">String</span><span class="sxs-lookup"><span data-stu-id="3a10e-120">String</span></span>| <span data-ttu-id="3a10e-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3a10e-121">Read-only.</span></span> <span data-ttu-id="3a10e-122">Identificador do **complannerr**</span><span class="sxs-lookup"><span data-stu-id="3a10e-122">Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a10e-123">Relações</span><span class="sxs-lookup"><span data-stu-id="3a10e-123">Relationships</span></span>
| <span data-ttu-id="3a10e-124">Relação</span><span class="sxs-lookup"><span data-stu-id="3a10e-124">Relationship</span></span> | <span data-ttu-id="3a10e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a10e-125">Type</span></span>   |<span data-ttu-id="3a10e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a10e-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a10e-127">Planeje</span><span class="sxs-lookup"><span data-stu-id="3a10e-127">plans</span></span>|<span data-ttu-id="3a10e-128">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="3a10e-128">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="3a10e-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3a10e-129">Read-only.</span></span> <span data-ttu-id="3a10e-130">Anulável.</span><span class="sxs-lookup"><span data-stu-id="3a10e-130">Nullable.</span></span> <span data-ttu-id="3a10e-131">Retorna o [plannerPlans](plannerplan.md) de Propriedade do grupo.</span><span class="sxs-lookup"><span data-stu-id="3a10e-131">Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3a10e-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a10e-132">JSON representation</span></span>
<span data-ttu-id="3a10e-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a10e-133">Here is a JSON representation of the resource.</span></span>

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


