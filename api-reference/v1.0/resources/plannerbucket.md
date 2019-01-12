---
title: Tipo de recurso plannerBucket
description: ) para tarefas em um plano no Office 365. Ele está contido em um plannerPlan e pode ter uma coleção de plannerTasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 8cfc25e5554b20d4f808c8929b53549f4c44d7a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982831"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="699fa-104">Tipo de recurso plannerBucket</span><span class="sxs-lookup"><span data-stu-id="699fa-104">plannerBucket resource type</span></span>

<span data-ttu-id="699fa-p102">O recurso **plannerBucket** representa um Bucket (ou "coluna personalizada") para tarefas em um plano no Office 365. Ele está contido em um [plannerPlan](plannerplan.md) e pode ter uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="699fa-p102">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="699fa-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="699fa-107">Methods</span></span>

| <span data-ttu-id="699fa-108">Método</span><span class="sxs-lookup"><span data-stu-id="699fa-108">Method</span></span>           | <span data-ttu-id="699fa-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="699fa-109">Return Type</span></span>    |<span data-ttu-id="699fa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="699fa-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="699fa-111">Get plannerBucket</span><span class="sxs-lookup"><span data-stu-id="699fa-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="699fa-112">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="699fa-112">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="699fa-113">Leia as propriedades e as relações do objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="699fa-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="699fa-114">Listar plannerTasks</span><span class="sxs-lookup"><span data-stu-id="699fa-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="699fa-115">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="699fa-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="699fa-116">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="699fa-116">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="699fa-117">Criar</span><span class="sxs-lookup"><span data-stu-id="699fa-117">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="699fa-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="699fa-118">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="699fa-119">Crie um novo objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="699fa-119">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="699fa-120">Update</span><span class="sxs-lookup"><span data-stu-id="699fa-120">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="699fa-121">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="699fa-121">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="699fa-122">Atualize o objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="699fa-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="699fa-123">Delete</span><span class="sxs-lookup"><span data-stu-id="699fa-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="699fa-124">None</span><span class="sxs-lookup"><span data-stu-id="699fa-124">None</span></span> |<span data-ttu-id="699fa-125">Exclua o objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="699fa-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="699fa-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="699fa-126">Properties</span></span>
| <span data-ttu-id="699fa-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="699fa-127">Property</span></span>     | <span data-ttu-id="699fa-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="699fa-128">Type</span></span>   |<span data-ttu-id="699fa-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="699fa-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="699fa-130">id</span><span class="sxs-lookup"><span data-stu-id="699fa-130">id</span></span>|<span data-ttu-id="699fa-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="699fa-131">String</span></span>| <span data-ttu-id="699fa-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="699fa-132">Read-only.</span></span> <span data-ttu-id="699fa-133">ID do compartimento de memória.</span><span class="sxs-lookup"><span data-stu-id="699fa-133">ID of the bucket.</span></span> <span data-ttu-id="699fa-134">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="699fa-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="699fa-135">[Validação de formato](planner-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="699fa-135">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="699fa-136">name</span><span class="sxs-lookup"><span data-stu-id="699fa-136">name</span></span>|<span data-ttu-id="699fa-137">String</span><span class="sxs-lookup"><span data-stu-id="699fa-137">String</span></span>|<span data-ttu-id="699fa-138">Nome do bucket.</span><span class="sxs-lookup"><span data-stu-id="699fa-138">Name of the bucket.</span></span>|
|<span data-ttu-id="699fa-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="699fa-139">orderHint</span></span>|<span data-ttu-id="699fa-140">String</span><span class="sxs-lookup"><span data-stu-id="699fa-140">String</span></span>|<span data-ttu-id="699fa-p104">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="699fa-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="699fa-143">planId</span><span class="sxs-lookup"><span data-stu-id="699fa-143">planId</span></span>|<span data-ttu-id="699fa-144">String</span><span class="sxs-lookup"><span data-stu-id="699fa-144">String</span></span>|<span data-ttu-id="699fa-145">ID do plano ao qual o bucket pertence.</span><span class="sxs-lookup"><span data-stu-id="699fa-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="699fa-146">Relações</span><span class="sxs-lookup"><span data-stu-id="699fa-146">Relationships</span></span>
| <span data-ttu-id="699fa-147">Relação</span><span class="sxs-lookup"><span data-stu-id="699fa-147">Relationship</span></span> | <span data-ttu-id="699fa-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="699fa-148">Type</span></span>   |<span data-ttu-id="699fa-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="699fa-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="699fa-150">tarefas</span><span class="sxs-lookup"><span data-stu-id="699fa-150">tasks</span></span>|<span data-ttu-id="699fa-151">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="699fa-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="699fa-p105">Somente leitura. Anulável. A coleção de tarefas no bucket.</span><span class="sxs-lookup"><span data-stu-id="699fa-p105">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="699fa-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="699fa-155">JSON representation</span></span>
<span data-ttu-id="699fa-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="699fa-156">Here is a JSON representation of the resource.</span></span>

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
