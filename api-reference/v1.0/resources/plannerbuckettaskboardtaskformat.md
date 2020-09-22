---
title: tipo de recurso plannerBucketTaskBoardTaskFormat
description: O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição buckets do quadro de tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais são atribuídas). Cada tarefa terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 1bd9282a137640af0abc1fd590ac5a87c18ea94e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037497"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="422f1-104">tipo de recurso plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="422f1-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="422f1-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="422f1-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="422f1-106">O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição buckets do quadro de tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais são atribuídas).</span><span class="sxs-lookup"><span data-stu-id="422f1-106">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to).</span></span> <span data-ttu-id="422f1-107">Cada [tarefa](plannertask.md) terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="422f1-107">Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="422f1-108">Methods</span><span class="sxs-lookup"><span data-stu-id="422f1-108">Methods</span></span>

| <span data-ttu-id="422f1-109">Método</span><span class="sxs-lookup"><span data-stu-id="422f1-109">Method</span></span>           | <span data-ttu-id="422f1-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="422f1-110">Return Type</span></span>    |<span data-ttu-id="422f1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="422f1-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="422f1-112">Obter plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="422f1-112">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="422f1-113">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="422f1-113">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="422f1-114">Leia as propriedades e os relacionamentos do objeto **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="422f1-114">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="422f1-115">Atualização</span><span class="sxs-lookup"><span data-stu-id="422f1-115">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="422f1-116">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="422f1-116">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="422f1-117">Atualize o objeto **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="422f1-117">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="422f1-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="422f1-118">Properties</span></span>
| <span data-ttu-id="422f1-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="422f1-119">Property</span></span>     | <span data-ttu-id="422f1-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="422f1-120">Type</span></span>   |<span data-ttu-id="422f1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="422f1-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="422f1-122">id</span><span class="sxs-lookup"><span data-stu-id="422f1-122">id</span></span>|<span data-ttu-id="422f1-123">String</span><span class="sxs-lookup"><span data-stu-id="422f1-123">String</span></span>| <span data-ttu-id="422f1-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="422f1-124">Read-only.</span></span> <span data-ttu-id="422f1-125">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="422f1-125">ID of the resource.</span></span> <span data-ttu-id="422f1-126">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="422f1-126">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="422f1-127">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="422f1-127">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="422f1-128">orderHint</span><span class="sxs-lookup"><span data-stu-id="422f1-128">orderHint</span></span>|<span data-ttu-id="422f1-129">String</span><span class="sxs-lookup"><span data-stu-id="422f1-129">String</span></span>|<span data-ttu-id="422f1-130">Dica usada para ordenar tarefas no modo de exibição de Bucket do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="422f1-130">Hint used to order tasks in the Bucket view of the Task Board.</span></span> <span data-ttu-id="422f1-131">O formato é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="422f1-131">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="422f1-132">Relações</span><span class="sxs-lookup"><span data-stu-id="422f1-132">Relationships</span></span>
<span data-ttu-id="422f1-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="422f1-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="422f1-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="422f1-134">JSON representation</span></span>
<span data-ttu-id="422f1-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="422f1-135">Here is a JSON representation of the resource.</span></span>

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

