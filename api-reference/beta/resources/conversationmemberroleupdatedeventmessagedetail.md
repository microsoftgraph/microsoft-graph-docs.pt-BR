---
title: tipo de recurso conversationMemberRoleUpdatedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma função atualizada de um membro da conversa em um canal ou em uma equipe.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2ab15ff8f874ffeaa4424f29b8cc452ae128ae2c
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534230"
---
# <a name="conversationmemberroleupdatedeventmessagedetail-resource-type"></a>tipo de recurso conversationMemberRoleUpdatedEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre uma função atualizada de um membro da conversa em um canal ou em uma equipe.
Essa mensagem é gerada quando a função de um membro em um canal ou uma equipe é atualizada.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|conversationMemberRoles|Coleção de cadeias de caracteres|Funções para o usuário membro de coversation.|
|conversationMemberUser|[teamworkUserIdentity](../resources/teamworkuseridentity.md)|Identidade do usuário membro da conversa.|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conversationMemberRoleUpdatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conversationMemberRoleUpdatedEventMessageDetail",
  "conversationMemberRoles": [
    "String"
  ],
  "converstaionMemberUser": {
    "@odata.type": "microsoft.graph.teamworkUserIdentity"
  },
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre uma função atualizada de um membro da conversa em um canal ou em uma equipe](/graph/system-messages/#conversation-member-role-updated)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).