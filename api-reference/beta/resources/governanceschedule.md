---
title: Tipo de recurso governanceSchedule
description: 'Representa a agenda de um governanceRoleAssignmentRequest. Para uma solicitação de atribuição de função, o agendamento controla quando executar a operação de atribuição de função, quando interromper a atribuição de função e com que frequência fará a operação de atribuição de função. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: f7583f15641c541493ded9f9a4779777e9f35f2a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722276"
---
# <a name="governanceschedule-resource-type"></a>Tipo de recurso governanceSchedule

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a agenda de [um governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md). Para uma solicitação de atribuição de função, o agendamento controla quando executar a operação de atribuição de função, quando interromper a atribuição de função e com que frequência fará a operação de atribuição de função.



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|startDateTime|DateTimeOffset|A hora de início da atribuição de função. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|endDateTime|DateTimeOffset|A hora de término da atribuição de função. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. *Observação: se o valor for `null` , ele indicará uma atribuição permanente.*|
|tipo|Cadeia de caracteres|O tipo de agendamento de atribuição de função. Por `Once` enquanto, só há suporte.
|duração|Duration|A duração de uma atribuição de função. Está no formato de um TimeSpan.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSchedule"
}-->

```json
{
  "duration": "String (timespan)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


