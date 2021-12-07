---
title: tipo de recurso meetingPolicyUpdatedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma política de reunião atualizada.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 256f50d33957ca76bdeedda604698c80739b431b
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322289"
---
# <a name="meetingpolicyupdatedeventmessagedetail-resource-type"></a>tipo de recurso meetingPolicyUpdatedEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre uma política de reunião atualizada.
Essa mensagem é gerada quando a opção de reunião **Permitir bate-papo de reunião** é atualizada.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|meetingChatEnabled|Booliano|Representa se o [chat de reunião](../resources/chat.md) está habilitado ou não.|
|meetingChatId|String|Identificador exclusivo do chat de **reunião.**|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingPolicyUpdatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.meetingPolicyUpdatedEventMessageDetail",
  "meetingChatId": "String",
  "meetingChatEnabled": "Boolean",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre uma política de reunião atualizada](/graph/system-messages/#meeting-policy-updated)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
