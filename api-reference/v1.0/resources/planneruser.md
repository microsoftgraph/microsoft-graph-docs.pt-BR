---
title: Tipo de recurso plannerUser
description: O recurso de **plannerUser** fornecer acesso aos recursos de Planejador de um usuário. Não contém todas as propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b73e422e232a96068f4545def0f0fdbd9f74ff07
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953546"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="d268e-104">Tipo de recurso plannerUser</span><span class="sxs-lookup"><span data-stu-id="d268e-104">plannerUser resource type</span></span>

<span data-ttu-id="d268e-p102">O recurso **plannerUser** oferece acesso aos recursos do Planner para um [usuário](user.md). Ele não contém quaisquer propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="d268e-p102">The **plannerUser** resource provide access to Planner resources for a [user](user.md). It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="d268e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d268e-107">Methods</span></span>

| <span data-ttu-id="d268e-108">Método</span><span class="sxs-lookup"><span data-stu-id="d268e-108">Method</span></span>           | <span data-ttu-id="d268e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d268e-109">Return Type</span></span>    |<span data-ttu-id="d268e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d268e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d268e-111">Listar planos</span><span class="sxs-lookup"><span data-stu-id="d268e-111">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="d268e-112">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="d268e-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d268e-113">Obtenha uma coleção de objetos **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="d268e-113">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="d268e-114">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="d268e-114">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="d268e-115">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="d268e-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d268e-116">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="d268e-116">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="d268e-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d268e-117">Properties</span></span>
| <span data-ttu-id="d268e-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d268e-118">Property</span></span>     | <span data-ttu-id="d268e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d268e-119">Type</span></span>   |<span data-ttu-id="d268e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d268e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d268e-121">id</span><span class="sxs-lookup"><span data-stu-id="d268e-121">id</span></span>|<span data-ttu-id="d268e-122">String</span><span class="sxs-lookup"><span data-stu-id="d268e-122">String</span></span>| <span data-ttu-id="d268e-p103">Somente leitura. O identificador do plannerUser</span><span class="sxs-lookup"><span data-stu-id="d268e-p103">Read-only. Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="d268e-125">Relações</span><span class="sxs-lookup"><span data-stu-id="d268e-125">Relationships</span></span>
| <span data-ttu-id="d268e-126">Relação</span><span class="sxs-lookup"><span data-stu-id="d268e-126">Relationship</span></span> | <span data-ttu-id="d268e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d268e-127">Type</span></span>   |<span data-ttu-id="d268e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d268e-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d268e-129">plans</span><span class="sxs-lookup"><span data-stu-id="d268e-129">plans</span></span>|<span data-ttu-id="d268e-130">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="d268e-130">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d268e-p104">Somente leitura. Anulável. Returna o [plannerTasks](plannertask.md) atribuídos ao usuário.</span><span class="sxs-lookup"><span data-stu-id="d268e-p104">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="d268e-134">tarefas</span><span class="sxs-lookup"><span data-stu-id="d268e-134">tasks</span></span>|<span data-ttu-id="d268e-135">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="d268e-135">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d268e-p105">Somente leitura. Anulável. Returna o objeto [plannerTasks](plannerplan.md) atribuído ao usuário.</span><span class="sxs-lookup"><span data-stu-id="d268e-p105">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d268e-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d268e-139">JSON representation</span></span>
<span data-ttu-id="d268e-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d268e-140">Here is a JSON representation of the resource.</span></span>

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
