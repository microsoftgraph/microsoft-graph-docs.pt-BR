---
title: Tipo de recurso callStartedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre a chamada iniciada.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: de887904a352749b2a8edd3e9b4d5554e0f34d49
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534204"
---
# <a name="callstartedeventmessagedetail-resource-type"></a>Tipo de recurso callStartedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre a chamada iniciada.
Essa mensagem é gerada quando uma chamada é iniciada.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|callEventType|teamworkCallEventType|Representa o tipo de evento de chamada. Os valores possíveis são: `call`, `meeting`, `screenShare`, `unknownFutureValue`.|
|callId|Cadeia de Caracteres|Identificador exclusivo da chamada.|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callStartedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callStartedEventMessageDetail",
  "callId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "callEventType": "String"
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre a chamada iniciada](/graph/system-messages/#call-started)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).