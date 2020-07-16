---
title: tipo de recurso plannerBucket
description: ) para tarefas em um plano no Microsoft 365. Ele está contido em um plannerPlan e pode ter uma coleção de plannerTasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 33ce6a6be827510b522359ac93a77d1f0b74b477
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897047"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="3d569-104">tipo de recurso plannerBucket</span><span class="sxs-lookup"><span data-stu-id="3d569-104">plannerBucket resource type</span></span>

<span data-ttu-id="3d569-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d569-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d569-106">O recurso **plannerBucket** representa um Bucket (ou "coluna personalizada") para tarefas em um plano no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3d569-106">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Microsoft 365.</span></span> <span data-ttu-id="3d569-107">Ele está contido em um [plannerPlan](plannerplan.md) e pode ter uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="3d569-107">It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="3d569-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="3d569-108">Methods</span></span>

| <span data-ttu-id="3d569-109">Método</span><span class="sxs-lookup"><span data-stu-id="3d569-109">Method</span></span>           | <span data-ttu-id="3d569-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3d569-110">Return Type</span></span>    |<span data-ttu-id="3d569-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d569-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3d569-112">Obter plannerBucket</span><span class="sxs-lookup"><span data-stu-id="3d569-112">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="3d569-113">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="3d569-113">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="3d569-114">Leia as propriedades e os relacionamentos do objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="3d569-114">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="3d569-115">Listar plannerTasks</span><span class="sxs-lookup"><span data-stu-id="3d569-115">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="3d569-116">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="3d569-116">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="3d569-117">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="3d569-117">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="3d569-118">Criar</span><span class="sxs-lookup"><span data-stu-id="3d569-118">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="3d569-119">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="3d569-119">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="3d569-120">Criar um novo objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="3d569-120">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="3d569-121">Update</span><span class="sxs-lookup"><span data-stu-id="3d569-121">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="3d569-122">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="3d569-122">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="3d569-123">Atualize o objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="3d569-123">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="3d569-124">Delete</span><span class="sxs-lookup"><span data-stu-id="3d569-124">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="3d569-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d569-125">None</span></span> |<span data-ttu-id="3d569-126">Exclua o objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="3d569-126">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3d569-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d569-127">Properties</span></span>
| <span data-ttu-id="3d569-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d569-128">Property</span></span>     | <span data-ttu-id="3d569-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d569-129">Type</span></span>   |<span data-ttu-id="3d569-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d569-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d569-131">id</span><span class="sxs-lookup"><span data-stu-id="3d569-131">id</span></span>|<span data-ttu-id="3d569-132">String</span><span class="sxs-lookup"><span data-stu-id="3d569-132">String</span></span>| <span data-ttu-id="3d569-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d569-133">Read-only.</span></span> <span data-ttu-id="3d569-134">ID do Bucket.</span><span class="sxs-lookup"><span data-stu-id="3d569-134">ID of the bucket.</span></span> <span data-ttu-id="3d569-135">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="3d569-135">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="3d569-136">[Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="3d569-136">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="3d569-137">nome</span><span class="sxs-lookup"><span data-stu-id="3d569-137">name</span></span>|<span data-ttu-id="3d569-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d569-138">String</span></span>|<span data-ttu-id="3d569-139">Nome do bucket.</span><span class="sxs-lookup"><span data-stu-id="3d569-139">Name of the bucket.</span></span>|
|<span data-ttu-id="3d569-140">orderHint</span><span class="sxs-lookup"><span data-stu-id="3d569-140">orderHint</span></span>|<span data-ttu-id="3d569-141">String</span><span class="sxs-lookup"><span data-stu-id="3d569-141">String</span></span>|<span data-ttu-id="3d569-p104">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="3d569-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="3d569-144">planId</span><span class="sxs-lookup"><span data-stu-id="3d569-144">planId</span></span>|<span data-ttu-id="3d569-145">String</span><span class="sxs-lookup"><span data-stu-id="3d569-145">String</span></span>|<span data-ttu-id="3d569-146">ID do plano ao qual o Bucket pertence.</span><span class="sxs-lookup"><span data-stu-id="3d569-146">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d569-147">Relações</span><span class="sxs-lookup"><span data-stu-id="3d569-147">Relationships</span></span>
| <span data-ttu-id="3d569-148">Relação</span><span class="sxs-lookup"><span data-stu-id="3d569-148">Relationship</span></span> | <span data-ttu-id="3d569-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d569-149">Type</span></span>   |<span data-ttu-id="3d569-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d569-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d569-151">tarefas</span><span class="sxs-lookup"><span data-stu-id="3d569-151">tasks</span></span>|<span data-ttu-id="3d569-152">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="3d569-152">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="3d569-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d569-153">Read-only.</span></span> <span data-ttu-id="3d569-154">Anulável.</span><span class="sxs-lookup"><span data-stu-id="3d569-154">Nullable.</span></span> <span data-ttu-id="3d569-155">A coleção de tarefas no Bucket.</span><span class="sxs-lookup"><span data-stu-id="3d569-155">The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d569-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d569-156">JSON representation</span></span>
<span data-ttu-id="3d569-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d569-157">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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
  "suppressions": []
}
-->
