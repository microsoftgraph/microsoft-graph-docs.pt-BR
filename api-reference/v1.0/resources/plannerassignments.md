---
title: Tipo de recurso plannerAssignments
description: 'O **recurso plannerAssignments** representa atribuições de um recurso plannerTask. Esse tipo é um tipo aberto. Cada nome da propriedade neste tipo '
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: c6c90a607622dc47f7fd3a3d77b7b42b2c39b6e5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044339"
---
# <a name="plannerassignments-resource-type"></a>Tipo de recurso plannerAssignments

Namespace: microsoft.graph

O **recurso plannerAssignments** representa atribuições de um [recurso plannerTask.](plannertask.md) Esse tipo é um tipo aberto. Cada nome de propriedade nesse tipo é a ID de um objeto de usuário ao qual uma tarefa é atribuída. Os usuários podem ser atribuídos a tarefas com a criação de novas propriedades nomeadas com sua ID, com um objeto [plannerassignment](plannerassignment.md) com a propriedade orderHint preenchida como o valor. Os atribuídos podem ser não atribuídos da tarefa definindo o propety nomeado com sua ID como nulo.


## <a name="properties"></a>Propriedades
As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, porém, o cliente deve fornecer as IDs do usuário atribuídas como nomes de propriedade. A propriedade deve ser definida como um **objeto plannerAssignment** para criar ou modificar os atribuídos e null para removê-los.

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
Este exemplo remove o usuário com a ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 da lista de destinatários da tarefa, enquanto altera a ordem do destinatário com a ID do usuário 4e98f8f1-bb03-4015-b8e0-19bb370949d8. Se a tarefa ainda não estiver atribuída ao usuário com a ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8, a atualização das atribuições com esse valor atribuirá a tarefa a esse usuário.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

