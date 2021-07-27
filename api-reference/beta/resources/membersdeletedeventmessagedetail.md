---
title: Tipo de recurso membersDeletedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre membros excluídos.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dd19922ec5c238d407cae6879efb389a52a58b62
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534216"
---
# <a name="membersdeletedeventmessagedetail-resource-type"></a>Tipo de recurso membersDeletedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre membros excluídos.
Essa mensagem é gerada quando membros são removidos de um chat, um canal ou uma equipe.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|membros|[coleção teamworkUserIdentity](../resources/teamworkuseridentity.md)|Lista de membros excluídos.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.membersDeletedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.membersDeletedEventMessageDetail",
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
- [Resposta de exemplo para uma mensagem de evento sobre membros excluídos](/graph/system-messages/#members-deleted)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).