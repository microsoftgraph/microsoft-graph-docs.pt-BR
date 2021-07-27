---
title: Tipo de recurso membersAddedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre membros adicionados.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 43a9d93166968f92cde12f37b76b8da9062ee4c3
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534218"
---
# <a name="membersaddedeventmessagedetail-resource-type"></a>Tipo de recurso membersAddedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre membros adicionados.
Essa mensagem é gerada quando os membros são adicionados a um chat, um canal ou uma equipe.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|membros|[coleção teamworkUserIdentity](../resources/teamworkuseridentity.md)|Lista de membros adicionados.|

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
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre membros adicionados](/graph/system-messages/#members-added)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).