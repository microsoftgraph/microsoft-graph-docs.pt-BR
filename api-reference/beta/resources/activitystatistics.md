---
title: tipo de recurso activityStatistics
description: Representa o tempo gasto em atividades de trabalho, incluindo email, reuniões, trabalho de foco, chats e chamadas.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5cee94c1ff36bf30d977b7eb97d77f11d4d2ff5e
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450699"
---
# <a name="activitystatistics-resource-type"></a>tipo de recurso activityStatistics

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o tempo gasto por um usuário em várias atividades de trabalho durante e fora do horário de trabalho, para o intervalo de tempo especificado na solicitação, que usa um período de agregação de um dia.

Os seguintes tipos de estatísticas são derivados de **activityStatistics**:

* [Call](callactivitystatistics.md)
* [Chat](chatactivitystatistics.md)
* [Email](emailactivitystatistics.md)
* [Foco](focusactivitystatistics.md)
* [Atenda](meetingactivitystatistics.md)

### <a name="activity-id-property"></a>Propriedade ID da atividade

Em uma solicitação HTTP, para obter um tipo específico de estatísticas de atividade dentro de um intervalo de datas, você pode expressar essas informações como uma ID para a coleção de activityStatistics do usuário no seguinte formato `{startdate}` , `{enddate}` onde e são expressas no calendário ISO 8601 formato de data `{activity}` e pode ser "Call", "chat", "email", "foco" ou "reunião":

```
{activity}_{startdate}_{enddate}
```

Por exemplo, a ID "email_2019-08 -10 _2019-08-12" representa o emailActivityStatistics para o usuário especificado entre 10 de agosto de 2019 e 12 de agosto de 2019.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter activityStatistics](../api/activitystatistics-get.md) | [activityStatistics](activitystatistics.md) | Obter as propriedades das estatísticas de uma atividade especificada para um usuário, para o intervalo de tempo especificado. |
| [Listar activityStatistics](../api/activitystatistics-list.md) | [activityStatistics](activitystatistics.md) | Recupere as propriedades da coleção de estatísticas de atividade de um usuário para a última semana completa.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|atividade|analyticsActivityType| O tipo de atividade para a qual as estatísticas são retornadas. Os valores possíveis são: `call`, `chat`, `email`, `focus`e `meeting`.|
|duration|Duração|Total de horas gasto na atividade. O valor é representado no formato ISO 8601 para durações.|
|endDate|Data|Data em que a atividade foi concluída, expressada no formato ISO 8601 para datas do calendário. Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.|
|id|String| ID somente leitura da atividade, que representa `{activity}_{startdate}_{enddate}`.|
|startDate|Date|Data em que a atividade foi iniciada, expressa no formato ISO 8601 para datas do calendário. Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.|
|timeZoneUsed|String|O fuso horário que o usuário define no Microsoft Outlook é usado para a computação. Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".|

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