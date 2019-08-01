---
title: tipo de recurso plannerAssignedToTaskBoardTaskFormat
description: O recurso **plannerAssignedToTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição AssignedTo do quadro de tarefas (um modo organizado por usuários aos quais as tarefas são atribuídas). Cada tarefa terá um objeto **plannerAssignedToTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: c85a68a3a9c17a35bc94ee32ebff156198029bed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035347"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="c676d-104">tipo de recurso plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c676d-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="c676d-105">O recurso **plannerAssignedToTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição AssignedTo do quadro de tarefas (um modo organizado por usuários aos quais as tarefas são atribuídas).</span><span class="sxs-lookup"><span data-stu-id="c676d-105">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to).</span></span> <span data-ttu-id="c676d-106">Cada [tarefa](plannertask.md) terá um objeto **plannerAssignedToTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="c676d-106">Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="c676d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c676d-107">Methods</span></span>

| <span data-ttu-id="c676d-108">Método</span><span class="sxs-lookup"><span data-stu-id="c676d-108">Method</span></span>           | <span data-ttu-id="c676d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c676d-109">Return Type</span></span>    |<span data-ttu-id="c676d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c676d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c676d-111">Obter plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c676d-111">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="c676d-112">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c676d-112">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="c676d-113">Leia as propriedades e os relacionamentos do objeto **plannerAssignedToTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="c676d-113">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="c676d-114">Atualização</span><span class="sxs-lookup"><span data-stu-id="c676d-114">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="c676d-115">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c676d-115">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="c676d-116">Atualize o objeto **plannerAssignedToTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="c676d-116">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c676d-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c676d-117">Properties</span></span>
| <span data-ttu-id="c676d-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c676d-118">Property</span></span>     | <span data-ttu-id="c676d-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="c676d-119">Type</span></span>   |<span data-ttu-id="c676d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c676d-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c676d-121">id</span><span class="sxs-lookup"><span data-stu-id="c676d-121">id</span></span>|<span data-ttu-id="c676d-122">String</span><span class="sxs-lookup"><span data-stu-id="c676d-122">String</span></span>| <span data-ttu-id="c676d-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c676d-123">Read-only.</span></span> <span data-ttu-id="c676d-124">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="c676d-124">ID of the resource.</span></span> <span data-ttu-id="c676d-125">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="c676d-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="c676d-126">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="c676d-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="c676d-127">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="c676d-127">orderHintsByAssignee</span></span>|[<span data-ttu-id="c676d-128">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="c676d-128">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="c676d-129">Dicionário de dicas usado para ordenar tarefas na exibição AssignedTo do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="c676d-129">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board.</span></span> <span data-ttu-id="c676d-130">A chave de cada entrada é um dos usuários para os quais a tarefa é atribuída e o valor é a dica ORDER.</span><span class="sxs-lookup"><span data-stu-id="c676d-130">The key of each entry is one of the users the task is assigned to and the value is the order hint.</span></span> <span data-ttu-id="c676d-131">O formato de cada valor é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="c676d-131">The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="c676d-132">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="c676d-132">unassignedOrderHint</span></span>|<span data-ttu-id="c676d-133">String</span><span class="sxs-lookup"><span data-stu-id="c676d-133">String</span></span>|<span data-ttu-id="c676d-134">O valor de dica usado para ordenar a tarefa na exibição AssignedTo do quadro de tarefas quando a tarefa não é atribuída a qualquer pessoa ou quando o dicionário do orderHintsByAssignee não fornece uma dica de pedido para o usuário ao qual a tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="c676d-134">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to.</span></span> <span data-ttu-id="c676d-135">O formato é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="c676d-135">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c676d-136">Relações</span><span class="sxs-lookup"><span data-stu-id="c676d-136">Relationships</span></span>
<span data-ttu-id="c676d-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c676d-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c676d-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c676d-138">JSON representation</span></span>
<span data-ttu-id="c676d-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c676d-139">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
