---
title: Tipo de recurso membersJoinedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre membros ingressado.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: bbcbabbdec89c44aa88adbae36191472fee31053
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322298"
---
# <a name="membersjoinedeventmessagedetail-resource-type"></a>Tipo de recurso membersJoinedEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre [membros ingressado.](../resources/conversationMember.md)
Essa mensagem é gerada quando **os membros ins** juntam-se a um chat de [reunião.](../resources/chat.md)


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|members|[coleção teamworkUserIdentity](../resources/teamworkuseridentity.md)|Lista de **membros que** ingressaram no **chat**.|

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
- [Resposta de exemplo para uma mensagem de evento sobre **membros ingressado**](/graph/system-messages/#members-joined)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
