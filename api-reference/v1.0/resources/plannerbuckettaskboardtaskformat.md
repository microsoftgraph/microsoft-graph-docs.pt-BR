---
title: tipo de recurso plannerBucketTaskBoardTaskFormat
description: O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição buckets do quadro de tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais são atribuídas). Cada tarefa terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 4982b0b539412058d6d598893b698f12d88bd671
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462239"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="abdda-104">tipo de recurso plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="abdda-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="abdda-105">O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição buckets do quadro de tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais são atribuídas).</span><span class="sxs-lookup"><span data-stu-id="abdda-105">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to).</span></span> <span data-ttu-id="abdda-106">Cada [tarefa](plannertask.md) terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="abdda-106">Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="abdda-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="abdda-107">Methods</span></span>

| <span data-ttu-id="abdda-108">Método</span><span class="sxs-lookup"><span data-stu-id="abdda-108">Method</span></span>           | <span data-ttu-id="abdda-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="abdda-109">Return Type</span></span>    |<span data-ttu-id="abdda-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="abdda-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="abdda-111">Obter plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="abdda-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="abdda-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="abdda-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="abdda-113">Leia as propriedades e os relacionamentos do objeto **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="abdda-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="abdda-114">Atualização</span><span class="sxs-lookup"><span data-stu-id="abdda-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="abdda-115">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="abdda-115">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="abdda-116">Atualize o objeto **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="abdda-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="abdda-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="abdda-117">Properties</span></span>
| <span data-ttu-id="abdda-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abdda-118">Property</span></span>     | <span data-ttu-id="abdda-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="abdda-119">Type</span></span>   |<span data-ttu-id="abdda-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="abdda-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abdda-121">id</span><span class="sxs-lookup"><span data-stu-id="abdda-121">id</span></span>|<span data-ttu-id="abdda-122">String</span><span class="sxs-lookup"><span data-stu-id="abdda-122">String</span></span>| <span data-ttu-id="abdda-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="abdda-123">Read-only.</span></span> <span data-ttu-id="abdda-124">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="abdda-124">ID of the resource.</span></span> <span data-ttu-id="abdda-125">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="abdda-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="abdda-126">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="abdda-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="abdda-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="abdda-127">orderHint</span></span>|<span data-ttu-id="abdda-128">String</span><span class="sxs-lookup"><span data-stu-id="abdda-128">String</span></span>|<span data-ttu-id="abdda-129">Dica usada para ordenar tarefas no modo de exibição de Bucket do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="abdda-129">Hint used to order tasks in the Bucket view of the Task Board.</span></span> <span data-ttu-id="abdda-130">O formato é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="abdda-130">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="abdda-131">Relações</span><span class="sxs-lookup"><span data-stu-id="abdda-131">Relationships</span></span>
<span data-ttu-id="abdda-132">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="abdda-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="abdda-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="abdda-133">JSON representation</span></span>
<span data-ttu-id="abdda-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="abdda-134">Here is a JSON representation of the resource.</span></span>

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
