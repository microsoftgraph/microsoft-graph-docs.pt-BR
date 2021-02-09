---
title: tipo de recurso segment
description: O tipo de segmento
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ef965bcfb10eeafd0a2c4f58351aa74650abcd05
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159637"
---
# <a name="segment-resource-type"></a>tipo de recurso segment

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma parte de uma User-User comunicação ou uma User-Meeting no caso de uma chamada de conferência. Uma chamada VOIP típica terá um segmento por sessão. Em determinados cenários, como chamadas PSTN, haverá vários segmentos por sessão devido à comunicação adicional entre servidores necessária para conectar a chamada.

## <a name="methods"></a>Métodos

Não existem métodos para acessar diretamente segmentos. Use a api [Obter callRecord](../api/callrecords-callrecord-get.md) com ou a api de sessão de lista com para `$expand=sessions($expand=segments)` obter os [](../api/callrecords-session-list.md) `$expand=segments` segmentos de um [callRecord](callrecords-callrecord.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|Identificador exclusivo do segmento. Somente leitura.|
|chamador|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|Ponto de extremidade que iniciou esse segmento.|
|destinatário da chamada|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|Ponto de extremidade que atendeu esse segmento.|
|failureInfo|[microsoft.graph.callRecords.failureInfo](callrecords-failureinfo.md)|Informações de falha associadas ao segmento em caso de falha.|
|mídia|[coleção microsoft.graph.callRecords.media](callrecords-media.md)|Mídia associada a este segmento.|
|startDateTime|DateTimeOffset|Horário UTC quando o segmento foi iniciado. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|Hora UTC quando o segmento terminou. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.segment",
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

