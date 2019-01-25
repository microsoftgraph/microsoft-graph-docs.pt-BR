---
title: Tipo de recurso plannerOrderHintsByAssignee
description: O **plannerOrderHintsByAssignee** é um recurso que contém as dicas de ordenação para os destinatários em um recurso de plannerTask, para indicar a ordem da tarefa no modo do conselho tarefa atribuída a.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 27ef2c796c636e39ed6408c373cf0ac66c5572dd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520904"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a><span data-ttu-id="f8343-103">Tipo de recurso plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="f8343-103">plannerOrderHintsByAssignee resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8343-p101">O **plannerOrderHintsByAssignee** é um recurso que contém [dicas de ordenação](planner-order-hint-format.md) para os destinatários em um recurso [plannerTask](plannertask.md) para indicar a ordem da Tarefa no modo de exibição AssignedTo do Quadro de Tarefas. Este é um Tipo Aberto. As propriedades são as identificações dos usuários atribuídos à tarefa, e os valores são as dicas de ordem.</span><span class="sxs-lookup"><span data-stu-id="f8343-p101">The **plannerOrderHintsByAssignee** is a resource that contains [ordering hints](planner-order-hint-format.md) for assignees in a [plannerTask](plannertask.md) resource, to indicate the order of the task in Assigned To view of the Task Board. This type is an open type. The properties are the ids of users assigned to the task, and the values are order hints.</span></span>

## <a name="properties"></a><span data-ttu-id="f8343-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8343-107">Properties</span></span>
<span data-ttu-id="f8343-p102">As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer as identificações dos usuários atribuídos à tarefa, como nomes de propriedades e uma [dica de ordem](planner-order-hint-format.md) válida como o valor. As propriedades não podem ser removidas deste tipo. O serviço automaticamente removerá os valores à medida que as atribuições existentes no objeto [plannerTask](plannertask.md) forem atualizadas.</span><span class="sxs-lookup"><span data-stu-id="f8343-p102">Properties of an Open Type can be defined by the client. In this case, the client must provide ids of users assigned to the task as property names, and a valid [order hint](planner-order-hint-format.md) as the value. Properties cannot be removed from this type. The service will automatically remove values as the assignments on the containing [plannerTask](plannertask.md) are updated.</span></span>

<span data-ttu-id="f8343-112">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="f8343-112">Example:</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerorderhintsbyassignee.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
