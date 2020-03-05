---
title: tipo de recurso plannerProgressTaskBoardTaskFormat
description: O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição de progresso do quadro de tarefas (um modo organizado pelo estado do campo PercentComplete no objeto Task, com as colunas não iniciadas, em andamento e concluída). Cada tarefa terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 7be6483f127910224b05e05fdf885780d8767176
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521668"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a>tipo de recurso plannerProgressTaskBoardTaskFormat

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição de progresso do quadro de tarefas (um modo organizado pelo estado do campo PercentComplete no objeto Task, com as colunas não iniciadas, em andamento e concluída). Cada [tarefa](plannertask.md) terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-get.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) |Leia as propriedades e os relacionamentos do objeto **plannerProgressTaskBoardTaskFormat** .|
|[Update](../api/plannerprogresstaskboardtaskformat-update.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)    |Atualize o objeto **plannerProgressTaskBoardTaskFormat** . |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID do recurso. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.|
|orderHint|String|O valor de dica usado para ordenar a tarefa no modo de exibição de progresso do quadro de tarefas. O formato é definido conforme descrito [aqui](planner-order-hint-format.md).|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
