---
title: tipo de recurso plannerBucketTaskBoardTaskFormat
description: O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição buckets do quadro de tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais são atribuídas). Cada tarefa terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b9e9713dca07e8eff0b320fcc50c8c48cc46f489
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009096"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="b78d7-104">tipo de recurso plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="b78d7-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b78d7-105">O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição buckets do quadro de tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais são atribuídas).</span><span class="sxs-lookup"><span data-stu-id="b78d7-105">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to).</span></span> <span data-ttu-id="b78d7-106">Cada [tarefa](plannertask.md) terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="b78d7-106">Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="b78d7-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b78d7-107">Methods</span></span>

| <span data-ttu-id="b78d7-108">Método</span><span class="sxs-lookup"><span data-stu-id="b78d7-108">Method</span></span>           | <span data-ttu-id="b78d7-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b78d7-109">Return Type</span></span>    |<span data-ttu-id="b78d7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b78d7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b78d7-111">Obter plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="b78d7-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="b78d7-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="b78d7-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="b78d7-113">Leia as propriedades e os relacionamentos do objeto **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="b78d7-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="b78d7-114">Atualização</span><span class="sxs-lookup"><span data-stu-id="b78d7-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="b78d7-115">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="b78d7-115">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="b78d7-116">Atualize o objeto **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="b78d7-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b78d7-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b78d7-117">Properties</span></span>
| <span data-ttu-id="b78d7-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b78d7-118">Property</span></span>     | <span data-ttu-id="b78d7-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b78d7-119">Type</span></span>   |<span data-ttu-id="b78d7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b78d7-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b78d7-121">id</span><span class="sxs-lookup"><span data-stu-id="b78d7-121">id</span></span>|<span data-ttu-id="b78d7-122">String</span><span class="sxs-lookup"><span data-stu-id="b78d7-122">String</span></span>| <span data-ttu-id="b78d7-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b78d7-123">Read-only.</span></span> <span data-ttu-id="b78d7-124">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="b78d7-124">ID of the resource.</span></span> <span data-ttu-id="b78d7-125">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="b78d7-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="b78d7-126">[Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="b78d7-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="b78d7-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="b78d7-127">orderHint</span></span>|<span data-ttu-id="b78d7-128">String</span><span class="sxs-lookup"><span data-stu-id="b78d7-128">String</span></span>|<span data-ttu-id="b78d7-129">Dica usada para ordenar tarefas no modo de exibição de Bucket do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="b78d7-129">Hint used to order tasks in the Bucket view of the Task Board.</span></span> <span data-ttu-id="b78d7-130">O formato é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="b78d7-130">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="b78d7-131">Relações</span><span class="sxs-lookup"><span data-stu-id="b78d7-131">Relationships</span></span>
<span data-ttu-id="b78d7-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b78d7-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b78d7-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b78d7-133">JSON representation</span></span>
<span data-ttu-id="b78d7-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b78d7-134">Here is a JSON representation of the resource.</span></span>

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
