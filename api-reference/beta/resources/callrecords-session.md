---
title: tipo de recurso de sessão
description: O tipo de sessão
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 48983f3a6c4adf12184802722ba2607780c7b531
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720218"
---
# <a name="session-resource-type"></a>tipo de recurso de sessão

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma User-User ou uma comunicação User-Meeting no caso de uma chamada de conferência.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar sessões](../api/callrecords-session-list.md) | [coleção microsoft.graph.callRecords.session](callrecords-session.md) | Recupere a lista de sessões associadas a um [objeto callRecord.](callrecords-callrecord.md)
 |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|cadeia de caracteres|Identificador exclusivo da sessão. Somente leitura.|
|chamador|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|Ponto de extremidade que iniciou a sessão.|
|callee|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|Ponto de extremidade que atendeu a sessão.|
|failureInfo|[microsoft.graph.callRecords.failureInfo](callrecords-failureinfo.md)|Informações de falha associadas à sessão se a sessão falhou.|
|modalidades|coleção microsoft.graph.callRecords.modality|Lista de modalidades presentes na sessão. Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|startDateTime|DateTimeOffset|FIME UTC quando o primeiro usuário ingressou na sessão. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|endDateTime|DateTimeOffset|Hora UTC quando o último usuário saiu da sessão. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|


## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|segmentos|[coleção microsoft.graph.callRecords.segment](callrecords-segment.md)|A lista de segmentos envolvidos na sessão. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.session",
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

