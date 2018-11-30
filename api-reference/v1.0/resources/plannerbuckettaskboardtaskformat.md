---
title: Tipo de recurso plannerBucketTaskBoardTaskFormat
description: O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Buckets do Quadro de Tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais elas são atribuídas). Cada tarefa terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.
ms.openlocfilehash: 7fb15bf59b2c7ffc0a515baff7b3f0dda8be179f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003836"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="d2876-104">Tipo de recurso plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d2876-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="d2876-p102">O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Buckets do Quadro de Tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais elas são atribuídas). Cada [tarefa](plannertask.md) terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="d2876-p102">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="d2876-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d2876-107">Methods</span></span>

| <span data-ttu-id="d2876-108">Método</span><span class="sxs-lookup"><span data-stu-id="d2876-108">Method</span></span>           | <span data-ttu-id="d2876-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d2876-109">Return Type</span></span>    |<span data-ttu-id="d2876-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2876-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2876-111">Get plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d2876-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="d2876-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d2876-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="d2876-113">Leia as propriedades e as relações do objeto **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="d2876-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="d2876-114">Update</span><span class="sxs-lookup"><span data-stu-id="d2876-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="d2876-115">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d2876-115">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="d2876-116">Atualize o objeto **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="d2876-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d2876-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2876-117">Properties</span></span>
| <span data-ttu-id="d2876-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2876-118">Property</span></span>     | <span data-ttu-id="d2876-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2876-119">Type</span></span>   |<span data-ttu-id="d2876-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2876-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2876-121">id</span><span class="sxs-lookup"><span data-stu-id="d2876-121">id</span></span>|<span data-ttu-id="d2876-122">String</span><span class="sxs-lookup"><span data-stu-id="d2876-122">String</span></span>| <span data-ttu-id="d2876-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d2876-123">Read-only.</span></span> <span data-ttu-id="d2876-124">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2876-124">ID of the resource.</span></span> <span data-ttu-id="d2876-125">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d2876-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d2876-126">[Validação de formato](planner-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="d2876-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d2876-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="d2876-127">orderHint</span></span>|<span data-ttu-id="d2876-128">String</span><span class="sxs-lookup"><span data-stu-id="d2876-128">String</span></span>|<span data-ttu-id="d2876-p104">Dica usada para ordenar tarefas no modo de exibição Bucket do Quadro de Tarefas. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="d2876-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2876-131">Relações</span><span class="sxs-lookup"><span data-stu-id="d2876-131">Relationships</span></span>
<span data-ttu-id="d2876-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2876-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d2876-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2876-133">JSON representation</span></span>
<span data-ttu-id="d2876-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2876-134">Here is a JSON representation of the resource.</span></span>

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