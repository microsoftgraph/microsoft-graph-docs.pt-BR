---
title: tipo de recurso callRecordingEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre a gravação de chamada.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8c0730eaef43904ddbda314543ba623ee72fb325
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535666"
---
# <a name="callrecordingeventmessagedetail-resource-type"></a>tipo de recurso callRecordingEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre a gravação de chamada.
Essa mensagem é gerada quando uma gravação de chamada é iniciada.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|callId|Cadeia de Caracteres|Identificador exclusivo da chamada.|
|callRecordingDisplayName|Cadeia de Caracteres|Nome de exibição para a gravação de chamada.|
|callRecordingDuration|Duration|Duração da gravação de chamada.|
|callRecordingStatus|callRecordingStatus|Status da gravação de chamada. Os valores possíveis são: `success`, `failure`, `initial`, `chunkFinished`, `unknownFutureValue`.|
|callRecordingUrl|Cadeia de Caracteres|URL de gravação de chamada.|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|meetingOrganizer|[identitySet](../resources/identityset.md)|Organizador da reunião.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecordingEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecordingEventMessageDetail",
  "callId": "String",
  "callRecordingDisplayName": "String",
  "callRecordingUrl": "String",
  "callRecordingDuration": "String (duration)",
  "callRecordingStatus": "String",
  "meetingOrganizer": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre gravação de chamada](/graph/system-messages/#call-recording)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).

