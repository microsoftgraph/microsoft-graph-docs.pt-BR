---
title: Tipo de recurso chatMessageMentionedIdentitySet
description: Representa o recurso @mentioned em uma mensagem em um chat ou em um canal.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9bbd65344616a979916a1b2bf32528bc8cd00814
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211196"
---
# <a name="chatmessagementionedidentityset-resource-type"></a>Tipo de recurso chatMessageMentionedIdentitySet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o recurso (usuário, aplicativo ou conversa) @mentioned em uma [mensagem](../resources/chatmessage.md) em um chat ou em um canal.


Herda de [identitySet](../resources/identityset.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|aplicativo|[identity](../resources/identity.md)|Herdado [de identitySet](../resources/identityset.md). Se presente, representa um aplicativo (por exemplo, bot) @mentioned em uma [mensagem](../resources/chatmessage.md).|
|conversa|[teamworkConversationIdentity](../resources/teamworkconversationidentity.md)|Se presente, representa uma conversa (por exemplo, equipe ou canal) @mentioned em uma [mensagem](../resources/chatmessage.md).|
|device|[identity](../resources/identity.md)|Herdado [de identitySet](../resources/identityset.md). Não é usado porque não tem suporte para @mention dispositivos.|
|user|[identity](../resources/identity.md)|Herdado [de identitySet](../resources/identityset.md). Se presente, representa um usuário @mentioned em uma [mensagem](../resources/chatmessage.md).|
|tag|[teamworkTagIdentity](../resources/teamworktagidentity.md)|Se presente, representa uma marca @mentioned em uma mensagem de [equipe](../resources/chatmessage.md).|

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
  },
  "tag": {
    "@odata.type": "microsoft.graph.teamworkTagIdentity"
  }
}
```