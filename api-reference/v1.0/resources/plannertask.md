---
title: tipo de recurso plannerTask
description: O recurso **plannerTask** representa uma tarefa do Planner no Microsoft 365. Uma tarefa do Planner está contida em um plano e pode ser atribuída a um bucket em um plano. Cada objeto de tarefa tem um objeto de detalhes que pode conter mais informações sobre a tarefa. Confira a visão geral para obter mais informações sobre as relações entre o grupo, o plano e a tarefa.
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 0504168a280c75d15276fbb1fa097c84cafcc1ce
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720603"
---
# <a name="plannertask-resource-type"></a>tipo de recurso plannerTask

Namespace: microsoft.graph

O recurso **plannerTask** representa uma tarefa do Planner no Microsoft 365. Uma tarefa do Planner está contida em um [plano](plannerplan.md) e pode ser atribuída a um [bucket](plannerbucket.md) em um plano. Cada objeto de tarefa tem um objeto de [detalhes](plannertaskdetails.md) que pode conter mais informações sobre a tarefa. Confira a [visão geral](planner-overview.md) para obter mais informações sobre as relações entre o grupo, o plano e a tarefa.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter plannerTask](../api/plannertask-get.md) | [plannerTask](plannertask.md) |Leia as propriedades e as relações do objeto **plannerTask**.|
|[Update](../api/plannertask-update.md) | [plannerTask](plannertask.md) |Atualizar o objeto **plannerTask**. |
|[Delete](../api/plannertask-delete.md) | Nenhum |Excluir o objeto **plannerTask**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|activeChecklistItemCount|Int32|Número de itens de lista de verificação com valor definido como `false`, representando itens incompletos.|
|appliedCategories|[plannerAppliedCategories](plannerappliedcategories.md)|As categorias às quais a tarefa foi aplicada. Confira os possíveis valores em [Categorias aplicadas](plannerappliedcategories.md).|
|assigneePriority|String|Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](planner-order-hint-format.md).|
|assignments|[plannerAssignments](plannerassignments.md)|O conjunto de destinatários aos quais a tarefa é atribuída.|
|bucketId|String|ID do bucket ao qual a tarefa pertence. O bucket precisa estar no plano no qual a tarefa está. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço. |
|checklistItemCount|Int32|Número de itens de lista de verificação que estão presentes na tarefa.|
|completedBy|[identitySet](identityset.md)|Identidade do usuário que concluiu a tarefa.|
|completedDateTime|DateTimeOffset|Somente leitura. A data e a hora na qual o `'percentComplete'` da tarefa está definido como `'100'`. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|conversationThreadId|String|Identificação do thread da conversa na tarefa. Essa é a identificação do objeto do thread da conversa criado no grupo.|
|createdBy|[identitySet](identityset.md)|Identidade do usuário que criou a tarefa.|
|createdDateTime|DateTimeOffset|Somente leitura. A data e a hora que a tarefa é criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|dueDateTime|DateTimeOffset|A data e a hora que a tarefa já deve estar concluída. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|hasDescription|Booliano|Somente leitura. O valor é `true` se o objeto de detalhes da tarefa tem uma descrição não vazia e `false` caso contrário.|
|id|String|Somente leitura. A ID da tarefa. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.|
|orderHint|String|Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](planner-order-hint-format.md).|
|percentComplete|Int32|A porcentagem de conclusão da tarefa. Quando definido como `100`, a tarefa será considerada concluída. |
|planId|String|ID do plano ao qual a tarefa pertence.|
|previewType|String|Isso define o tipo de visualização que aparece na tarefa. Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|referenceCount|Int32|Número de referências externas existentes na tarefa.|
|startDateTime|DateTimeOffset|A data e a hora que a tarefa começa. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|title|String|Título da tarefa.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedToTaskBoardFormat|[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)| Somente leitura. Anulável. Usado para renderizar a tarefa corretamente na exibição de quadro de tarefa quando agrupado por assignedTo.|
|bucketTaskBoardFormat|[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)| Somente leitura. Anulável. Usado para renderizar a tarefa corretamente na exibição de quadro de tarefa quando agrupado por bucket.|
|detalhes|[plannerTaskDetails](plannertaskdetails.md)| Somente leitura. Anulável. Outros detalhes sobre a tarefa.|
|progressTaskBoardFormat|[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)| Somente leitura. Anulável. Usado para renderizar a tarefa corretamente na exibição de quadro de tarefa quando agrupado por progresso.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTask"
}-->

```json
{
  "activeChecklistItemCount": 1024,
  "appliedCategories": {"@odata.type": "microsoft.graph.plannerAppliedCategories"},
  "assigneePriority": "String",
  "assignments": {"@odata.type": "microsoft.graph.plannerAssignments"},
  "bucketId": "String",
  "checklistItemCount": 1024,
  "completedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "completedDateTime": "String (timestamp)",
  "conversationThreadId": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "hasDescription": true,
  "id": "String (identifier)",
  "orderHint": "String",
  "percentComplete": 1024,
  "planId": "String",
  "previewType": "String",
  "referenceCount": 1024,
  "startDateTime": "String (timestamp)",
  "title": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

