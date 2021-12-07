---
title: tipo de recurso callRecordingEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre a gravação de chamada.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b37d49f0b13aa9da1445f74b74011f3bdc129112
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322341"
---
# <a name="callrecordingeventmessagedetail-resource-type"></a>tipo de recurso callRecordingEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre a gravação de chamada.
Essa mensagem é gerada quando uma gravação de chamada é iniciada.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|callId|String|Identificador exclusivo da chamada.|
|callRecordingDisplayName|String|Nome de exibição para a gravação de chamada.|
|callRecordingDuration|Duração|Duração da gravação de chamada.|
|callRecordingStatus|callRecordingStatus|Status da gravação de chamada. Os valores possíveis são: `success`, `failure`, `initial`, `chunkFinished`, `unknownFutureValue`.|
|callRecordingUrl|String|URL de gravação de chamada.|
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

