---
title: tipo de recurso de sessão
description: O tipo de sessão
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d72ddd8273088fb7b1401d93e686914a69d18ebd
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394653"
---
# <a name="session-resource-type"></a>tipo de recurso de sessão

Namespace: Microsoft. Graph. callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma comunicação do usuário ou uma comunicação de reunião do usuário no caso de uma chamada em conferência.

## <a name="methods"></a>Methods

Não existem métodos para acessar diretamente as sessões. Use a API [Get callRecord](../api/callrecords-callrecord-get.md) com `$expand=sessions` para obter as sessões para um [callRecord](callrecords-callrecord.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|cadeia de caracteres|Identificador exclusivo da sessão. Somente leitura.|
|pelas|[Microsoft. Graph. callRecords. EndPoint](callrecords-endpoint.md)|Ponto de extremidade que iniciou a sessão.|
|receptor|[Microsoft. Graph. callRecords. EndPoint](callrecords-endpoint.md)|Ponto de extremidade que atendeu à sessão.|
|failureInfo|[Microsoft. Graph. callRecords. failureInfo](callrecords-failureinfo.md)|Informações de falha associadas à sessão se a sessão falhou.|
|modalidades|coleção de cadeias de caracteres|Lista de modalidades presentes na sessão. Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|startDateTime|DateTimeOffset|UTC fime quando o primeiro usuário ingressou na sessão. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|Hora UTC quando o último usuário saiu da sessão. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|


## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|segmentos|coleção [Microsoft. Graph. callRecords. Segment](callrecords-segment.md)|A lista de segmentos envolvidos na sessão. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.session",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "caller": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "callee": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "failureInfo": {"@odata.type": "microsoft.graph.callRecords.failureInfo"},
  "modalities": ["string"],
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "session resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->