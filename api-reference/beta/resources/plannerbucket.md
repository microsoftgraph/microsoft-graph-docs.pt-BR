---
title: Tipo de recurso plannerBucket
description: ) para tarefas em um plano no Office 365. Ele está contido em um plannerPlan e pode ter uma coleção de plannerTasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 4ed1cbe51ca22fbabce6dfd030747e728299190f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929708"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="5b34f-104">Tipo de recurso plannerBucket</span><span class="sxs-lookup"><span data-stu-id="5b34f-104">plannerBucket resource type</span></span>

> <span data-ttu-id="5b34f-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5b34f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b34f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5b34f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b34f-p103">O recurso **plannerBucket** representa um Bucket (ou "coluna personalizada") para tarefas em um plano no Office 365. Ele está contido em um [plannerPlan](plannerplan.md) e pode ter uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="5b34f-p103">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="5b34f-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="5b34f-109">Methods</span></span>

| <span data-ttu-id="5b34f-110">Método</span><span class="sxs-lookup"><span data-stu-id="5b34f-110">Method</span></span>           | <span data-ttu-id="5b34f-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5b34f-111">Return Type</span></span>    |<span data-ttu-id="5b34f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b34f-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5b34f-113">Get plannerBucket</span><span class="sxs-lookup"><span data-stu-id="5b34f-113">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="5b34f-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="5b34f-114">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="5b34f-115">Leia as propriedades e as relações do objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="5b34f-115">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="5b34f-116">Listar plannerTasks</span><span class="sxs-lookup"><span data-stu-id="5b34f-116">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="5b34f-117">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="5b34f-117">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="5b34f-118">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="5b34f-118">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="5b34f-119">Criar</span><span class="sxs-lookup"><span data-stu-id="5b34f-119">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="5b34f-120">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="5b34f-120">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="5b34f-121">Crie um novo objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="5b34f-121">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="5b34f-122">Update</span><span class="sxs-lookup"><span data-stu-id="5b34f-122">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="5b34f-123">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="5b34f-123">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="5b34f-124">Atualize o objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="5b34f-124">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="5b34f-125">Delete</span><span class="sxs-lookup"><span data-stu-id="5b34f-125">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="5b34f-126">None</span><span class="sxs-lookup"><span data-stu-id="5b34f-126">None</span></span> |<span data-ttu-id="5b34f-127">Exclua o objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="5b34f-127">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5b34f-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b34f-128">Properties</span></span>
| <span data-ttu-id="5b34f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b34f-129">Property</span></span>     | <span data-ttu-id="5b34f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b34f-130">Type</span></span>   |<span data-ttu-id="5b34f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b34f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b34f-132">id</span><span class="sxs-lookup"><span data-stu-id="5b34f-132">id</span></span>|<span data-ttu-id="5b34f-133">String</span><span class="sxs-lookup"><span data-stu-id="5b34f-133">String</span></span>| <span data-ttu-id="5b34f-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b34f-134">Read-only.</span></span> <span data-ttu-id="5b34f-135">ID do compartimento de memória.</span><span class="sxs-lookup"><span data-stu-id="5b34f-135">ID of the bucket.</span></span> <span data-ttu-id="5b34f-136">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="5b34f-136">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="5b34f-137">[Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="5b34f-137">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="5b34f-138">name</span><span class="sxs-lookup"><span data-stu-id="5b34f-138">name</span></span>|<span data-ttu-id="5b34f-139">String</span><span class="sxs-lookup"><span data-stu-id="5b34f-139">String</span></span>|<span data-ttu-id="5b34f-140">Nome do bucket.</span><span class="sxs-lookup"><span data-stu-id="5b34f-140">Name of the bucket.</span></span>|
|<span data-ttu-id="5b34f-141">orderHint</span><span class="sxs-lookup"><span data-stu-id="5b34f-141">orderHint</span></span>|<span data-ttu-id="5b34f-142">String</span><span class="sxs-lookup"><span data-stu-id="5b34f-142">String</span></span>|<span data-ttu-id="5b34f-p105">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="5b34f-p105">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="5b34f-145">planId</span><span class="sxs-lookup"><span data-stu-id="5b34f-145">planId</span></span>|<span data-ttu-id="5b34f-146">String</span><span class="sxs-lookup"><span data-stu-id="5b34f-146">String</span></span>|<span data-ttu-id="5b34f-147">ID do plano ao qual o bucket pertence.</span><span class="sxs-lookup"><span data-stu-id="5b34f-147">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b34f-148">Relações</span><span class="sxs-lookup"><span data-stu-id="5b34f-148">Relationships</span></span>
| <span data-ttu-id="5b34f-149">Relação</span><span class="sxs-lookup"><span data-stu-id="5b34f-149">Relationship</span></span> | <span data-ttu-id="5b34f-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b34f-150">Type</span></span>   |<span data-ttu-id="5b34f-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b34f-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b34f-152">tarefas</span><span class="sxs-lookup"><span data-stu-id="5b34f-152">tasks</span></span>|<span data-ttu-id="5b34f-153">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="5b34f-153">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="5b34f-p106">Somente leitura. Anulável. A coleção de tarefas no bucket.</span><span class="sxs-lookup"><span data-stu-id="5b34f-p106">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b34f-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b34f-157">JSON representation</span></span>
<span data-ttu-id="5b34f-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b34f-158">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
