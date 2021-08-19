---
title: Tipo de recurso membersAddedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre membros adicionados.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 33d0c73ff5726310c1a4566813bd034cd9d5e9cc
ms.sourcegitcommit: 6f04ad0e0cde696661511dcdf343942b43f73fc6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396988"
---
# <a name="membersaddedeventmessagedetail-resource-type"></a>Tipo de recurso membersAddedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre membros adicionados.
Essa mensagem é gerada quando os membros são adicionados a um chat, um canal ou uma equipe.
A **propriedade visibleHistoryStartDateTime** para um evento adicionado de membros em um canal é sempre definida como , o que indica que todo o `0001-01-01T00:00:00Z` histórico é compartilhado.

> **Observação**: para um chat, quando o tempo de histórico de compartilhamento selecionado para membros for anterior ao tempo de histórico visível do initator, a propriedade **visibleHistoryStartDateTime** para [conversationMember](conversationmember.md) e a mensagem **membersAddedEventMessageDetail** podem ter valores diferentes. [conversationMember](conversationmember.md) tem o tempo de histórico visível efetivo para o membro com base no tempo de histórico visível do iniciador.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|membros|[coleção teamworkUserIdentity](../resources/teamworkuseridentity.md)|Lista de membros adicionados.|
|visibleHistoryStartDateTime|DateTimeOffset|O timestamp que denota o quanto o histórico de uma conversa é compartilhado com os membros da conversa.|

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
- [Resposta de exemplo para uma mensagem de evento sobre membros adicionados](/graph/system-messages/#members-added)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
