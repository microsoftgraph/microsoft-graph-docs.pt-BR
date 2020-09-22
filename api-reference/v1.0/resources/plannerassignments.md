---
title: tipo de recurso plannerAssignments
description: 'O recurso **plannerAssignments** representa as atribuições de um recurso plannerTask. Este tipo é um tipo aberto. Cada nome de propriedade neste tipo '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: ba9240839d4541a9bd3858289a452c4176abdb09
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037532"
---
# <a name="plannerassignments-resource-type"></a>tipo de recurso plannerAssignments

Namespace: microsoft.graph

O recurso **plannerAssignments** representa as atribuições de um recurso [plannerTask](plannertask.md) . Este tipo é um tipo aberto. Cada nome de propriedade desse tipo é a ID de um objeto de usuário ao qual uma tarefa é atribuída. Os usuários podem ser atribuídos a tarefas com a criação de novas propriedades nomeadas com a ID, com um objeto [plannerassignment](plannerassignment.md) com a propriedade orderHint preenchida como o valor. Os destinatários podem ser desatribuídos da tarefa definindo o propriedade nomeado com sua ID como nulo.


## <a name="properties"></a>Propriedades
As propriedades de um tipo aberto podem ser definidas pelo cliente. Nesse caso, no entanto, o cliente deve fornecer IDs de usuário atribuídas como nomes de propriedade. A propriedade deve ser definida como um objeto **plannerAssignment** para criar ou modificar destinatários, e como nulo para removê-los.

Exemplo:

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47", "4e98f8f1-bb03-4015-b8e0-19bb370949d8" ],
  "@odata.type": "microsoft.graph.plannerAssignments"
}-->
```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": null,
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": { 
      "@odata.type": "microsoft.graph.plannerAssignment",
      "orderHint": "String"
    }
}
```
Este exemplo remove o usuário com ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 da lista de destinatários da tarefa, enquanto altera a ordem do destinatário com a ID de usuário 4e98f8f1-BB03-4015-B8E0-19bb370949d8. Se a tarefa ainda não estiver atribuída ao usuário com ID 4e98f8f1-BB03-4015-B8E0-19bb370949d8, a atualização das atribuições com esse valor atribuirá a tarefa a esse usuário.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

