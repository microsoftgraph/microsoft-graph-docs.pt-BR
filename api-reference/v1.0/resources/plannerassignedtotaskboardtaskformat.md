---
title: tipo de recurso plannerAssignedToTaskBoardTaskFormat
description: O recurso **plannerAssignedToTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição AssignedTo do quadro de tarefas (um modo organizado por usuários aos quais as tarefas são atribuídas). Cada tarefa terá um objeto **plannerAssignedToTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 000797631f5f15b0d9128e4433512e8451975255
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534028"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="9c2d1-104">tipo de recurso plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9c2d1-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="9c2d1-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c2d1-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c2d1-106">O recurso **plannerAssignedToTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição AssignedTo do quadro de tarefas (um modo organizado por usuários aos quais as tarefas são atribuídas).</span><span class="sxs-lookup"><span data-stu-id="9c2d1-106">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to).</span></span> <span data-ttu-id="9c2d1-107">Cada [tarefa](plannertask.md) terá um objeto **plannerAssignedToTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-107">Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="9c2d1-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="9c2d1-108">Methods</span></span>

| <span data-ttu-id="9c2d1-109">Método</span><span class="sxs-lookup"><span data-stu-id="9c2d1-109">Method</span></span>           | <span data-ttu-id="9c2d1-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9c2d1-110">Return Type</span></span>    |<span data-ttu-id="9c2d1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c2d1-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c2d1-112">Obter plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9c2d1-112">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="9c2d1-113">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9c2d1-113">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="9c2d1-114">Leia as propriedades e os relacionamentos do objeto **plannerAssignedToTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="9c2d1-114">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="9c2d1-115">Atualizar</span><span class="sxs-lookup"><span data-stu-id="9c2d1-115">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="9c2d1-116">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9c2d1-116">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="9c2d1-117">Atualize o objeto **plannerAssignedToTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="9c2d1-117">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9c2d1-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c2d1-118">Properties</span></span>
| <span data-ttu-id="9c2d1-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c2d1-119">Property</span></span>     | <span data-ttu-id="9c2d1-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c2d1-120">Type</span></span>   |<span data-ttu-id="9c2d1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c2d1-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c2d1-122">id</span><span class="sxs-lookup"><span data-stu-id="9c2d1-122">id</span></span>|<span data-ttu-id="9c2d1-123">String</span><span class="sxs-lookup"><span data-stu-id="9c2d1-123">String</span></span>| <span data-ttu-id="9c2d1-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-124">Read-only.</span></span> <span data-ttu-id="9c2d1-125">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-125">ID of the resource.</span></span> <span data-ttu-id="9c2d1-126">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-126">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="9c2d1-127">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-127">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="9c2d1-128">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="9c2d1-128">orderHintsByAssignee</span></span>|[<span data-ttu-id="9c2d1-129">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="9c2d1-129">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="9c2d1-130">Dicionário de dicas usado para ordenar tarefas na exibição AssignedTo do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-130">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board.</span></span> <span data-ttu-id="9c2d1-131">A chave de cada entrada é um dos usuários para os quais a tarefa é atribuída e o valor é a dica ORDER.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-131">The key of each entry is one of the users the task is assigned to and the value is the order hint.</span></span> <span data-ttu-id="9c2d1-132">O formato de cada valor é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="9c2d1-132">The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="9c2d1-133">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="9c2d1-133">unassignedOrderHint</span></span>|<span data-ttu-id="9c2d1-134">String</span><span class="sxs-lookup"><span data-stu-id="9c2d1-134">String</span></span>|<span data-ttu-id="9c2d1-135">O valor de dica usado para ordenar a tarefa na exibição AssignedTo do quadro de tarefas quando a tarefa não é atribuída a qualquer pessoa ou quando o dicionário do orderHintsByAssignee não fornece uma dica de pedido para o usuário ao qual a tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-135">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to.</span></span> <span data-ttu-id="9c2d1-136">O formato é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="9c2d1-136">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c2d1-137">Relações</span><span class="sxs-lookup"><span data-stu-id="9c2d1-137">Relationships</span></span>
<span data-ttu-id="9c2d1-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c2d1-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9c2d1-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c2d1-139">JSON representation</span></span>
<span data-ttu-id="9c2d1-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-140">Here is a JSON representation of the resource.</span></span>

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
