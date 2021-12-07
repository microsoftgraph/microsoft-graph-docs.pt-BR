---
title: Tipo de recurso callStartedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre a chamada iniciada.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2e567a4dae25ff671b86c78a03243c93ddcf9e90
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322286"
---
# <a name="callstartedeventmessagedetail-resource-type"></a>Tipo de recurso callStartedEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre a chamada iniciada.
Essa mensagem é gerada quando uma chamada é iniciada.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|callEventType|teamworkCallEventType|Representa o tipo de evento de chamada. Os valores possíveis são: `call`, `meeting`, `screenShare`, `unknownFutureValue`.|
|callId|String|Identificador exclusivo da chamada.|
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
