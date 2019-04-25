---
title: tipo de recurso plannerBucket
description: ) para tarefas em um plano no Office 365. Ele está contido em um plannerPlan e pode ter uma coleção de plannerTasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 85cf30bc13b3236928e662807a144f81614adbd7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579251"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="d74da-104">tipo de recurso plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d74da-104">plannerBucket resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d74da-105">O recurso **plannerBucket** representa um Bucket (ou "coluna personalizada") para tarefas em um plano no Office 365.</span><span class="sxs-lookup"><span data-stu-id="d74da-105">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365.</span></span> <span data-ttu-id="d74da-106">Ele está contido em um [plannerPlan](plannerplan.md) e pode ter uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="d74da-106">It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="d74da-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d74da-107">Methods</span></span>

| <span data-ttu-id="d74da-108">Método</span><span class="sxs-lookup"><span data-stu-id="d74da-108">Method</span></span>           | <span data-ttu-id="d74da-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d74da-109">Return Type</span></span>    |<span data-ttu-id="d74da-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d74da-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d74da-111">Obter plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d74da-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="d74da-112">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d74da-112">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="d74da-113">Leia as propriedades e os relacionamentos do objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="d74da-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="d74da-114">Listar plannerTasks</span><span class="sxs-lookup"><span data-stu-id="d74da-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="d74da-115">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="d74da-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d74da-116">Obtenha uma coleção de objetos **plannerTask** .</span><span class="sxs-lookup"><span data-stu-id="d74da-116">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="d74da-117">Create</span><span class="sxs-lookup"><span data-stu-id="d74da-117">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="d74da-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d74da-118">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="d74da-119">Criar um novo objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="d74da-119">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="d74da-120">Update</span><span class="sxs-lookup"><span data-stu-id="d74da-120">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="d74da-121">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d74da-121">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="d74da-122">Atualize o objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="d74da-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="d74da-123">Excluir</span><span class="sxs-lookup"><span data-stu-id="d74da-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="d74da-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d74da-124">None</span></span> |<span data-ttu-id="d74da-125">Exclua o objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="d74da-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d74da-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d74da-126">Properties</span></span>
| <span data-ttu-id="d74da-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d74da-127">Property</span></span>     | <span data-ttu-id="d74da-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="d74da-128">Type</span></span>   |<span data-ttu-id="d74da-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="d74da-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d74da-130">id</span><span class="sxs-lookup"><span data-stu-id="d74da-130">id</span></span>|<span data-ttu-id="d74da-131">String</span><span class="sxs-lookup"><span data-stu-id="d74da-131">String</span></span>| <span data-ttu-id="d74da-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d74da-132">Read-only.</span></span> <span data-ttu-id="d74da-133">ID do Bucket.</span><span class="sxs-lookup"><span data-stu-id="d74da-133">ID of the bucket.</span></span> <span data-ttu-id="d74da-134">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d74da-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d74da-135">[Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="d74da-135">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d74da-136">name</span><span class="sxs-lookup"><span data-stu-id="d74da-136">name</span></span>|<span data-ttu-id="d74da-137">String</span><span class="sxs-lookup"><span data-stu-id="d74da-137">String</span></span>|<span data-ttu-id="d74da-138">Nome do Bucket.</span><span class="sxs-lookup"><span data-stu-id="d74da-138">Name of the bucket.</span></span>|
|<span data-ttu-id="d74da-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="d74da-139">orderHint</span></span>|<span data-ttu-id="d74da-140">String</span><span class="sxs-lookup"><span data-stu-id="d74da-140">String</span></span>|<span data-ttu-id="d74da-p104">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="d74da-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="d74da-143">planId</span><span class="sxs-lookup"><span data-stu-id="d74da-143">planId</span></span>|<span data-ttu-id="d74da-144">String</span><span class="sxs-lookup"><span data-stu-id="d74da-144">String</span></span>|<span data-ttu-id="d74da-145">ID do plano ao qual o Bucket pertence.</span><span class="sxs-lookup"><span data-stu-id="d74da-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d74da-146">Relações</span><span class="sxs-lookup"><span data-stu-id="d74da-146">Relationships</span></span>
| <span data-ttu-id="d74da-147">Relação</span><span class="sxs-lookup"><span data-stu-id="d74da-147">Relationship</span></span> | <span data-ttu-id="d74da-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="d74da-148">Type</span></span>   |<span data-ttu-id="d74da-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="d74da-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d74da-150">tarefas</span><span class="sxs-lookup"><span data-stu-id="d74da-150">tasks</span></span>|<span data-ttu-id="d74da-151">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="d74da-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d74da-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d74da-152">Read-only.</span></span> <span data-ttu-id="d74da-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d74da-153">Nullable.</span></span> <span data-ttu-id="d74da-154">A coleção de tarefas no Bucket.</span><span class="sxs-lookup"><span data-stu-id="d74da-154">The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d74da-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d74da-155">JSON representation</span></span>
<span data-ttu-id="d74da-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d74da-156">Here is a JSON representation of the resource.</span></span>

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
