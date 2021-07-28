---
title: tipo de recurso meetingPolicyUpdatedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma política de reunião atualizada.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2fb18c1275fe6b0d9979978a0d07b4247ddfcdce
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534220"
---
# <a name="meetingpolicyupdatedeventmessagedetail-resource-type"></a>tipo de recurso meetingPolicyUpdatedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre uma política de reunião atualizada.
Essa mensagem é gerada quando a opção de reunião **Permitir bate-papo de reunião** é atualizada.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|meetingChatEnabled|Boolean|Representa se o chat de reunião está habilitado ou não.|
|meetingChatId|Cadeia de Caracteres|Identificador exclusivo do chat de reunião.|

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