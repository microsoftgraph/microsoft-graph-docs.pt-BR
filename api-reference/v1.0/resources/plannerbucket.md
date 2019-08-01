---
title: tipo de recurso plannerBucket
description: ) para tarefas em um plano no Office 365. Ele está contido em um plannerPlan e pode ter uma coleção de plannerTasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b6810a62ecab5209ca1c17aa7f3ca9e4753a50a9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035319"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="c0576-104">tipo de recurso plannerBucket</span><span class="sxs-lookup"><span data-stu-id="c0576-104">plannerBucket resource type</span></span>

<span data-ttu-id="c0576-105">O recurso **plannerBucket** representa um Bucket (ou "coluna personalizada") para tarefas em um plano no Office 365.</span><span class="sxs-lookup"><span data-stu-id="c0576-105">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365.</span></span> <span data-ttu-id="c0576-106">Ele está contido em um [plannerPlan](plannerplan.md) e pode ter uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="c0576-106">It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="c0576-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c0576-107">Methods</span></span>

| <span data-ttu-id="c0576-108">Método</span><span class="sxs-lookup"><span data-stu-id="c0576-108">Method</span></span>           | <span data-ttu-id="c0576-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c0576-109">Return Type</span></span>    |<span data-ttu-id="c0576-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0576-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c0576-111">Obter plannerBucket</span><span class="sxs-lookup"><span data-stu-id="c0576-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="c0576-112">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="c0576-112">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="c0576-113">Leia as propriedades e os relacionamentos do objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="c0576-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="c0576-114">Listar plannerTasks</span><span class="sxs-lookup"><span data-stu-id="c0576-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="c0576-115">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="c0576-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="c0576-116">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="c0576-116">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="c0576-117">Create</span><span class="sxs-lookup"><span data-stu-id="c0576-117">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="c0576-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="c0576-118">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="c0576-119">Criar um novo objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="c0576-119">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="c0576-120">Atualização</span><span class="sxs-lookup"><span data-stu-id="c0576-120">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="c0576-121">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="c0576-121">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="c0576-122">Atualize o objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="c0576-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="c0576-123">Delete</span><span class="sxs-lookup"><span data-stu-id="c0576-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="c0576-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c0576-124">None</span></span> |<span data-ttu-id="c0576-125">Exclua o objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="c0576-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c0576-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0576-126">Properties</span></span>
| <span data-ttu-id="c0576-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0576-127">Property</span></span>     | <span data-ttu-id="c0576-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0576-128">Type</span></span>   |<span data-ttu-id="c0576-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0576-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0576-130">id</span><span class="sxs-lookup"><span data-stu-id="c0576-130">id</span></span>|<span data-ttu-id="c0576-131">String</span><span class="sxs-lookup"><span data-stu-id="c0576-131">String</span></span>| <span data-ttu-id="c0576-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c0576-132">Read-only.</span></span> <span data-ttu-id="c0576-133">ID do Bucket.</span><span class="sxs-lookup"><span data-stu-id="c0576-133">ID of the bucket.</span></span> <span data-ttu-id="c0576-134">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="c0576-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="c0576-135">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="c0576-135">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="c0576-136">name</span><span class="sxs-lookup"><span data-stu-id="c0576-136">name</span></span>|<span data-ttu-id="c0576-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0576-137">String</span></span>|<span data-ttu-id="c0576-138">Nome do Bucket.</span><span class="sxs-lookup"><span data-stu-id="c0576-138">Name of the bucket.</span></span>|
|<span data-ttu-id="c0576-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="c0576-139">orderHint</span></span>|<span data-ttu-id="c0576-140">String</span><span class="sxs-lookup"><span data-stu-id="c0576-140">String</span></span>|<span data-ttu-id="c0576-p104">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="c0576-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="c0576-143">planId</span><span class="sxs-lookup"><span data-stu-id="c0576-143">planId</span></span>|<span data-ttu-id="c0576-144">String</span><span class="sxs-lookup"><span data-stu-id="c0576-144">String</span></span>|<span data-ttu-id="c0576-145">ID do plano ao qual o Bucket pertence.</span><span class="sxs-lookup"><span data-stu-id="c0576-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0576-146">Relações</span><span class="sxs-lookup"><span data-stu-id="c0576-146">Relationships</span></span>
| <span data-ttu-id="c0576-147">Relação</span><span class="sxs-lookup"><span data-stu-id="c0576-147">Relationship</span></span> | <span data-ttu-id="c0576-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0576-148">Type</span></span>   |<span data-ttu-id="c0576-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0576-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0576-150">tarefas</span><span class="sxs-lookup"><span data-stu-id="c0576-150">tasks</span></span>|<span data-ttu-id="c0576-151">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="c0576-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="c0576-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c0576-152">Read-only.</span></span> <span data-ttu-id="c0576-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c0576-153">Nullable.</span></span> <span data-ttu-id="c0576-154">A coleção de tarefas no Bucket.</span><span class="sxs-lookup"><span data-stu-id="c0576-154">The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0576-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0576-155">JSON representation</span></span>
<span data-ttu-id="c0576-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0576-156">Here is a JSON representation of the resource.</span></span>

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
