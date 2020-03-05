---
title: tipo de recurso callActivityStatistics
description: Representa informações sobre as atividades de chamada para os usuários.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 03625811beec7df8cd679455e9853ea49edf0ed6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507814"
---
# <a name="callactivitystatistics-resource-type"></a>tipo de recurso callActivityStatistics

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa dados sobre o tempo gasto pelo usuário em atividades de chamada no Microsoft Teams ou no Skype for Business. Isso é baseado no [activityStatistics](../resources/activitystatistics.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|atividade|analyticsActivityType| Atividade de chamada para a qual as estatísticas são retornadas.|
|duration|Duração|Total de horas gasto em chamadas. O valor é representado no formato ISO 8601 para durações.|
|endDate|Data|Data de término da atividade de chamada. O valor é representado no formato ISO 8601 para datas do calendário. Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.|
|id|String| Somente leitura ID para a atividade de chamada.|
|startDate|Date|Data de início da atividade de chamada. O valor é representado no formato ISO 8601 para datas do calendário. Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.|
|timeZoneUsed|String|O fuso horário que o usuário define no calendário do Microsoft Outlook é usado para a computação. Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".|
|afterHours|Duração|Tempo gasto em chamadas fora do horário de trabalho, que se baseia na configuração de calendário do Outlook do usuário para horário de trabalho. O valor é representado no formato ISO 8601 para durações. |

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
  "@odata.type": "microsoft.graph.callActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->