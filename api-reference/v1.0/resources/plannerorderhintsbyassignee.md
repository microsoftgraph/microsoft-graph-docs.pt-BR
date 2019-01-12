---
title: Tipo de recurso plannerOrderHintsByAssignee
description: O **plannerOrderHintsByAssignee** é um recurso que contém as dicas de ordenação para os destinatários em um recurso de plannerTask, para indicar a ordem da tarefa no modo do conselho tarefa atribuída a.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b285c4a04d045c8a4e70a574c88772a0981c95e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967746"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a>Tipo de recurso plannerOrderHintsByAssignee

O **plannerOrderHintsByAssignee** é um recurso que contém [dicas de ordenação](planner-order-hint-format.md) para os destinatários em um recurso [plannerTask](plannertask.md) para indicar a ordem da Tarefa no modo de exibição AssignedTo do Quadro de Tarefas. Este é um Tipo Aberto. As propriedades são as identificações dos usuários atribuídos à tarefa, e os valores são as dicas de ordem.

## <a name="properties"></a>Propriedades
As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer as identificações dos usuários atribuídos à tarefa, como nomes de propriedades e uma [dica de ordem](planner-order-hint-format.md) válida como o valor. As propriedades não podem ser removidas deste tipo. O serviço automaticamente removerá os valores à medida que as atribuições existentes no objeto [plannerTask](plannertask.md) forem atualizadas.

Exemplo:

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
