---
title: tipo de recurso plannerBucket
description: ) para tarefas em um plano no Office 365. Ele está contido em um plannerPlan e pode ter uma coleção de plannerTasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 40dc49363e4214c044c408760007a46b8f65ea46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447147"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="ed16a-104">tipo de recurso plannerBucket</span><span class="sxs-lookup"><span data-stu-id="ed16a-104">plannerBucket resource type</span></span>

<span data-ttu-id="ed16a-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ed16a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed16a-106">O recurso **plannerBucket** representa um Bucket (ou "coluna personalizada") para tarefas em um plano no Office 365.</span><span class="sxs-lookup"><span data-stu-id="ed16a-106">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365.</span></span> <span data-ttu-id="ed16a-107">Ele está contido em um [plannerPlan](plannerplan.md) e pode ter uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="ed16a-107">It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="ed16a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="ed16a-108">Methods</span></span>

| <span data-ttu-id="ed16a-109">Método</span><span class="sxs-lookup"><span data-stu-id="ed16a-109">Method</span></span>           | <span data-ttu-id="ed16a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ed16a-110">Return Type</span></span>    |<span data-ttu-id="ed16a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed16a-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ed16a-112">Obter plannerBucket</span><span class="sxs-lookup"><span data-stu-id="ed16a-112">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="ed16a-113">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="ed16a-113">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="ed16a-114">Leia as propriedades e os relacionamentos do objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="ed16a-114">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="ed16a-115">Listar plannerTasks</span><span class="sxs-lookup"><span data-stu-id="ed16a-115">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="ed16a-116">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="ed16a-116">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="ed16a-117">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="ed16a-117">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="ed16a-118">Create</span><span class="sxs-lookup"><span data-stu-id="ed16a-118">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="ed16a-119">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="ed16a-119">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="ed16a-120">Criar um novo objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="ed16a-120">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="ed16a-121">Update</span><span class="sxs-lookup"><span data-stu-id="ed16a-121">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="ed16a-122">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="ed16a-122">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="ed16a-123">Atualize o objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="ed16a-123">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="ed16a-124">Delete</span><span class="sxs-lookup"><span data-stu-id="ed16a-124">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="ed16a-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed16a-125">None</span></span> |<span data-ttu-id="ed16a-126">Exclua o objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="ed16a-126">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ed16a-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed16a-127">Properties</span></span>
| <span data-ttu-id="ed16a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed16a-128">Property</span></span>     | <span data-ttu-id="ed16a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed16a-129">Type</span></span>   |<span data-ttu-id="ed16a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed16a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed16a-131">id</span><span class="sxs-lookup"><span data-stu-id="ed16a-131">id</span></span>|<span data-ttu-id="ed16a-132">String</span><span class="sxs-lookup"><span data-stu-id="ed16a-132">String</span></span>| <span data-ttu-id="ed16a-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed16a-133">Read-only.</span></span> <span data-ttu-id="ed16a-134">ID do Bucket.</span><span class="sxs-lookup"><span data-stu-id="ed16a-134">ID of the bucket.</span></span> <span data-ttu-id="ed16a-135">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ed16a-135">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="ed16a-136">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="ed16a-136">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="ed16a-137">nome</span><span class="sxs-lookup"><span data-stu-id="ed16a-137">name</span></span>|<span data-ttu-id="ed16a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed16a-138">String</span></span>|<span data-ttu-id="ed16a-139">Nome do bucket.</span><span class="sxs-lookup"><span data-stu-id="ed16a-139">Name of the bucket.</span></span>|
|<span data-ttu-id="ed16a-140">orderHint</span><span class="sxs-lookup"><span data-stu-id="ed16a-140">orderHint</span></span>|<span data-ttu-id="ed16a-141">String</span><span class="sxs-lookup"><span data-stu-id="ed16a-141">String</span></span>|<span data-ttu-id="ed16a-p104">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="ed16a-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="ed16a-144">planId</span><span class="sxs-lookup"><span data-stu-id="ed16a-144">planId</span></span>|<span data-ttu-id="ed16a-145">String</span><span class="sxs-lookup"><span data-stu-id="ed16a-145">String</span></span>|<span data-ttu-id="ed16a-146">ID do plano ao qual o Bucket pertence.</span><span class="sxs-lookup"><span data-stu-id="ed16a-146">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed16a-147">Relações</span><span class="sxs-lookup"><span data-stu-id="ed16a-147">Relationships</span></span>
| <span data-ttu-id="ed16a-148">Relação</span><span class="sxs-lookup"><span data-stu-id="ed16a-148">Relationship</span></span> | <span data-ttu-id="ed16a-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed16a-149">Type</span></span>   |<span data-ttu-id="ed16a-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed16a-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed16a-151">tarefas</span><span class="sxs-lookup"><span data-stu-id="ed16a-151">tasks</span></span>|<span data-ttu-id="ed16a-152">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="ed16a-152">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="ed16a-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed16a-153">Read-only.</span></span> <span data-ttu-id="ed16a-154">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ed16a-154">Nullable.</span></span> <span data-ttu-id="ed16a-155">A coleção de tarefas no Bucket.</span><span class="sxs-lookup"><span data-stu-id="ed16a-155">The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed16a-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed16a-156">JSON representation</span></span>
<span data-ttu-id="ed16a-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed16a-157">Here is a JSON representation of the resource.</span></span>

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
