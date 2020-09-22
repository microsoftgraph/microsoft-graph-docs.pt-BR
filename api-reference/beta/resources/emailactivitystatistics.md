---
title: tipo de recurso emailActivityStatistics
description: Representa informações adicionais sobre atividades de email para usuários
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: af0fbc4247e7ffc9c8285409789d0437d8e09cb5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055509"
---
# <a name="emailactivitystatistics-resource-type"></a>tipo de recurso emailActivityStatistics

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa dados sobre o tempo gasto pelo usuário em atividades de email no Microsoft Outlook. Isso é baseado no [activityStatistics](../resources/activitystatistics.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|atividade|analyticsActivityType| Atividade de email para a qual as estatísticas são retornadas.|
|duration|Duração|Total de horas gasto nos emails. O valor é representado no formato ISO 8601 para durações.|
|endDate|Data|Data de término da atividade de email. O valor é representado no formato ISO 8601 para datas do calendário. Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.|
|id|Cadeia de caracteres| ID somente leitura da atividade de email.|
|startDate|Data|Data de início da atividade de email. O valor é representado no formato ISO 8601 para datas do calendário. Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.|
|timeZoneUsed|Cadeia de caracteres|O fuso horário que o usuário define no calendário do Outlook é usado para a computação. Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".|
|afterHours|Duração|Total de horas gasto no email fora do horário de trabalho, que se baseia na configuração de calendário do Outlook do usuário para horário de trabalho. O valor é representado no formato ISO 8601 para durações. |
|readEmail|Duração|Total de horas gasto na leitura de email. O valor é representado no formato ISO 8601 para durações.|
|sentEmail|Duração|Total de horas gasto na gravação e envio de email. O valor é representado no formato ISO 8601 para durações.|

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
  "@odata.type": "microsoft.graph.emailActivityStatistics"
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
  "readEmail": "String (ISO 8601 duration)",
  "sentEmail": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

