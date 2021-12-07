---
title: Tipo de recurso membersAddedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre membros adicionados.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: df1bb119f115d047fb8d5ff6a426ae259d8fe55d
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322325"
---
# <a name="membersaddedeventmessagedetail-resource-type"></a>Tipo de recurso membersAddedEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre [membros adicionados.](../resources/conversationMember.md)
Essa mensagem é gerada quando **os membros** são adicionados a [um chat,](../resources/chat.md)um [canal](../resources/channel.md)ou uma [equipe.](../resources/team.md)
A **propriedade visibleHistoryStartDateTime** para  um evento sobre membros adicionados **a** um canal é sempre definida como , o que indica que todo o histórico é `0001-01-01T00:00:00Z` compartilhado.

> **Observação**: a propriedade **visibleHistoryStartDateTime** para um [conversationMember](conversationmember.md) e a mensagem **membersAddedEventMessageDetail** podem  ter valores diferentes se o valor **selecionado shareHistoryTime** para membros em um **chat** for anterior ao tempo de histórico visível do iniciador.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|members|[coleção teamworkUserIdentity](../resources/teamworkuseridentity.md)|Lista de **membros** adicionados.|
|visibleHistoryStartDateTime|DateTimeOffset|O timestamp que indica o quanto o histórico de uma conversa é compartilhado com os membros da conversa.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.membersAddedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.membersAddedEventMessageDetail",
  "members": [
    {
      "@odata.type": "microsoft.graph.teamworkUserIdentity"
    }
  ],
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "visibleHistoryStartDateTime": "String (timestamp)"
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre **membros adicionados**](/graph/system-messages/#members-added)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
