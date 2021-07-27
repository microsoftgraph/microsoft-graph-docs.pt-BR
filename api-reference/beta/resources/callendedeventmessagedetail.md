---
title: Tipo de recurso callEndedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma chamada encerrada.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3ff10e7d9cdd73df3f2db8171795a5d0ae5f61d3
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534209"
---
# <a name="callendedeventmessagedetail-resource-type"></a>Tipo de recurso callEndedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre uma chamada encerrada.
Essa mensagem é gerada quando uma chamada termina.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|callDuration|Duration|Duração da chamada.|
|callEventType|teamworkCallEventType|Representa o tipo de evento de chamada. Os valores possíveis são: `call`, `meeting`, `screenShare`, `unknownFutureValue`.|
|callId|Cadeia de Caracteres|Identificador exclusivo da chamada.|
|callParticipants|[Coleção callParticipantInfo](../resources/callparticipantinfo.md)|Lista de participantes de chamada.|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callEndedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callEndedEventMessageDetail",
  "callId": "String",
  "callParticipants": [
    {
      "@odata.type": "microsoft.graph.callParticipantInfo"
    }
  ],
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "callDuration": "String (duration)",
  "callEventType": "String"
}
```

## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre uma chamada encerrada](/graph/system-messages/#call-ended)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).

