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
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a>Tipo de recurso plannerAssignedToTaskBoardTaskFormat

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso **plannerAssignedToTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição AssignedTo do Quadro de Tarefas (um modo de exibição organizado por usuários aos quais as tarefas são atribuídas). Cada [tarefa](plannertask.md) terá um objeto **plannerAssignedToTaskBoardTaskFormat** associado a ela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-get.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) |Leia as propriedades e relações do objeto **plannerAssignedToTaskBoardTaskFormat**.|
|[Update](../api/plannerassignedtotaskboardtaskformat-update.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)  |Atualize o objeto **plannerAssignedToTaskBoardTaskFormat**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID do recurso. É 28 caracteres longos e diferencia maiusculas de minúsculas. [Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.|
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->