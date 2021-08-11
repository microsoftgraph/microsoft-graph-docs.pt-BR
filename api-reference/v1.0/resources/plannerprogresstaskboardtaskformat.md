---
title: Tipo de recurso plannerProgressTaskBoardTaskFormat
description: O **recurso plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente na exibição Progresso do Quadro de Tarefas (uma exibição organizada pelo estado do campo PercentComplete no objeto de tarefa, com colunas para Não Iniciado, Em Andamento e Concluído). Cada tarefa terá um **objeto plannerProgressTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9715fb55187a3d48ea8d21f5bd088dbfb2e08f189ed9c96e66e747c100a1272f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218433"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a>Tipo de recurso plannerProgressTaskBoardTaskFormat

Namespace: microsoft.graph

O **recurso plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente na exibição Progresso do Quadro de Tarefas (uma exibição organizada pelo estado do campo PercentComplete no objeto de tarefa, com colunas para Não Iniciado, Em Andamento e Concluído). Cada [tarefa](plannertask.md) terá um **objeto plannerProgressTaskBoardTaskFormat** associado a ela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-get.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) |Ler propriedades e relações do **objeto plannerProgressTaskBoardTaskFormat.**|
|[Atualizar](../api/plannerprogresstaskboardtaskformat-update.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)    |Atualize **o objeto plannerProgressTaskBoardTaskFormat.** |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID do recurso. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.|
|orderHint|String|Valor de dica usado para ordenar a tarefa no modo de exibição Progresso do Quadro de Tarefas. O formato é definido como descrito [aqui](planner-order-hint-format.md).|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

