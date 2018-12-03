---
title: Tipo de recurso plannerGroup
description: O recurso de **plannerGroup** fornece acesso aos recursos de Planejador para um grupo. Não contém todas as propriedades utilizáveis.
ms.openlocfilehash: 03db48d9525915ec58ee902922fa0292c0fd89ec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035522"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="bfb14-104">Tipo de recurso plannerGroup</span><span class="sxs-lookup"><span data-stu-id="bfb14-104">plannerGroup resource type</span></span>

> <span data-ttu-id="bfb14-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bfb14-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfb14-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bfb14-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bfb14-p103">O recurso **plannerGroup** oferece acesso aos recursos do Planner para um [grupo](group.md). Ele não contém quaisquer propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="bfb14-p103">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="bfb14-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="bfb14-109">Methods</span></span>

| <span data-ttu-id="bfb14-110">Método</span><span class="sxs-lookup"><span data-stu-id="bfb14-110">Method</span></span>           | <span data-ttu-id="bfb14-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bfb14-111">Return Type</span></span>    |<span data-ttu-id="bfb14-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfb14-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bfb14-113">Listar planos</span><span class="sxs-lookup"><span data-stu-id="bfb14-113">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="bfb14-114">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="bfb14-114">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="bfb14-115">Obtenha uma coleção de objetos **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="bfb14-115">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="bfb14-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bfb14-116">Properties</span></span>
| <span data-ttu-id="bfb14-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bfb14-117">Property</span></span>     | <span data-ttu-id="bfb14-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfb14-118">Type</span></span>   |<span data-ttu-id="bfb14-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfb14-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfb14-120">id</span><span class="sxs-lookup"><span data-stu-id="bfb14-120">id</span></span>|<span data-ttu-id="bfb14-121">String</span><span class="sxs-lookup"><span data-stu-id="bfb14-121">String</span></span>| <span data-ttu-id="bfb14-p104">Somente leitura. O identificador do **plannerGroup**</span><span class="sxs-lookup"><span data-stu-id="bfb14-p104">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfb14-124">Relações</span><span class="sxs-lookup"><span data-stu-id="bfb14-124">Relationships</span></span>
| <span data-ttu-id="bfb14-125">Relação</span><span class="sxs-lookup"><span data-stu-id="bfb14-125">Relationship</span></span> | <span data-ttu-id="bfb14-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfb14-126">Type</span></span>   |<span data-ttu-id="bfb14-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfb14-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfb14-128">plans</span><span class="sxs-lookup"><span data-stu-id="bfb14-128">plans</span></span>|<span data-ttu-id="bfb14-129">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="bfb14-129">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="bfb14-p105">Somente leitura. Anulável. Retorna o [plannerPlans](plannerplan.md) que pertence ao grupo.</span><span class="sxs-lookup"><span data-stu-id="bfb14-p105">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bfb14-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bfb14-133">JSON representation</span></span>
<span data-ttu-id="bfb14-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bfb14-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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