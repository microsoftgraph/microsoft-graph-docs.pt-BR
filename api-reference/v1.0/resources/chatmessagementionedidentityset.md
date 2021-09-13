---
title: Tipo de recurso chatMessageMentionedIdentitySet
description: Representa o recurso @mentioned em uma mensagem em um chat ou em um canal.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9ca4ebbe6b5c508aa6ec2ea0480eae2f66634b76
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109406"
---
# <a name="chatmessagementionedidentityset-resource-type"></a>Tipo de recurso chatMessageMentionedIdentitySet

Namespace: microsoft.graph

Representa o recurso (usuário, aplicativo ou conversa) @mentioned em uma [mensagem](../resources/chatmessage.md) em um chat ou em um canal.


Herda de [identitySet](../resources/identityset.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|aplicativo|[identity](../resources/identity.md)|Herdado [de identitySet](../resources/identityset.md). Se presente, representa um aplicativo (por exemplo, bot) @mentioned em uma [mensagem](../resources/chatmessage.md).|
|conversa|[teamworkConversationIdentity](../resources/teamworkconversationidentity.md)|Se presente, representa uma conversa (por exemplo, equipe ou canal) @mentioned em uma [mensagem](../resources/chatmessage.md).|
|device|[identity](../resources/identity.md)|Herdado [de identitySet](../resources/identityset.md). Não é usado porque não tem suporte para @mention dispositivos.|
|usuário|[identity](../resources/identity.md)|Herdado [de identitySet](../resources/identityset.md). Se presente, representa um usuário @mentioned em uma [mensagem](../resources/chatmessage.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageMentionedIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageMentionedIdentitySet",
  "user": {
    "@odata.type": "microsoft.graph.identity"
  },
  "application": {
    "@odata.type": "microsoft.graph.identity"
  },
  "device": {
    "@odata.type": "microsoft.graph.identity"
  },
  "conversation": {
    "@odata.type": "microsoft.graph.teamworkConversationIdentity"
  }
}
```
