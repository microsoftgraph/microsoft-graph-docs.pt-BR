---
title: tipo de recurso plannerAssignments
description: 'O recurso **plannerAssignments** representa as atribuições de um recurso plannerTask. Este tipo é um tipo aberto. Cada nome de propriedade neste tipo '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2c379c786e3b94395aa3de7bc382e184db0fcc24
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541364"
---
# <a name="plannerassignments-resource-type"></a>tipo de recurso plannerAssignments

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **plannerAssignments** representa as atribuições de um recurso [plannerTask](plannertask.md) . Este tipo é um tipo aberto. Cada nome de propriedade desse tipo é a ID de um objeto de usuário ao qual uma tarefa é atribuída. Os usuários podem ser atribuídos a tarefas com a criação de novas propriedades nomeadas com a ID, com um objeto [plannerassignment](plannerassignment.md) com a propriedade orderHint preenchida como o valor. Os destinatários podem ser desatribuídos da tarefa definindo o propriedade nomeado com sua ID como nulo.


## <a name="properties"></a>Propriedades
As propriedades de um tipo aberto podem ser definidas pelo cliente. Nesse caso, no entanto, o cliente deve fornecer IDs de usuário atribuídas como nomes de propriedade. A propriedade deve ser definida como um objeto **plannerAssignment** para criar ou modificar destinatários, e como nulo para removê-los.

Exemplo:

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerassignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
