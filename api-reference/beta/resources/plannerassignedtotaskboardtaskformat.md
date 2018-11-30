---
title: Tipo de recurso plannerAssignedToTaskBoardTaskFormat
description: O recurso **plannerAssignedToTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição AssignedTo do Quadro de Tarefas (um modo de exibição organizado por usuários aos quais as tarefas são atribuídas). Cada tarefa terá um objeto **plannerAssignedToTaskBoardTaskFormat** associado a ela.
ms.openlocfilehash: 8fc96d6fa7d4f05f6bc81f7030ebe766bf769e40
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037288"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="da905-104">Tipo de recurso plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="da905-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="da905-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="da905-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da905-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="da905-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da905-p103">O recurso **plannerAssignedToTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição AssignedTo do Quadro de Tarefas (um modo de exibição organizado por usuários aos quais as tarefas são atribuídas). Cada [tarefa](plannertask.md) terá um objeto **plannerAssignedToTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="da905-p103">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="da905-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="da905-109">Methods</span></span>

| <span data-ttu-id="da905-110">Método</span><span class="sxs-lookup"><span data-stu-id="da905-110">Method</span></span>           | <span data-ttu-id="da905-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="da905-111">Return Type</span></span>    |<span data-ttu-id="da905-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="da905-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="da905-113">Get plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="da905-113">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="da905-114">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="da905-114">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="da905-115">Leia as propriedades e relações do objeto **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="da905-115">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="da905-116">Update</span><span class="sxs-lookup"><span data-stu-id="da905-116">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="da905-117">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="da905-117">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="da905-118">Atualize o objeto **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="da905-118">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="da905-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da905-119">Properties</span></span>
| <span data-ttu-id="da905-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da905-120">Property</span></span>     | <span data-ttu-id="da905-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="da905-121">Type</span></span>   |<span data-ttu-id="da905-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="da905-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da905-123">id</span><span class="sxs-lookup"><span data-stu-id="da905-123">id</span></span>|<span data-ttu-id="da905-124">String</span><span class="sxs-lookup"><span data-stu-id="da905-124">String</span></span>| <span data-ttu-id="da905-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="da905-125">Read-only.</span></span> <span data-ttu-id="da905-126">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="da905-126">ID of the resource.</span></span> <span data-ttu-id="da905-127">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="da905-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="da905-128">[Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="da905-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="da905-129">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="da905-129">orderHintsByAssignee</span></span>|[<span data-ttu-id="da905-130">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="da905-130">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="da905-p105">O dicionário de dicas usado para ordenar tarefas no modo de exibição AssignedTo do Quadro de Tarefas. A chave de cada entrada é um dos usuários ao qual a tarefa é atribuída, e o valor é a dica de ordem. O formato de cada valor é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="da905-p105">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="da905-134">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="da905-134">unassignedOrderHint</span></span>|<span data-ttu-id="da905-135">String</span><span class="sxs-lookup"><span data-stu-id="da905-135">String</span></span>|<span data-ttu-id="da905-p106">Valor da dica usado para ordenar a tarefa no modo de exibição AssignedTo do Quadro de Tarefas quando a tarefa não for atribuída a ninguém ou se o dicionário orderHintsByAssignee não oferecer uma dica de ordem para o usuário à qual a tarefa foi atribuída. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="da905-p106">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="da905-138">Relações</span><span class="sxs-lookup"><span data-stu-id="da905-138">Relationships</span></span>
<span data-ttu-id="da905-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da905-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="da905-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da905-140">JSON representation</span></span>
<span data-ttu-id="da905-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da905-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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