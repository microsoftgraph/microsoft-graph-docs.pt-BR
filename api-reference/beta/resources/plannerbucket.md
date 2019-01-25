---
title: Tipo de recurso plannerBucket
description: ) para tarefas em um plano no Office 365. Ele está contido em um plannerPlan e pode ter uma coleção de plannerTasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 85cf30bc13b3236928e662807a144f81614adbd7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524454"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="e2698-104">Tipo de recurso plannerBucket</span><span class="sxs-lookup"><span data-stu-id="e2698-104">plannerBucket resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2698-p102">O recurso **plannerBucket** representa um Bucket (ou "coluna personalizada") para tarefas em um plano no Office 365. Ele está contido em um [plannerPlan](plannerplan.md) e pode ter uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="e2698-p102">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="e2698-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e2698-107">Methods</span></span>

| <span data-ttu-id="e2698-108">Método</span><span class="sxs-lookup"><span data-stu-id="e2698-108">Method</span></span>           | <span data-ttu-id="e2698-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e2698-109">Return Type</span></span>    |<span data-ttu-id="e2698-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2698-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e2698-111">Get plannerBucket</span><span class="sxs-lookup"><span data-stu-id="e2698-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="e2698-112">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="e2698-112">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="e2698-113">Leia as propriedades e as relações do objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="e2698-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="e2698-114">Listar plannerTasks</span><span class="sxs-lookup"><span data-stu-id="e2698-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="e2698-115">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="e2698-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="e2698-116">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="e2698-116">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="e2698-117">Criar</span><span class="sxs-lookup"><span data-stu-id="e2698-117">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="e2698-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="e2698-118">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="e2698-119">Crie um novo objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="e2698-119">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="e2698-120">Update</span><span class="sxs-lookup"><span data-stu-id="e2698-120">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="e2698-121">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="e2698-121">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="e2698-122">Atualize o objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="e2698-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="e2698-123">Delete</span><span class="sxs-lookup"><span data-stu-id="e2698-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="e2698-124">None</span><span class="sxs-lookup"><span data-stu-id="e2698-124">None</span></span> |<span data-ttu-id="e2698-125">Exclua o objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="e2698-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e2698-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2698-126">Properties</span></span>
| <span data-ttu-id="e2698-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2698-127">Property</span></span>     | <span data-ttu-id="e2698-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2698-128">Type</span></span>   |<span data-ttu-id="e2698-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2698-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2698-130">id</span><span class="sxs-lookup"><span data-stu-id="e2698-130">id</span></span>|<span data-ttu-id="e2698-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2698-131">String</span></span>| <span data-ttu-id="e2698-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e2698-132">Read-only.</span></span> <span data-ttu-id="e2698-133">ID do compartimento de memória.</span><span class="sxs-lookup"><span data-stu-id="e2698-133">ID of the bucket.</span></span> <span data-ttu-id="e2698-134">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="e2698-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="e2698-135">[Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="e2698-135">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="e2698-136">name</span><span class="sxs-lookup"><span data-stu-id="e2698-136">name</span></span>|<span data-ttu-id="e2698-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2698-137">String</span></span>|<span data-ttu-id="e2698-138">Nome do bucket.</span><span class="sxs-lookup"><span data-stu-id="e2698-138">Name of the bucket.</span></span>|
|<span data-ttu-id="e2698-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="e2698-139">orderHint</span></span>|<span data-ttu-id="e2698-140">String</span><span class="sxs-lookup"><span data-stu-id="e2698-140">String</span></span>|<span data-ttu-id="e2698-p104">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="e2698-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="e2698-143">planId</span><span class="sxs-lookup"><span data-stu-id="e2698-143">planId</span></span>|<span data-ttu-id="e2698-144">String</span><span class="sxs-lookup"><span data-stu-id="e2698-144">String</span></span>|<span data-ttu-id="e2698-145">ID do plano ao qual o bucket pertence.</span><span class="sxs-lookup"><span data-stu-id="e2698-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2698-146">Relações</span><span class="sxs-lookup"><span data-stu-id="e2698-146">Relationships</span></span>
| <span data-ttu-id="e2698-147">Relação</span><span class="sxs-lookup"><span data-stu-id="e2698-147">Relationship</span></span> | <span data-ttu-id="e2698-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2698-148">Type</span></span>   |<span data-ttu-id="e2698-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2698-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2698-150">tarefas</span><span class="sxs-lookup"><span data-stu-id="e2698-150">tasks</span></span>|<span data-ttu-id="e2698-151">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="e2698-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="e2698-p105">Somente leitura. Anulável. A coleção de tarefas no bucket.</span><span class="sxs-lookup"><span data-stu-id="e2698-p105">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2698-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2698-155">JSON representation</span></span>
<span data-ttu-id="e2698-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2698-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerbucket.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
