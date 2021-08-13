---
title: Tipo de recurso plannerAssignedToTaskBoardTaskFormat
description: O **recurso plannerAssignedToTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente na exibição AssignedTo do Quadro de Tarefas (uma exibição organizada pelos usuários aos quais as tarefas são atribuídas). Cada tarefa terá um **objeto plannerAssignedToTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: ca256007f0e4b10fab53f814942736ead094555fef69b038c9680a8e08139303
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152324"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a>Tipo de recurso plannerAssignedToTaskBoardTaskFormat

Namespace: microsoft.graph

O **recurso plannerAssignedToTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente na exibição AssignedTo do Quadro de Tarefas (uma exibição organizada pelos usuários aos quais as tarefas são atribuídas). Cada [tarefa](plannertask.md) terá um **objeto plannerAssignedToTaskBoardTaskFormat** associado a ela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-get.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) |Ler propriedades e relações do **objeto plannerAssignedToTaskBoardTaskFormat.**|
|[Atualizar](../api/plannerassignedtotaskboardtaskformat-update.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)  |Atualizar **o objeto plannerAssignedToTaskBoardTaskFormat.** |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID do recurso. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.|
|orderHintsByAssignee|[plannerOrderHintsByAssignee](plannerorderhintsbyassignee.md)|Dicionário de dicas usadas para ordenar tarefas no modo de exibição AssignedTo do Quadro de Tarefas. A chave de cada entrada é um dos usuários aos qual a tarefa é atribuída e o valor é a dica de pedido. O formato de cada valor é definido como descrito [aqui](planner-order-hint-format.md).|
|unassignedOrderHint|Cadeia de caracteres|Valor de dica usado para ordenar a tarefa no modo de exibição AssignedTo do Quadro de Tarefas quando a tarefa não é atribuída a ninguém ou se o dicionário orderHintsByAssignee não fornecer uma dica de ordem para o usuário ao qual a tarefa é atribuída. O formato é definido como descrito [aqui](planner-order-hint-format.md).|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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

