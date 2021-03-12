---
title: tipo de recurso segment
description: O tipo de segmento
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 886ea3661c83d6a84f9e171a11eee927920a8077
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722241"
---
# <a name="segment-resource-type"></a>tipo de recurso segment

Namespace: microsoft.graph.callRecords

Representa uma parte de uma comunicação User-User ou uma User-Meeting no caso de uma chamada de conferência. Uma chamada VOIP típica terá um segmento por sessão. Em determinados cenários, como chamadas PSTN, haverá vários segmentos por sessão devido à comunicação de servidor para servidor adicional necessária para conectar a chamada.

## <a name="methods"></a>Methods

Não existem métodos para acessar diretamente segmentos. Use a api [Get callRecord](../api/callrecords-callrecord-get.md) com ou a api de sessão list com para obter os `$expand=sessions($expand=segments)` [](../api/callrecords-session-list.md) `$expand=segments` segmentos de um [callRecord](callrecords-callrecord.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|Identificador exclusivo do segmento. Somente leitura.|
|chamador|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|Ponto de extremidade que iniciou esse segmento.|
|callee|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|Ponto de extremidade que respondeu a esse segmento.|
|failureInfo|[microsoft.graph.callRecords.failureInfo](callrecords-failureinfo.md)|Informações de falha associadas ao segmento se falharem.|
|mídia|[coleção microsoft.graph.callRecords.media](callrecords-media.md)|Mídia associada a esse segmento.|
|startDateTime|DateTimeOffset|Hora UTC quando o segmento foi iniciado. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|endDateTime|DateTimeOffset|Hora UTC quando o segmento terminou. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|

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
