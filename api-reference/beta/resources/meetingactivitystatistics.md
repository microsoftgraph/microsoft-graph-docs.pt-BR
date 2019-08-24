---
title: tipo de recurso meetingActivityStatistics
description: Representa informações sobre as atividades de reunião para os usuários.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 14d926a41680f1292b7599bd76b458705b426719
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622534"
---
# <a name="meetingactivitystatistics-resource-type"></a>tipo de recurso meetingActivityStatistics

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa dados sobre o tempo gasto pelo usuário em reuniões no Microsoft Outlook, Microsoft Teams ou Skype for Business. Isso é baseado no [activityStatistics](../resources/activitystatistics.md).
<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get meetingActivityStatistics](../api/meetingactivitystatistics-get.md) | [meetingActivityStatistics](meetingactivitystatistics.md) | Read properties and relationships of meetingActivityStatistics object; name of the activity for which statistics are returned as “meeting.” |
-->
## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|atividade|analyticsActivityType| Atividade de reunião para a qual as estatísticas são retornadas.|
|duration|Duração|Total de horas gasto em reuniões. O valor é representado no formato ISO 8601 para durações.|
|endDate|Data|Data de término da atividade da reunião. O valor é representado no formato ISO 8601 para datas do calendário. Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.|
|id|String| ID somente leitura da atividade da reunião.|
|startDate|Date|Data de início da atividade da reunião. O valor é representado no formato ISO 8601 para datas do calendário. Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.|
|timeZoneUsed|String|O fuso horário do Outlook definido pelo usuário no calendário do Outlook é usado para a computação. Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".|
|afterHours|Duração|Tempo gasto em reuniões fora do horário de trabalho, que se baseia na configuração de calendário do Outlook do usuário para horário de trabalho. O valor é representado no formato ISO 8601 para durações.|
|conflitantes|Duração|Tempo gasto em reuniões conflitantes (reuniões que se sobrepõem a outras reuniões que a pessoa aceitou e onde o status da pessoa está definido como ocupado). O valor é representado no formato ISO 8601 para durações.|
|long|Duração|Tempo gasto em reuniões longas (mais de uma hora em duração). O valor é representado no formato ISO 8601 para durações.|
|multitarefas|Duração|Tempo gasto em reuniões em que a pessoa estava multitarefa (leitura/envio de mais de um número mínimo de emails e/ou envio de mais de um número mínimo de mensagens no Microsoft Teams ou no Skype for Business). O valor é representado no formato ISO 8601 para durações.|
|organiza|Duração|Tempo gasto em reuniões organizadas pelo usuário. O valor é representado no formato ISO 8601 para durações.|
|recorrente|Duração|Tempo gasto em reuniões recorrentes. O valor é representado no formato ISO 8601 para durações.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)",
  "conflicting": "String (ISO 8601 duration)",
  "long": "String (ISO 8601 duration)",
  "multitasking": "String (ISO 8601 duration)",
  "organized": "String (ISO 8601 duration)",
  "recurring": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->