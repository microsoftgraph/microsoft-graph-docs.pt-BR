---
title: Tipo de recurso callTranscriptEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre transcrição de chamada.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 00d5b1e4433cb74fdc1e0c023727a93cbd2ac54b
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534205"
---
# <a name="calltranscripteventmessagedetail-resource-type"></a>Tipo de recurso callTranscriptEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre transcrição de chamada.
Essa mensagem é gerada quando a transcrição está disponível para uma chamada.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|callId|Cadeia de Caracteres|Identificador exclusivo da chamada.|
|callTranscriptICalUid|Cadeia de Caracteres|Identificador exclusivo para uma transcrição de chamada.|
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