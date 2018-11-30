---
title: Tipo de recurso plannerAssignedToTaskBoardTaskFormat
description: O recurso **plannerAssignedToTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição AssignedTo do Quadro de Tarefas (um modo de exibição organizado por usuários aos quais as tarefas são atribuídas). Cada tarefa terá um objeto **plannerAssignedToTaskBoardTaskFormat** associado a ela.
ms.openlocfilehash: 35aaf5d93e4190fead1234131864e7fab11b96b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005995"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="9e449-104">Tipo de recurso plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9e449-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="9e449-p102">O recurso **plannerAssignedToTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição AssignedTo do Quadro de Tarefas (um modo de exibição organizado por usuários aos quais as tarefas são atribuídas). Cada [tarefa](plannertask.md) terá um objeto **plannerAssignedToTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="9e449-p102">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="9e449-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="9e449-107">Methods</span></span>

| <span data-ttu-id="9e449-108">Método</span><span class="sxs-lookup"><span data-stu-id="9e449-108">Method</span></span>           | <span data-ttu-id="9e449-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9e449-109">Return Type</span></span>    |<span data-ttu-id="9e449-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e449-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9e449-111">Get plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9e449-111">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="9e449-112">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9e449-112">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="9e449-113">Leia as propriedades e relações do objeto **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="9e449-113">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="9e449-114">Update</span><span class="sxs-lookup"><span data-stu-id="9e449-114">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="9e449-115">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9e449-115">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="9e449-116">Atualize o objeto **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="9e449-116">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9e449-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e449-117">Properties</span></span>
| <span data-ttu-id="9e449-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e449-118">Property</span></span>     | <span data-ttu-id="9e449-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e449-119">Type</span></span>   |<span data-ttu-id="9e449-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e449-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e449-121">id</span><span class="sxs-lookup"><span data-stu-id="9e449-121">id</span></span>|<span data-ttu-id="9e449-122">String</span><span class="sxs-lookup"><span data-stu-id="9e449-122">String</span></span>| <span data-ttu-id="9e449-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e449-123">Read-only.</span></span> <span data-ttu-id="9e449-124">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e449-124">ID of the resource.</span></span> <span data-ttu-id="9e449-125">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9e449-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="9e449-126">[Validação de formato](planner-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="9e449-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="9e449-127">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="9e449-127">orderHintsByAssignee</span></span>|[<span data-ttu-id="9e449-128">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="9e449-128">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="9e449-p104">O dicionário de dicas usado para ordenar tarefas no modo de exibição AssignedTo do Quadro de Tarefas. A chave de cada entrada é um dos usuários ao qual a tarefa é atribuída, e o valor é a dica de ordem. O formato de cada valor é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="9e449-p104">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="9e449-132">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="9e449-132">unassignedOrderHint</span></span>|<span data-ttu-id="9e449-133">String</span><span class="sxs-lookup"><span data-stu-id="9e449-133">String</span></span>|<span data-ttu-id="9e449-p105">Valor da dica usado para ordenar a tarefa no modo de exibição AssignedTo do Quadro de Tarefas quando a tarefa não for atribuída a ninguém ou se o dicionário orderHintsByAssignee não oferecer uma dica de ordem para o usuário à qual a tarefa foi atribuída. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="9e449-p105">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e449-136">Relações</span><span class="sxs-lookup"><span data-stu-id="9e449-136">Relationships</span></span>
<span data-ttu-id="9e449-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e449-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9e449-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e449-138">JSON representation</span></span>
<span data-ttu-id="9e449-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e449-139">Here is a JSON representation of the resource.</span></span>

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