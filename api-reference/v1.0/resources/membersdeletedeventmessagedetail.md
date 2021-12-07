---
title: Tipo de recurso membersDeletedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre membros excluídos.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0f33dfa80fc27f7eb48e00dbaa6c427f7bb30a45
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322331"
---
# <a name="membersdeletedeventmessagedetail-resource-type"></a>Tipo de recurso membersDeletedEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre [membros](../resources/conversationMember.md) excluídos.
Essa mensagem é gerada quando **os membros** são removidos de um [chat,](../resources/chat.md)um [canal](../resources/channel.md)ou uma [equipe.](../resources/team.md)


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|
|members|[coleção teamworkUserIdentity](../resources/teamworkuseridentity.md)|Lista de **membros** excluídos.|

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
- [Resposta de exemplo para uma mensagem de evento sobre **membros** excluídos](/graph/system-messages/#members-deleted)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
