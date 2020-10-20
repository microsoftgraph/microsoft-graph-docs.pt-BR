---
title: tipo de recurso callRecord
description: O tipo callRecord
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cf438689ec873ba915c735fee7ebc2162757f8ff
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601367"
---
# <a name="callrecord-resource-type"></a>tipo de recurso callRecord

Namespace: microsoft.graph.callRecords

Representa uma única chamada ponto a ponto ou uma chamada de grupo entre vários participantes, às vezes chamada de reunião online.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter callRecord](../api/callrecords-callrecord-get.md) | [Microsoft. Graph. callRecords. callRecord](callrecords-callrecord.md) | Leia as propriedades e os relacionamentos do objeto callRecord. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|Hora UTC quando o último usuário saiu da chamada. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|String|Identificador exclusivo do registro de chamada. Somente leitura.|
|joinWebUrl|String|URL de reunião associada à chamada. Pode não estar disponível para um tipo de registro de chamada peerToPeer.|
|lastModifiedDateTime|DateTimeOffset|Hora UTC quando o registro de chamada foi criado. O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|modalidades|coleção de modalidades de Microsoft. Graph. callRecords.|Lista de todas as modalidades usadas na chamada. Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|organizer|[identitySet](identityset.md)|A identidade da parte de organização.|
|participantes|Coleção [identitySet](identityset.md)|Lista de identidades distintas envolvidas na chamada.|
|startDateTime|DateTimeOffset|Hora UTC quando o primeiro usuário ingressou na chamada. O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|type|Microsoft. Graph. callRecords. CallType|Indica o tipo da chamada. Os valores possíveis são: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.|
|versão|Int64|Versão de aumento monotônico do registro de chamada. Registros de chamada de versão superior com a mesma ID incluem dados adicionais comparados à versão inferior.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|sessões|coleção [Microsoft. Graph. callRecords. Session](callrecords-session.md)|Lista de sessões envolvidas na chamada. As chamadas ponto a ponto normalmente têm apenas uma sessão, enquanto as chamadas de grupo normalmente têm pelo menos uma sessão por participante. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.callRecord",
  "baseType": "",
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
