---
title: tipo de recurso focusActivityStatistics
description: Representa informações sobre o trabalho de foco individual para usuários
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3da2dc2719f24bfd986d5a3df550b4635b734131
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052877"
---
# <a name="focusactivitystatistics-resource-type"></a>tipo de recurso focusActivityStatistics

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa dados sobre o tempo do usuário disponível para trabalho de foco. Isso é baseado no [activityStatistics](../resources/activitystatistics.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|atividade|analyticsActivityType| Atividade de foco para a qual as estatísticas são retornadas.|
|duration|Duração|Soma total de horas de foco, que é igual a todos os blocos de tempo de pelo menos duas horas consecutivas, no calendário do Microsoft Outlook de um usuário sem uma reunião com outras pessoas dentro do horário de trabalho definido pelo usuário. O valor é representado no formato ISO 8601 para durações.|
|endDate|Data|Data de término da atividade de foco. O valor é representado no formato ISO 8601 para datas do calendário. Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.|
|id|Cadeia de caracteres| Somente leitura ID para a atividade Focus.|
|startDate|Data|Data de início da atividade de foco. O valor é representado no formato ISO 8601 para datas do calendário. Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.|
|timeZoneUsed|Cadeia de caracteres|O fuso horário que o usuário define no calendário do Outlook é usado para a computação. Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".|

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
  "@odata.type": "microsoft.graph.focusActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String"
  }
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "focusActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

