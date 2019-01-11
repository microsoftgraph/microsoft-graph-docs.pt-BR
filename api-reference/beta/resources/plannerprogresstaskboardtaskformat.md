---
title: Tipo de recurso plannerProgressTaskBoardTaskFormat
description: O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Progress do Quadro de Tarefas (uma exibição organizada pelo estado do campo PercentComplete no objeto da tarefa, com colunas para Não Iniciado, Em Andamento e Concluído). Cada tarefa terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
ms.openlocfilehash: 2f3395e0b63d038b8c280e54a76afcc2ca864789
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845581"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a>Tipo de recurso plannerProgressTaskBoardTaskFormat

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Progress do Quadro de Tarefas (uma exibição organizada pelo estado do campo PercentComplete no objeto da tarefa, com colunas para Não Iniciado, Em Andamento e Concluído). Cada [tarefa](plannertask.md) terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-get.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) |Leia as propriedades e as relações do objeto **plannerProgressTaskBoardTaskFormat**.|
|[Update](../api/plannerprogresstaskboardtaskformat-update.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)    |Atualize o objeto **plannerProgressTaskBoardTaskFormat**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| Somente leitura. ID do recurso. É 28 caracteres longos e diferencia maiusculas de minúsculas. [Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.|
|orderHint|String|Valor da dica usado para ordenar a tarefa no modo de exibição Progress do Quadro de Tarefas. O formato é definido como descrito [aqui](planner-order-hint-format.md).|

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
