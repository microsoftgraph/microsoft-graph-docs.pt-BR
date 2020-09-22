---
title: tipo de recurso plannerBucket
description: ) para tarefas em um plano no Microsoft 365. Ele está contido em um plannerPlan e pode ter uma coleção de plannerTasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 02c8ef4dc25d43ee1fdd57a939bd0ed69ba86b81
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073586"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="9a863-104">tipo de recurso plannerBucket</span><span class="sxs-lookup"><span data-stu-id="9a863-104">plannerBucket resource type</span></span>

<span data-ttu-id="9a863-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a863-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a863-106">O recurso **plannerBucket** representa um Bucket (ou "coluna personalizada") para tarefas em um plano no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9a863-106">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Microsoft 365.</span></span> <span data-ttu-id="9a863-107">Ele está contido em um [plannerPlan](plannerplan.md) e pode ter uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="9a863-107">It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="9a863-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="9a863-108">Methods</span></span>

| <span data-ttu-id="9a863-109">Método</span><span class="sxs-lookup"><span data-stu-id="9a863-109">Method</span></span>           | <span data-ttu-id="9a863-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9a863-110">Return Type</span></span>    |<span data-ttu-id="9a863-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a863-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9a863-112">Obter plannerBucket</span><span class="sxs-lookup"><span data-stu-id="9a863-112">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="9a863-113">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="9a863-113">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="9a863-114">Leia as propriedades e os relacionamentos do objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="9a863-114">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="9a863-115">Listar plannerTasks</span><span class="sxs-lookup"><span data-stu-id="9a863-115">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="9a863-116">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="9a863-116">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="9a863-117">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="9a863-117">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="9a863-118">Create</span><span class="sxs-lookup"><span data-stu-id="9a863-118">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="9a863-119">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="9a863-119">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="9a863-120">Criar um novo objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="9a863-120">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="9a863-121">Update</span><span class="sxs-lookup"><span data-stu-id="9a863-121">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="9a863-122">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="9a863-122">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="9a863-123">Atualize o objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="9a863-123">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="9a863-124">Delete</span><span class="sxs-lookup"><span data-stu-id="9a863-124">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="9a863-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9a863-125">None</span></span> |<span data-ttu-id="9a863-126">Exclua o objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="9a863-126">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9a863-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a863-127">Properties</span></span>
| <span data-ttu-id="9a863-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a863-128">Property</span></span>     | <span data-ttu-id="9a863-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a863-129">Type</span></span>   |<span data-ttu-id="9a863-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a863-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a863-131">id</span><span class="sxs-lookup"><span data-stu-id="9a863-131">id</span></span>|<span data-ttu-id="9a863-132">String</span><span class="sxs-lookup"><span data-stu-id="9a863-132">String</span></span>| <span data-ttu-id="9a863-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a863-133">Read-only.</span></span> <span data-ttu-id="9a863-134">ID do Bucket.</span><span class="sxs-lookup"><span data-stu-id="9a863-134">ID of the bucket.</span></span> <span data-ttu-id="9a863-135">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9a863-135">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="9a863-136">[Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="9a863-136">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="9a863-137">name</span><span class="sxs-lookup"><span data-stu-id="9a863-137">name</span></span>|<span data-ttu-id="9a863-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a863-138">String</span></span>|<span data-ttu-id="9a863-139">Nome do bucket.</span><span class="sxs-lookup"><span data-stu-id="9a863-139">Name of the bucket.</span></span>|
|<span data-ttu-id="9a863-140">orderHint</span><span class="sxs-lookup"><span data-stu-id="9a863-140">orderHint</span></span>|<span data-ttu-id="9a863-141">String</span><span class="sxs-lookup"><span data-stu-id="9a863-141">String</span></span>|<span data-ttu-id="9a863-p104">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="9a863-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="9a863-144">planId</span><span class="sxs-lookup"><span data-stu-id="9a863-144">planId</span></span>|<span data-ttu-id="9a863-145">String</span><span class="sxs-lookup"><span data-stu-id="9a863-145">String</span></span>|<span data-ttu-id="9a863-146">ID do plano ao qual o Bucket pertence.</span><span class="sxs-lookup"><span data-stu-id="9a863-146">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a863-147">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="9a863-147">Relationships</span></span>
| <span data-ttu-id="9a863-148">Relação</span><span class="sxs-lookup"><span data-stu-id="9a863-148">Relationship</span></span> | <span data-ttu-id="9a863-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a863-149">Type</span></span>   |<span data-ttu-id="9a863-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a863-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a863-151">tarefas</span><span class="sxs-lookup"><span data-stu-id="9a863-151">tasks</span></span>|<span data-ttu-id="9a863-152">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="9a863-152">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="9a863-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a863-153">Read-only.</span></span> <span data-ttu-id="9a863-154">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9a863-154">Nullable.</span></span> <span data-ttu-id="9a863-155">A coleção de tarefas no Bucket.</span><span class="sxs-lookup"><span data-stu-id="9a863-155">The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a863-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a863-156">JSON representation</span></span>
<span data-ttu-id="9a863-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a863-157">Here is a JSON representation of the resource.</span></span>

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


