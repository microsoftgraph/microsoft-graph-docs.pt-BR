---
title: tipo de recurso plannerAssignment
description: O recurso **plannerAssignment** representa a atribuição de uma tarefa a um usuário. Esse tipo é usado no tipo aberto plannerAssignments.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 5ae09a6c528e0311c542283ea5929ffba88ba029
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447140"
---
# <a name="plannerassignment-resource-type"></a>tipo de recurso plannerAssignment

Namespace: Microsoft. Graph

O recurso **plannerAssignment** representa a atribuição de uma tarefa a um usuário. Esse tipo é usado no tipo aberto [plannerAssignments](plannerassignments.md).


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedBy|[identitySet](identityset.md)|A identidade do usuário que realizou a atribuição da tarefa, ou seja, o destinatário.|
|assignedDateTime|DateTimeOffset|O horário em que a tarefa foi atribuída. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|orderHint|String|Dica usada para ordenar destinatários em uma tarefa. O formato é definido conforme descrito [aqui](planner-order-hint-format.md).|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignment"
}-->

```json
{
  "assignedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
