---
title: tipo de recurso conversationMemberRoleUpdatedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma função atualizada de um membro da conversa em um canal ou em uma equipe.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2c91e2a476b048c6d451c31c96ac95a3756bbbe4
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322332"
---
# <a name="conversationmemberroleupdatedeventmessagedetail-resource-type"></a>tipo de recurso conversationMemberRoleUpdatedEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre uma função atualizada de um membro [da](../resources/conversationMember.md) conversa em um [canal](../resources/channel.md) ou em uma [equipe.](../resources/team.md)
Essa mensagem é gerada quando a função de **um membro** em um **canal** ou uma **equipe é** atualizada.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|conversationMemberRoles|Coleção String|Funções para o **usuário membro de coversation.**|
|conversationMemberUser|[teamworkUserIdentity](../resources/teamworkuseridentity.md)|Identidade do usuário **membro da** conversa.|
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
- [Resposta de exemplo para uma mensagem de evento sobre uma função atualizada de um membro **da** conversa em um **canal** ou em uma **equipe**](/graph/system-messages/#conversation-member-role-updated)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
