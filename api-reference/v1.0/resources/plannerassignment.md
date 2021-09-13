---
title: Tipo de recurso plannerAssignment
description: O **recurso plannerAssignment** representa a atribuição de uma tarefa a um usuário. Esse tipo é usado no tipo aberto plannerAssignments.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: ea71ff05e4c649712e9e37566dc8cc71e3529c76
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044360"
---
# <a name="plannerassignment-resource-type"></a>Tipo de recurso plannerAssignment

Namespace: microsoft.graph

O **recurso plannerAssignment** representa a atribuição de uma tarefa a um usuário. Esse tipo é usado no tipo aberto [plannerAssignments](plannerassignments.md).


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedBy|[identitySet](identityset.md)|A identidade do usuário que realizou a atribuição da tarefa, ou seja, o atribuídor.|
|assignedDateTime|DateTimeOffset|O momento em que a tarefa foi atribuída. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|orderHint|String|Dica usada para ordenar os atribuídos em uma tarefa. O formato é definido como descrito [aqui](planner-order-hint-format.md).|

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

