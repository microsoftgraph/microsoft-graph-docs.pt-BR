---
title: tipo de recurso educationAssignmentPointsGrade
description: Quando uma tarefa é definida como um tipo de nota de pontos, cada envio terá esse objeto associado à propriedade **submission.grade** . Isso cria uma subclasse de educationAssignmentGrade,
ms.localizationpriority: medium
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 76fdaab98599dc74b7ddcc11fdad3827f5622691
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684505"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>tipo de recurso educationAssignmentPointsGrade

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Quando uma tarefa é definida como um tipo de nota de pontos, cada envio terá esse objeto associado à propriedade **submission.grade** . Isso cria uma subclasse [de educationAssignmentGrade](educationassignmentgrade.md), que adicionará os dados de quem a essa propriedade. Os pontos máximos são armazenados na **propriedade assignments.grading** .


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|points|Único|Número de pontos que um professor está dando a esse objeto de envio.|
|gradedBy|[identitySet](identityset.md)| Usuário que fez a classificação. |
|gradedDateTime|DateTimeOffset| Momento no tempo em que a nota foi aplicada a este objeto de envio. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Double",
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


