---
title: tipo de recurso Segment
description: O tipo de segmento
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0d1047c0a83954acb393e5f4fd2879c5ab6c3ae5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046922"
---
# <a name="segment-resource-type"></a>tipo de recurso Segment

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma parte de uma comunicação do usuário ou uma comunicação de reunião do usuário no caso de uma chamada em conferência. Uma chamada VOIP típica terá um segmento por sessão. Em determinados cenários, como chamadas PSTN, haverá vários segmentos por sessão, devido à comunicação adicional de servidor para servidor necessária para conectar a chamada.

## <a name="methods"></a>Métodos

Não existem métodos para acessar diretamente os segmentos. Use a API [Get callRecord](../api/callrecords-callrecord-get.md) com `$expand=sessions($expand=segments)` ou a API de [sessão de lista](../api/callrecords-session-list.md) com `$expand=segments` para obter os segmentos de um [callRecord](callrecords-callrecord.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|Identificador exclusivo do segmento. Somente leitura.|
|pelas|[Microsoft. Graph. callRecords. EndPoint](callrecords-endpoint.md)|Ponto de extremidade que iniciou este segmento.|
|receptor|[Microsoft. Graph. callRecords. EndPoint](callrecords-endpoint.md)|Ponto de extremidade que respondeu a este segmento.|
|failureInfo|[Microsoft. Graph. callRecords. failureInfo](callrecords-failureinfo.md)|Informações de falha associadas ao segmento se ele falhar.|
|mídia|coleção [Microsoft. Graph. callRecords. Media](callrecords-media.md)|Mídia associada a este segmento.|
|startDateTime|DateTimeOffset|Hora UTC quando o segmento é iniciado. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|Hora UTC em que o segmento terminou. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.segment",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "caller": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "callee": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "failureInfo": {"@odata.type": "microsoft.graph.callRecords.failureInfo"},
  "media": [{"@odata.type": "microsoft.graph.callRecords.media"}],
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "segment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

