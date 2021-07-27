---
title: Tipo de recurso membersLeftEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre membros à esquerda.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 744cce3f20fcadc9afca9e863dd037b1dfe38b65
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534213"
---
# <a name="memberslefteventmessagedetail-resource-type"></a>Tipo de recurso membersLeftEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre membros à esquerda.
Essa mensagem é gerada quando os membros saem de um chat de reunião.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|membros|[coleção teamworkUserIdentity](../resources/teamworkuseridentity.md)|Lista de membros que deixaram o chat.|

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
- [Resposta de exemplo para uma mensagem de evento sobre membros à esquerda](/graph/system-messages/#members-left)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).