---
title: Tipo de recurso plannerBucketTaskBoardTaskFormat
description: O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Buckets do Quadro de Tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais elas são atribuídas). Cada tarefa terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 4982b0b539412058d6d598893b698f12d88bd671
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986219"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="80bd1-104">Tipo de recurso plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="80bd1-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="80bd1-p102">O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Buckets do Quadro de Tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais elas são atribuídas). Cada [tarefa](plannertask.md) terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="80bd1-p102">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="80bd1-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="80bd1-107">Methods</span></span>

| <span data-ttu-id="80bd1-108">Método</span><span class="sxs-lookup"><span data-stu-id="80bd1-108">Method</span></span>           | <span data-ttu-id="80bd1-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="80bd1-109">Return Type</span></span>    |<span data-ttu-id="80bd1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="80bd1-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="80bd1-111">Get plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="80bd1-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="80bd1-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="80bd1-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="80bd1-113">Leia as propriedades e as relações do objeto **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="80bd1-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="80bd1-114">Update</span><span class="sxs-lookup"><span data-stu-id="80bd1-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="80bd1-115">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="80bd1-115">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="80bd1-116">Atualize o objeto **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="80bd1-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="80bd1-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80bd1-117">Properties</span></span>
| <span data-ttu-id="80bd1-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80bd1-118">Property</span></span>     | <span data-ttu-id="80bd1-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="80bd1-119">Type</span></span>   |<span data-ttu-id="80bd1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="80bd1-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80bd1-121">id</span><span class="sxs-lookup"><span data-stu-id="80bd1-121">id</span></span>|<span data-ttu-id="80bd1-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80bd1-122">String</span></span>| <span data-ttu-id="80bd1-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80bd1-123">Read-only.</span></span> <span data-ttu-id="80bd1-124">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="80bd1-124">ID of the resource.</span></span> <span data-ttu-id="80bd1-125">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="80bd1-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="80bd1-126">[Validação de formato](planner-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="80bd1-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="80bd1-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="80bd1-127">orderHint</span></span>|<span data-ttu-id="80bd1-128">String</span><span class="sxs-lookup"><span data-stu-id="80bd1-128">String</span></span>|<span data-ttu-id="80bd1-p104">Dica usada para ordenar tarefas no modo de exibição Bucket do Quadro de Tarefas. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="80bd1-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="80bd1-131">Relações</span><span class="sxs-lookup"><span data-stu-id="80bd1-131">Relationships</span></span>
<span data-ttu-id="80bd1-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80bd1-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="80bd1-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80bd1-133">JSON representation</span></span>
<span data-ttu-id="80bd1-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80bd1-134">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
