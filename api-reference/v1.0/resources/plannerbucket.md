---
title: Tipo de recurso plannerBucket
description: ) para tarefas em um plano no Office 365. Ele está contido em um plannerPlan e pode ter uma coleção de plannerTasks.
ms.openlocfilehash: 44bce1606fa7561bc52098fe0e6ba8f70d737a58
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004473"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="ff489-104">Tipo de recurso plannerBucket</span><span class="sxs-lookup"><span data-stu-id="ff489-104">plannerBucket resource type</span></span>

<span data-ttu-id="ff489-p102">O recurso **plannerBucket** representa um Bucket (ou "coluna personalizada") para tarefas em um plano no Office 365. Ele está contido em um [plannerPlan](plannerplan.md) e pode ter uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="ff489-p102">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="ff489-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ff489-107">Methods</span></span>

| <span data-ttu-id="ff489-108">Método</span><span class="sxs-lookup"><span data-stu-id="ff489-108">Method</span></span>           | <span data-ttu-id="ff489-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ff489-109">Return Type</span></span>    |<span data-ttu-id="ff489-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff489-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff489-111">Get plannerBucket</span><span class="sxs-lookup"><span data-stu-id="ff489-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="ff489-112">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="ff489-112">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="ff489-113">Leia as propriedades e as relações do objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="ff489-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="ff489-114">Listar plannerTasks</span><span class="sxs-lookup"><span data-stu-id="ff489-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="ff489-115">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="ff489-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="ff489-116">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="ff489-116">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="ff489-117">Criar</span><span class="sxs-lookup"><span data-stu-id="ff489-117">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="ff489-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="ff489-118">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="ff489-119">Crie um novo objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="ff489-119">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="ff489-120">Update</span><span class="sxs-lookup"><span data-stu-id="ff489-120">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="ff489-121">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="ff489-121">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="ff489-122">Atualize o objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="ff489-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="ff489-123">Delete</span><span class="sxs-lookup"><span data-stu-id="ff489-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="ff489-124">None</span><span class="sxs-lookup"><span data-stu-id="ff489-124">None</span></span> |<span data-ttu-id="ff489-125">Exclua o objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="ff489-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ff489-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff489-126">Properties</span></span>
| <span data-ttu-id="ff489-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff489-127">Property</span></span>     | <span data-ttu-id="ff489-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff489-128">Type</span></span>   |<span data-ttu-id="ff489-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff489-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff489-130">id</span><span class="sxs-lookup"><span data-stu-id="ff489-130">id</span></span>|<span data-ttu-id="ff489-131">String</span><span class="sxs-lookup"><span data-stu-id="ff489-131">String</span></span>| <span data-ttu-id="ff489-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff489-132">Read-only.</span></span> <span data-ttu-id="ff489-133">ID do compartimento de memória.</span><span class="sxs-lookup"><span data-stu-id="ff489-133">ID of the bucket.</span></span> <span data-ttu-id="ff489-134">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ff489-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="ff489-135">[Validação de formato](planner-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="ff489-135">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="ff489-136">name</span><span class="sxs-lookup"><span data-stu-id="ff489-136">name</span></span>|<span data-ttu-id="ff489-137">String</span><span class="sxs-lookup"><span data-stu-id="ff489-137">String</span></span>|<span data-ttu-id="ff489-138">Nome do bucket.</span><span class="sxs-lookup"><span data-stu-id="ff489-138">Name of the bucket.</span></span>|
|<span data-ttu-id="ff489-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="ff489-139">orderHint</span></span>|<span data-ttu-id="ff489-140">String</span><span class="sxs-lookup"><span data-stu-id="ff489-140">String</span></span>|<span data-ttu-id="ff489-p104">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="ff489-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="ff489-143">planId</span><span class="sxs-lookup"><span data-stu-id="ff489-143">planId</span></span>|<span data-ttu-id="ff489-144">String</span><span class="sxs-lookup"><span data-stu-id="ff489-144">String</span></span>|<span data-ttu-id="ff489-145">ID do plano ao qual o bucket pertence.</span><span class="sxs-lookup"><span data-stu-id="ff489-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff489-146">Relações</span><span class="sxs-lookup"><span data-stu-id="ff489-146">Relationships</span></span>
| <span data-ttu-id="ff489-147">Relação</span><span class="sxs-lookup"><span data-stu-id="ff489-147">Relationship</span></span> | <span data-ttu-id="ff489-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff489-148">Type</span></span>   |<span data-ttu-id="ff489-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff489-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff489-150">tarefas</span><span class="sxs-lookup"><span data-stu-id="ff489-150">tasks</span></span>|<span data-ttu-id="ff489-151">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="ff489-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="ff489-p105">Somente leitura. Anulável. A coleção de tarefas no bucket.</span><span class="sxs-lookup"><span data-stu-id="ff489-p105">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff489-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff489-155">JSON representation</span></span>
<span data-ttu-id="ff489-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff489-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->