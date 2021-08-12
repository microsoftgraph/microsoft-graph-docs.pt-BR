---
title: Tipo de recurso plannerBucketTaskBoardTaskFormat
description: O **recurso plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente na exibição Buckets do Quadro de Tarefas (uma exibição organizada por tarefas dentro dos buckets aos que são atribuídas). Cada tarefa terá um **objeto plannerBucketTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 38e159858591f7e1725c455e07162f9e0f10bbd1f8fc8d8bcfe974e952c95ae6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178112"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a>Tipo de recurso plannerBucketTaskBoardTaskFormat

Namespace: microsoft.graph

O **recurso plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente na exibição Buckets do Quadro de Tarefas (uma exibição organizada por tarefas dentro dos buckets aos que são atribuídas). Cada [tarefa](plannertask.md) terá um **objeto plannerBucketTaskBoardTaskFormat** associado a ela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat-get.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) |Ler propriedades e relações do **objeto plannerBucketTaskBoardTaskFormat.**|
|[Atualizar](../api/plannerbuckettaskboardtaskformat-update.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)  |Atualize **o objeto plannerBucketTaskBoardTaskFormat.** |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID do recurso. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.|
|orderHint|String|Dica usada para ordenar tarefas no modo de exibição Bucket do Quadro de Tarefas. O formato é definido como descrito [aqui](planner-order-hint-format.md).|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
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
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

