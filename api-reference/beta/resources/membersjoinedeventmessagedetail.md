---
title: Tipo de recurso membersJoinedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre membros ingressado.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b5c95b230e31918ffce5a2a5588aed22e1a7dfd8
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534214"
---
# <a name="membersjoinedeventmessagedetail-resource-type"></a>Tipo de recurso membersJoinedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre membros ingressado.
Essa mensagem é gerada quando os membros ins juntam-se a um chat de reunião.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|membros|[coleção teamworkUserIdentity](../resources/teamworkuseridentity.md)|Lista de membros que ingressaram no chat.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.membersJoinedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.membersJoinedEventMessageDetail",
  "members": [
    {
      "@odata.type": "microsoft.graph.teamworkUserIdentity"
    }
  ],
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre membros ingressado](/graph/system-messages/#members-joined)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).