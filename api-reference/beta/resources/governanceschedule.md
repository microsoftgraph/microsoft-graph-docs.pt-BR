---
title: tipo de recurso de governanceSchedule
description: 'Representa o agendamento para um governanceRoleAssignmentRequest. Para uma solicitação de atribuição de função, controla a agenda quando executar a operação de atribuição de função, quando parar de atribuição de função e a frequência de realizar a operação de atribuição de função. '
localization_priority: Normal
ms.openlocfilehash: 8bf36b786adbd8064ee0c00c0ce293408c6e2b7f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882310"
---
# <a name="governanceschedule-resource-type"></a>tipo de recurso de governanceSchedule

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa o agendamento para um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md). Para uma solicitação de atribuição de função, controla a agenda quando executar a operação de atribuição de função, quando parar de atribuição de função e a frequência de realizar a operação de atribuição de função. 



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|startDateTime|DateTimeOffset|A hora de início da atribuição de função. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|A hora de término da atribuição de função. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. *Observação: se o valor for `null`, isso indica que uma atribuição permanente.*|
|type|Cadeia de caracteres|O tipo de agendamento de atribuição de função. Somente `Once` é suportado para agora.
|duration|Duração|A duração de uma atribuição de função. Ela está no formato de um TimeSpan.|

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
