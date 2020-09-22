---
title: tipo de recurso governanceSchedule
description: 'Representa o agendamento de um governanceRoleAssignmentRequest. Para uma solicitação de atribuição de função, o agendamento controla quando executar a operação de atribuição de função, quando parar a atribuição de função e com que frequência realizar a operação de atribuição de função. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 5d11f6c1dab607fea27ac71f3142f899a7183a79
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016671"
---
# <a name="governanceschedule-resource-type"></a>tipo de recurso governanceSchedule

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o agendamento de um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md). Para uma solicitação de atribuição de função, o agendamento controla quando executar a operação de atribuição de função, quando parar a atribuição de função e com que frequência realizar a operação de atribuição de função.



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|startDateTime|DateTimeOffset|A hora de início da atribuição de função. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|A hora de término da atribuição de função. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. *Observação: se o valor for `null` , ele indica uma atribuição permanente.*|
|tipo|String|O tipo de agendamento de atribuição de função. O só `Once` é suportado por enquanto.
|duration|Duração|A duração de uma atribuição de função. É no formato de um TimeSpan.|

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


