---
title: tipo de recurso plannerBucketTaskBoardTaskFormat
description: O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição buckets do quadro de tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais são atribuídas). Cada tarefa terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f90d90cd0b625c612b125ffc031fe6c3e252a253
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026527"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="e6dfc-104">tipo de recurso plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e6dfc-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="e6dfc-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6dfc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6dfc-106">O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição buckets do quadro de tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais são atribuídas).</span><span class="sxs-lookup"><span data-stu-id="e6dfc-106">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to).</span></span> <span data-ttu-id="e6dfc-107">Cada [tarefa](plannertask.md) terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="e6dfc-107">Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="e6dfc-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="e6dfc-108">Methods</span></span>

| <span data-ttu-id="e6dfc-109">Método</span><span class="sxs-lookup"><span data-stu-id="e6dfc-109">Method</span></span>           | <span data-ttu-id="e6dfc-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e6dfc-110">Return Type</span></span>    |<span data-ttu-id="e6dfc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6dfc-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e6dfc-112">Obter plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e6dfc-112">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="e6dfc-113">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e6dfc-113">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="e6dfc-114">Leia as propriedades e os relacionamentos do objeto **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="e6dfc-114">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="e6dfc-115">Update</span><span class="sxs-lookup"><span data-stu-id="e6dfc-115">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="e6dfc-116">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e6dfc-116">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="e6dfc-117">Atualize o objeto **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="e6dfc-117">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e6dfc-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6dfc-118">Properties</span></span>
| <span data-ttu-id="e6dfc-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6dfc-119">Property</span></span>     | <span data-ttu-id="e6dfc-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6dfc-120">Type</span></span>   |<span data-ttu-id="e6dfc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6dfc-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6dfc-122">id</span><span class="sxs-lookup"><span data-stu-id="e6dfc-122">id</span></span>|<span data-ttu-id="e6dfc-123">String</span><span class="sxs-lookup"><span data-stu-id="e6dfc-123">String</span></span>| <span data-ttu-id="e6dfc-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6dfc-124">Read-only.</span></span> <span data-ttu-id="e6dfc-125">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6dfc-125">ID of the resource.</span></span> <span data-ttu-id="e6dfc-126">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="e6dfc-126">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="e6dfc-127">[Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="e6dfc-127">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="e6dfc-128">orderHint</span><span class="sxs-lookup"><span data-stu-id="e6dfc-128">orderHint</span></span>|<span data-ttu-id="e6dfc-129">String</span><span class="sxs-lookup"><span data-stu-id="e6dfc-129">String</span></span>|<span data-ttu-id="e6dfc-130">Dica usada para ordenar tarefas no modo de exibição de Bucket do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="e6dfc-130">Hint used to order tasks in the Bucket view of the Task Board.</span></span> <span data-ttu-id="e6dfc-131">O formato é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="e6dfc-131">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6dfc-132">Relações</span><span class="sxs-lookup"><span data-stu-id="e6dfc-132">Relationships</span></span>
<span data-ttu-id="e6dfc-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6dfc-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e6dfc-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6dfc-134">JSON representation</span></span>
<span data-ttu-id="e6dfc-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6dfc-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


