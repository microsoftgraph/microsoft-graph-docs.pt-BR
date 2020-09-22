---
title: tipo de recurso activityStatistics
description: Representa o tempo gasto em atividades de trabalho, incluindo email, reuniões, trabalho de foco, chats e chamadas.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: e94f9ad746c497e3b81eff6b919c50a59c6a0a11
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004274"
---
# <a name="activitystatistics-resource-type"></a>tipo de recurso activityStatistics

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o tempo gasto por um usuário em várias atividades de trabalho durante e fora do horário de trabalho, para o intervalo de tempo especificado na solicitação, que usa um período de agregação de um dia.

Os seguintes tipos de estatísticas são derivados de **activityStatistics**:

* [Call](callactivitystatistics.md)
* [Chat](chatactivitystatistics.md)
* [Email](emailactivitystatistics.md)
* [Foco](focusactivitystatistics.md)
* [Atenda](meetingactivitystatistics.md)

<!--  removing per Mathew 2/6/2020   ### Activity id property

In an HTTP request, to get a specific type of activity statistics within a date range, you can express this information as an ID to the user's collection of activityStatistics in the following format, where `{startdate}` and `{enddate}` are expressed in ISO 8601 calendar date format and `{activity}` can be "call", "chat", "email", "focus", or "meeting":

```
{activity}_{startdate}_{enddate}
```

For example, the ID "email_2019-08-10_2019-08-12" represents the emailActivityStatistics for the specified user between August 10, 2019 and August 12, 2019.
-->
## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar activityStatistics](../api/activitystatistics-list.md) | [activityStatistics](activitystatistics.md) | Recupere as propriedades da coleção de estatísticas de atividade de um usuário para a última semana completa. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|atividade |analyticsActivityType |O tipo de atividade para a qual as estatísticas são retornadas. Os valores possíveis são: `call` , `chat` , `email` , `focus` e `meeting` . |
|duration |Duração |Total de horas gasto na atividade. O valor é representado no formato ISO 8601 para durações. |
|endDate |Data |Data em que a atividade foi concluída, expressada no formato ISO 8601 para datas do calendário. Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD. |
|id |String |ID somente leitura da atividade. Não analise ou personalize o valor para seus cenários. |
|startDate |Data |Data em que a atividade foi iniciada, expressa no formato ISO 8601 para datas do calendário. Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD. |
|timeZoneUsed |String |O fuso horário que o usuário define no Microsoft Outlook é usado para a computação. Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico". |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- { 
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activityStatistics",
  "keyProperty": "id"
}-->

```json
{
  "activity": "String",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601 format)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601 format)",
  "timeZoneUsed": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}--> 

