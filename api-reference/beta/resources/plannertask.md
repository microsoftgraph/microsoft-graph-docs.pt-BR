---
title: tipo de recurso plannerTask
description: The **plannerTask** resource represents a Planner task in Microsoft 365. A Planner task is contained in a plan and can be assigned to a bucket in a plan. Each task object has a details object which can contain more information about the task. See overview for more information regarding relationships between group, plan and task.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 07374c6e8dc2dfaee1caba9f7283a1404627fb22
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897341"
---
# <a name="plannertask-resource-type"></a>tipo de recurso plannerTask

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The **plannerTask** resource represents a Planner task in Microsoft 365. A Planner task is contained in a [plan](plannerplan.md) and can be assigned to a [bucket](plannerbucket.md) in a plan. Each task object has a [details](plannertaskdetails.md) object which can contain more information about the task. See [overview](planner-overview.md) for more information regarding relationships between group, plan and task.


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
|appliedCategories|[plannerAppliedCategories](plannerappliedcategories.md)|The categories to which the task has been applied. See [applied Categories](plannerappliedcategories.md) for possible values.|
|assigneePriority|String|Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).|
|assignments|[plannerAssignments](plannerassignments.md)|O conjunto de destinatários aos quais a tarefa é atribuída.|
|bucketId|String|ID do bucket ao qual a tarefa pertence. O bucket precisa estar no plano no qual a tarefa está. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço. |
|checklistItemCount|Int32|Número de itens de lista de verificação que estão presentes na tarefa.|
|completedBy|[identitySet](identityset.md)|Identidade do usuário que concluiu a tarefa.|
|completedDateTime|DateTimeOffset|Read-only. Date and time at which the `'percentComplete'` of the task is set to `'100'`. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|conversationThreadId|String|Thread ID of the conversation on the task. This is the ID of the conversation thread object created in the group.|
|createdBy|[identitySet](identityset.md)|Identidade do usuário que criou a tarefa.|
|createdDateTime|DateTimeOffset|Read-only. Date and time at which the task is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|dueDateTime|DateTimeOffset|Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|hasDescription|Booliano|Read-only. Value is `true` if the details object of the task has a non-empty description and `false` otherwise.|
|id|String|Somente leitura. A ID da tarefa. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.|
|orderHint|String|Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).|
|percentComplete|Int32|Percentage of task completion. When set to `100`, the task is considered completed. |
|prioridade|Int32|Prioridade da tarefa. O intervalo de valores válido é entre `0` e `10` (inclusive), com o valor crescente sendo prioridade mais baixa ( `0` tem a maior prioridade e `10` tem a menor prioridade).  Atualmente, o Planner interpreta valores `0` e `1` como "urgente" `2` e como "importante", e como "médio" e `3` `4` `5` `6` `7` `8` , `9` e `10` como "baixo".  Atualmente, o Planner define o valor `1` para "urgente", `3` para "importante", `5` para "médio" e `9` para "baixo".|
|planId|String|ID do plano ao qual a tarefa pertence.|
|previewType|String|Isso define o tipo de visualização que aparece na tarefa. Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|referenceCount|Int32|Número de referências externas existentes na tarefa.|
|startDateTime|DateTimeOffset|Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|title|String|Título da tarefa.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedToTaskBoardFormat|[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)| Read-only. Nullable. Used to render the task correctly in the task board view when grouped by assignedTo.|
|bucketTaskBoardFormat|[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)| Read-only. Nullable. Used to render the task correctly in the task board view when grouped by bucket.|
|detalhes|[plannerTaskDetails](plannertaskdetails.md)| Read-only. Nullable. Additional details about the task.|
|progressTaskBoardFormat|[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)| Read-only. Nullable. Used to render the task correctly in the task board view when grouped by progress.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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
  "priority": 1024,
  "planId": "String",
  "previewType": "String",
  "referenceCount": 1024,
  "startDateTime": "String (timestamp)",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
