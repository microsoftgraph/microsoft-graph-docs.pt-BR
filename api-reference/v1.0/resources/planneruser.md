---
title: Tipo de recurso plannerUser
description: O recurso de **plannerUser** fornecer acesso aos recursos de Planejador de um usuário. Não contém todas as propriedades utilizáveis.
ms.openlocfilehash: 777886a61d702198ec03ea844fb9fced761047ba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005524"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="21b17-104">Tipo de recurso plannerUser</span><span class="sxs-lookup"><span data-stu-id="21b17-104">plannerUser resource type</span></span>

<span data-ttu-id="21b17-p102">O recurso **plannerUser** oferece acesso aos recursos do Planner para um [usuário](user.md). Ele não contém quaisquer propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="21b17-p102">The **plannerUser** resource provide access to Planner resources for a [user](user.md). It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="21b17-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="21b17-107">Methods</span></span>

| <span data-ttu-id="21b17-108">Método</span><span class="sxs-lookup"><span data-stu-id="21b17-108">Method</span></span>           | <span data-ttu-id="21b17-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="21b17-109">Return Type</span></span>    |<span data-ttu-id="21b17-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="21b17-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="21b17-111">Listar planos</span><span class="sxs-lookup"><span data-stu-id="21b17-111">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="21b17-112">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="21b17-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="21b17-113">Obtenha uma coleção de objetos **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="21b17-113">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="21b17-114">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="21b17-114">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="21b17-115">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="21b17-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="21b17-116">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="21b17-116">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="21b17-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21b17-117">Properties</span></span>
| <span data-ttu-id="21b17-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21b17-118">Property</span></span>     | <span data-ttu-id="21b17-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="21b17-119">Type</span></span>   |<span data-ttu-id="21b17-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="21b17-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21b17-121">id</span><span class="sxs-lookup"><span data-stu-id="21b17-121">id</span></span>|<span data-ttu-id="21b17-122">String</span><span class="sxs-lookup"><span data-stu-id="21b17-122">String</span></span>| <span data-ttu-id="21b17-p103">Somente leitura. O identificador do plannerUser</span><span class="sxs-lookup"><span data-stu-id="21b17-p103">Read-only. Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="21b17-125">Relações</span><span class="sxs-lookup"><span data-stu-id="21b17-125">Relationships</span></span>
| <span data-ttu-id="21b17-126">Relação</span><span class="sxs-lookup"><span data-stu-id="21b17-126">Relationship</span></span> | <span data-ttu-id="21b17-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="21b17-127">Type</span></span>   |<span data-ttu-id="21b17-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="21b17-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21b17-129">plans</span><span class="sxs-lookup"><span data-stu-id="21b17-129">plans</span></span>|<span data-ttu-id="21b17-130">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="21b17-130">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="21b17-p104">Somente leitura. Anulável. Returna o [plannerTasks](plannertask.md) atribuídos ao usuário.</span><span class="sxs-lookup"><span data-stu-id="21b17-p104">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="21b17-134">tarefas</span><span class="sxs-lookup"><span data-stu-id="21b17-134">tasks</span></span>|<span data-ttu-id="21b17-135">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="21b17-135">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="21b17-p105">Somente leitura. Anulável. Returna o objeto [plannerTasks](plannerplan.md) atribuído ao usuário.</span><span class="sxs-lookup"><span data-stu-id="21b17-p105">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21b17-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21b17-139">JSON representation</span></span>
<span data-ttu-id="21b17-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21b17-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
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
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->