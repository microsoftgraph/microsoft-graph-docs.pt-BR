---
title: tipo de recurso plannerOrderHintsByAssignee
description: O **plannerOrderHintsByAssignee** é um recurso que contém dicas de ordenação para destinatários em um recurso plannerTask, para indicar a ordem da tarefa em atribuída ao modo de exibição do quadro de tarefas.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: c4c5099485c75c41e9ebb6275a7ffa5fed3be5a2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035228"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a><span data-ttu-id="24ad2-103">tipo de recurso plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="24ad2-103">plannerOrderHintsByAssignee resource type</span></span>

<span data-ttu-id="24ad2-104">O **plannerOrderHintsByAssignee** é um recurso que contém [dicas](planner-order-hint-format.md) de ordenação para destinatários em um recurso [plannerTask](plannertask.md) , para indicar a ordem da tarefa em atribuída ao modo de exibição do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="24ad2-104">The **plannerOrderHintsByAssignee** is a resource that contains [ordering hints](planner-order-hint-format.md) for assignees in a [plannerTask](plannertask.md) resource, to indicate the order of the task in Assigned To view of the Task Board.</span></span>
<span data-ttu-id="24ad2-105">Este tipo é um tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="24ad2-105">This type is an open type.</span></span> <span data-ttu-id="24ad2-106">As propriedades são as IDs dos usuários atribuídos à tarefa e os valores são dicas de ordenação.</span><span class="sxs-lookup"><span data-stu-id="24ad2-106">The properties are the ids of users assigned to the task, and the values are order hints.</span></span>

## <a name="properties"></a><span data-ttu-id="24ad2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="24ad2-107">Properties</span></span>
<span data-ttu-id="24ad2-108">As propriedades de um tipo aberto podem ser definidas pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="24ad2-108">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="24ad2-109">Nesse caso, o cliente deve fornecer IDs de usuários atribuídos à tarefa como nomes de propriedade e uma [dica de ordem](planner-order-hint-format.md) válida como o valor.</span><span class="sxs-lookup"><span data-stu-id="24ad2-109">In this case, the client must provide ids of users assigned to the task as property names, and a valid [order hint](planner-order-hint-format.md) as the value.</span></span>
<span data-ttu-id="24ad2-110">As propriedades não podem ser removidas desse tipo.</span><span class="sxs-lookup"><span data-stu-id="24ad2-110">Properties cannot be removed from this type.</span></span> <span data-ttu-id="24ad2-111">O serviço removerá automaticamente os valores, já que as atribuições no [plannerTask](plannertask.md) que o contém são atualizadas.</span><span class="sxs-lookup"><span data-stu-id="24ad2-111">The service will automatically remove values as the assignments on the containing [plannerTask](plannertask.md) are updated.</span></span>

<span data-ttu-id="24ad2-112">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="24ad2-112">Example:</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47", "4e98f8f1-bb03-4015-b8e0-19bb370949d8" ],
  "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": "String",
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
