---
title: Tipo de recurso membersLeftEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre membros à esquerda.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7fd75e032e58a2254cc9f9965360c2d3a9327759
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322292"
---
# <a name="memberslefteventmessagedetail-resource-type"></a>Tipo de recurso membersLeftEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre [membros à](../resources/conversationMember.md) esquerda.
Essa mensagem é gerada quando **os membros saem** de um chat de [reunião.](../resources/chat.md)


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|members|[coleção teamworkUserIdentity](../resources/teamworkuseridentity.md)|Lista de **membros que** deixaram o **chat**.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.membersLeftEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.membersLeftEventMessageDetail",
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
- [Resposta de exemplo para uma mensagem de evento sobre **membros à** esquerda](/graph/system-messages/#members-left)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
