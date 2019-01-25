---
title: Tipo de recurso plannerAssignedToTaskBoardTaskFormat
description: O recurso **plannerAssignedToTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição AssignedTo do Quadro de Tarefas (um modo de exibição organizado por usuários aos quais as tarefas são atribuídas). Cada **tarefa** terá um objeto plannerAssignedToTaskBoardTaskFormat associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6a7aa230a610ec63559797d058cbc3f64ffe843d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529814"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a>Tipo de recurso plannerAssignedToTaskBoardTaskFormat

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **plannerAssignedToTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição AssignedTo do Quadro de Tarefas (um modo de exibição organizado por usuários aos quais as tarefas são atribuídas). Cada [tarefa](plannertask.md) terá um objeto **plannerAssignedToTaskBoardTaskFormat** associado a ela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-get.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) |Leia as propriedades e relações do objeto **plannerAssignedToTaskBoardTaskFormat**.|
|[Update](../api/plannerassignedtotaskboardtaskformat-update.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)  |Atualize o objeto **plannerAssignedToTaskBoardTaskFormat**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| Somente leitura. ID do recurso. É 28 caracteres longos e diferencia maiusculas de minúsculas. [Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.|
|orderHintsByAssignee|[plannerOrderHintsByAssignee](plannerorderhintsbyassignee.md)|O dicionário de dicas usado para ordenar tarefas no modo de exibição AssignedTo do Quadro de Tarefas. A chave de cada entrada é um dos usuários ao qual a tarefa é atribuída, e o valor é a dica de ordem. O formato de cada valor é definido como descrito [aqui](planner-order-hint-format.md).|
|unassignedOrderHint|String|Valor da dica usado para ordenar a tarefa no modo de exibição AssignedTo do Quadro de Tarefas quando a tarefa não for atribuída a ninguém ou se o dicionário orderHintsByAssignee não oferecer uma dica de ordem para o usuário à qual a tarefa foi atribuída. O formato é definido como descrito [aqui](planner-order-hint-format.md).|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerassignedtotaskboardtaskformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
