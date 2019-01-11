---
title: Tipo de recurso plannerAssignments
description: 'O recurso de **plannerAssignments** representa atribuições de um recurso de plannerTask. Esse tipo é um tipo aberto. Nesse tipo de cada nome de propriedade '
localization_priority: Normal
ms.openlocfilehash: b858aa15181a53f4bb2abf58d16662a27a8230fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856004"
---
# <a name="plannerassignments-resource-type"></a>Tipo de recurso plannerAssignments

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso **plannerAssignment** representa as atribuições de um recurso [plannerTask](plannertask.md). Este é um Tipo Aberto. Cada nome de propriedade nesse tipo representa a ID do objeto de um usuário à qual uma tarefa é atribuída. Os usuários podem ser atribuídos a tarefas com a criação de novas propriedades nomeadas com sua ID, com um objeto [plannerassignment](plannerassignment.md) com a propriedade orderHint preenchida como o valor. Os destinatários podem ter a atribuição cancelada a partir da tarefa se a propriedade nomeada com a ID for configurada como nula.


## <a name="properties"></a>Propriedades
As propriedades de um Tipo Aberto podem ser definidas pelo cliente. No entanto, nesse caso, o cliente deve fornecer IDs do usuário atribuídas como nomes de propriedades. A propriedade deve ser definida com um objeto **plannerAssignment** para criar ou modificar os destinatários e como nula para removê-los.

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
Este exemplo remove usuário com a ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 da lista de destinatários da tarefa ao alterar a ordem dos destinatário com o usuário ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8. Se a tarefa já não estiver atribuída ao usuário com a ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8, a tarefa será atribuída a esse usuário se as atribuições forem atualizadas com esse valor.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
