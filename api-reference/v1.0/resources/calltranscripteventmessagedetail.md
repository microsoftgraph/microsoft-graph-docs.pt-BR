---
title: Tipo de recurso callTranscriptEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre transcrição de chamada.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5a57a6f5fc98fb518cf55d56c784fb86ec4c8aab
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322310"
---
# <a name="calltranscripteventmessagedetail-resource-type"></a>Tipo de recurso callTranscriptEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre transcrição de chamada.
Essa mensagem é gerada quando a transcrição está disponível para uma chamada.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|callId|String|Identificador exclusivo da chamada.|
|callTranscriptICalUid|String|Identificador exclusivo para uma transcrição de chamada.|
|meetingOrganizer|[identitySet](../resources/identityset.md)|O organizador da reunião.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callTranscriptEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callTranscriptEventMessageDetail",
  "callId": "String",
  "callTranscriptICalUid": "String",
  "meetingOrganizer": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre transcrição de chamada](/graph/system-messages/#call-transcript)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
