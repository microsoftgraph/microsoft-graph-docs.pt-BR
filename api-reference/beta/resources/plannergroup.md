---
title: Tipo de recurso plannerGroup
description: O recurso **plannerGroup** oferece acesso aos recursos do Planner para um grupo. Ele não contém quaisquer propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 84bb20d0b13f9a99db2f8c59b20e0c9c7c87f93f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513778"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="62ff9-104">Tipo de recurso plannerGroup</span><span class="sxs-lookup"><span data-stu-id="62ff9-104">plannerGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62ff9-p102">O recurso **plannerGroup** oferece acesso aos recursos do Planner para um [grupo](group.md). Ele não contém quaisquer propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="62ff9-p102">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="62ff9-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="62ff9-107">Methods</span></span>

| <span data-ttu-id="62ff9-108">Método</span><span class="sxs-lookup"><span data-stu-id="62ff9-108">Method</span></span>           | <span data-ttu-id="62ff9-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="62ff9-109">Return Type</span></span>    |<span data-ttu-id="62ff9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="62ff9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="62ff9-111">Listar planos</span><span class="sxs-lookup"><span data-stu-id="62ff9-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="62ff9-112">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="62ff9-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="62ff9-113">Obtenha uma coleção de objetos **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="62ff9-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="62ff9-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62ff9-114">Properties</span></span>
| <span data-ttu-id="62ff9-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62ff9-115">Property</span></span>     | <span data-ttu-id="62ff9-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="62ff9-116">Type</span></span>   |<span data-ttu-id="62ff9-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="62ff9-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62ff9-118">id</span><span class="sxs-lookup"><span data-stu-id="62ff9-118">id</span></span>|<span data-ttu-id="62ff9-119">String</span><span class="sxs-lookup"><span data-stu-id="62ff9-119">String</span></span>| <span data-ttu-id="62ff9-p103">Somente leitura. O identificador do **plannerGroup**</span><span class="sxs-lookup"><span data-stu-id="62ff9-p103">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="62ff9-122">Relações</span><span class="sxs-lookup"><span data-stu-id="62ff9-122">Relationships</span></span>
| <span data-ttu-id="62ff9-123">Relação</span><span class="sxs-lookup"><span data-stu-id="62ff9-123">Relationship</span></span> | <span data-ttu-id="62ff9-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="62ff9-124">Type</span></span>   |<span data-ttu-id="62ff9-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="62ff9-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62ff9-126">plans</span><span class="sxs-lookup"><span data-stu-id="62ff9-126">plans</span></span>|<span data-ttu-id="62ff9-127">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="62ff9-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="62ff9-p104">Somente leitura. Anulável. Retorna o [plannerPlans](plannerplan.md) que pertence ao grupo.</span><span class="sxs-lookup"><span data-stu-id="62ff9-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62ff9-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62ff9-131">JSON representation</span></span>
<span data-ttu-id="62ff9-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62ff9-132">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannergroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
