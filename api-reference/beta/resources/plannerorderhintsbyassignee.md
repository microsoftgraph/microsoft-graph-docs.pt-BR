---
title: tipo de recurso plannerOrderHintsByAssignee
description: O **plannerOrderHintsByAssignee** é um recurso que contém dicas de ordenação para destinatários em um recurso plannerTask, para indicar a ordem da tarefa em atribuída ao modo de exibição do quadro de tarefas.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 428944f9d622bba8db5d700b8d113a2c5b476301
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344435"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a>tipo de recurso plannerOrderHintsByAssignee

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **plannerOrderHintsByAssignee** é um recurso que contém [dicas](planner-order-hint-format.md) de ordenação para destinatários em um recurso [plannerTask](plannertask.md) , para indicar a ordem da tarefa em atribuída ao modo de exibição do quadro de tarefas.
Este tipo é um tipo aberto. As propriedades são as IDs dos usuários atribuídos à tarefa e os valores são dicas de ordenação.

## <a name="properties"></a>Propriedades
As propriedades de um tipo aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer IDs de usuários atribuídos à tarefa como nomes de propriedade e uma [dica de ordem](planner-order-hint-format.md) válida como o valor.
As propriedades não podem ser removidas desse tipo. O serviço removerá automaticamente os valores, já que as atribuições no [plannerTask](plannertask.md) que o contém são atualizadas.

Exemplo:

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
  "suppressions": []
}
-->
