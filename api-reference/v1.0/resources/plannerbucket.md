---
title: Tipo de recurso plannerBucket
description: ) para tarefas em um plano no Office 365. Ele está contido em um plannerPlan e pode ter uma coleção de plannerTasks.
author: TarkanSevilmis
localization_priority: Normal
ms.openlocfilehash: 592d0e24f527d7ae343bd29e71a3dfdf0247720f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831455"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="fa0f4-104">Tipo de recurso plannerBucket</span><span class="sxs-lookup"><span data-stu-id="fa0f4-104">plannerBucket resource type</span></span>

<span data-ttu-id="fa0f4-p102">O recurso **plannerBucket** representa um Bucket (ou "coluna personalizada") para tarefas em um plano no Office 365. Ele está contido em um [plannerPlan](plannerplan.md) e pode ter uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="fa0f4-p102">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="fa0f4-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="fa0f4-107">Methods</span></span>

| <span data-ttu-id="fa0f4-108">Método</span><span class="sxs-lookup"><span data-stu-id="fa0f4-108">Method</span></span>           | <span data-ttu-id="fa0f4-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fa0f4-109">Return Type</span></span>    |<span data-ttu-id="fa0f4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa0f4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fa0f4-111">Get plannerBucket</span><span class="sxs-lookup"><span data-stu-id="fa0f4-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="fa0f4-112">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="fa0f4-112">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="fa0f4-113">Leia as propriedades e as relações do objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="fa0f4-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="fa0f4-114">Listar plannerTasks</span><span class="sxs-lookup"><span data-stu-id="fa0f4-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="fa0f4-115">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="fa0f4-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="fa0f4-116">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="fa0f4-116">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="fa0f4-117">Criar</span><span class="sxs-lookup"><span data-stu-id="fa0f4-117">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="fa0f4-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="fa0f4-118">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="fa0f4-119">Crie um novo objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="fa0f4-119">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="fa0f4-120">Update</span><span class="sxs-lookup"><span data-stu-id="fa0f4-120">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="fa0f4-121">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="fa0f4-121">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="fa0f4-122">Atualize o objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="fa0f4-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="fa0f4-123">Delete</span><span class="sxs-lookup"><span data-stu-id="fa0f4-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="fa0f4-124">None</span><span class="sxs-lookup"><span data-stu-id="fa0f4-124">None</span></span> |<span data-ttu-id="fa0f4-125">Exclua o objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="fa0f4-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fa0f4-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa0f4-126">Properties</span></span>
| <span data-ttu-id="fa0f4-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa0f4-127">Property</span></span>     | <span data-ttu-id="fa0f4-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa0f4-128">Type</span></span>   |<span data-ttu-id="fa0f4-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa0f4-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa0f4-130">id</span><span class="sxs-lookup"><span data-stu-id="fa0f4-130">id</span></span>|<span data-ttu-id="fa0f4-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa0f4-131">String</span></span>| <span data-ttu-id="fa0f4-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fa0f4-132">Read-only.</span></span> <span data-ttu-id="fa0f4-133">ID do compartimento de memória.</span><span class="sxs-lookup"><span data-stu-id="fa0f4-133">ID of the bucket.</span></span> <span data-ttu-id="fa0f4-134">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="fa0f4-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="fa0f4-135">[Validação de formato](planner-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="fa0f4-135">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="fa0f4-136">name</span><span class="sxs-lookup"><span data-stu-id="fa0f4-136">name</span></span>|<span data-ttu-id="fa0f4-137">String</span><span class="sxs-lookup"><span data-stu-id="fa0f4-137">String</span></span>|<span data-ttu-id="fa0f4-138">Nome do bucket.</span><span class="sxs-lookup"><span data-stu-id="fa0f4-138">Name of the bucket.</span></span>|
|<span data-ttu-id="fa0f4-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="fa0f4-139">orderHint</span></span>|<span data-ttu-id="fa0f4-140">String</span><span class="sxs-lookup"><span data-stu-id="fa0f4-140">String</span></span>|<span data-ttu-id="fa0f4-p104">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="fa0f4-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="fa0f4-143">planId</span><span class="sxs-lookup"><span data-stu-id="fa0f4-143">planId</span></span>|<span data-ttu-id="fa0f4-144">String</span><span class="sxs-lookup"><span data-stu-id="fa0f4-144">String</span></span>|<span data-ttu-id="fa0f4-145">ID do plano ao qual o bucket pertence.</span><span class="sxs-lookup"><span data-stu-id="fa0f4-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa0f4-146">Relações</span><span class="sxs-lookup"><span data-stu-id="fa0f4-146">Relationships</span></span>
| <span data-ttu-id="fa0f4-147">Relação</span><span class="sxs-lookup"><span data-stu-id="fa0f4-147">Relationship</span></span> | <span data-ttu-id="fa0f4-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa0f4-148">Type</span></span>   |<span data-ttu-id="fa0f4-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa0f4-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa0f4-150">tarefas</span><span class="sxs-lookup"><span data-stu-id="fa0f4-150">tasks</span></span>|<span data-ttu-id="fa0f4-151">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="fa0f4-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="fa0f4-p105">Somente leitura. Anulável. A coleção de tarefas no bucket.</span><span class="sxs-lookup"><span data-stu-id="fa0f4-p105">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa0f4-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa0f4-155">JSON representation</span></span>
<span data-ttu-id="fa0f4-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa0f4-156">Here is a JSON representation of the resource.</span></span>

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
