---
title: Tipo de recurso callRecord
description: Representa uma única chamada ponto a ponto ou uma chamada de grupo entre vários participantes, às vezes chamada de reunião online.
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e0d9c93d696df969dd3cf78939d81a41385c8084
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58772223"
---
# <a name="callrecord-resource-type"></a>Tipo de recurso callRecord

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma única chamada ponto a ponto ou uma chamada de grupo entre vários participantes, às vezes chamada de reunião online.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter callRecord](../api/callrecords-callrecord-get.md) | [microsoft.graph.callRecords.callRecord](callrecords-callrecord.md) | Leia as propriedades e as relações de um **objeto callRecord.** |
| [getPstnCalls](../api/callrecords-callrecord-getpstncalls.md) | [coleção microsoft.graph.callRecords.pstnCallLogRow](callrecords-pstncalllogrow.md) | Listar **objetos pstnCallLogRow** em um registro de chamada. |
| [getDirectRoutingCalls](../api/callrecords-callrecord-getdirectroutingcalls.md) | [coleção microsoft.graph.callRecords.directRoutingLogRow](callrecords-directroutinglogrow.md)| Listar **objetos directRoutingLogRow** para um registro de chamada. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|Hora UTC quando o último usuário deixou a chamada. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|id|Cadeia de caracteres|Identificador exclusivo do registro de chamada. Somente leitura.|
|joinWebUrl|Cadeia de caracteres|URL de reunião associada à chamada. Pode não estar disponível para um tipo de registro de chamada peerToPeer.|
|lastModifiedDateTime|DateTimeOffset|Hora UTC quando o registro de chamada foi criado. O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|modalidades|coleção modality|Lista de todas as modalidades usadas na chamada. Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|organizer|[identitySet](identityset.md)|A identidade da parte organizadora.|
|participantes|Coleção [identitySet](identityset.md)|Lista de identidades distintas envolvidas na chamada.|
|startDateTime|DateTimeOffset|Hora UTC quando o primeiro usuário ingressou na chamada. O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|tipo|callType|Indica o tipo da chamada. Os valores possíveis são: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.|
|versão|Int64|Versão de aumento monótono do registro de chamada. Registros de chamada de versão superior com a mesma ID incluem dados adicionais em comparação com a versão inferior.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|sessões|[coleção microsoft.graph.callRecords.session](callrecords-session.md)|Lista de sessões envolvidas na chamada. As chamadas ponto a ponto geralmente têm apenas uma sessão, enquanto as chamadas de grupo geralmente têm pelo menos uma sessão por participante. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.callRecord",
  "keyProperty": "id"
}-->

```json
{
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "modalities": ["string"],
  "organizer": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}],
  "startDateTime": "String (timestamp)",
  "type": "string",
  "version": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


