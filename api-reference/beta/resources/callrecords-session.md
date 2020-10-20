---
title: tipo de recurso de sessão
description: O tipo de sessão
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 91683b4bd9568d14a7049a74d997564b570e4f26
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48600968"
---
# <a name="session-resource-type"></a>tipo de recurso de sessão

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma comunicação de User-User ou uma comunicação de User-Meeting no caso de uma chamada em conferência.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar sessões](../api/callrecords-session-list.md) | coleção [Microsoft. Graph. callRecords. Session](callrecords-session.md) | Recupere a lista de sessões associadas a um objeto [callRecord](callrecords-callrecord.md) .
 |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|string|Identificador exclusivo da sessão. Somente leitura.|
|pelas|[Microsoft. Graph. callRecords. EndPoint](callrecords-endpoint.md)|Ponto de extremidade que iniciou a sessão.|
|receptor|[Microsoft. Graph. callRecords. EndPoint](callrecords-endpoint.md)|Ponto de extremidade que atendeu à sessão.|
|failureInfo|[Microsoft. Graph. callRecords. failureInfo](callrecords-failureinfo.md)|Informações de falha associadas à sessão se a sessão falhou.|
|modalidades|coleção de modalidades de Microsoft. Graph. callRecords.|Lista de modalidades presentes na sessão. Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
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

