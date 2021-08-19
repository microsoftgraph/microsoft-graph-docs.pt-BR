---
title: Tipo de recurso chatMessageInfo
description: Representa uma visualização de um recurso chatMessage.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 289bce30b970edd46f0ad29fdbaa24fd6428c93d
ms.sourcegitcommit: 6f04ad0e0cde696661511dcdf343942b43f73fc6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2021
ms.locfileid: "58397037"
---
# <a name="chatmessageinfo-resource-type"></a>Tipo de recurso chatMessageInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma visualização de um [recurso chatMessage.](../resources/chatmessage.md) Esse objeto só pode ser buscado como parte de uma lista de [chats](../resources/chat.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|body|[itemBody](../resources/itembody.md)|Corpo do [chatMessage](../resources/chatmessage.md). Isso ainda conterá marcadores para @mentions e anexos, mesmo que o objeto não retorne @mentions e anexos.|
|createdDateTime|DateTimeOffset|Objeto date time representando a hora em que a mensagem foi criada.|
|from|[chatMessageFromIdentitySet](../resources/chatmessagefromidentityset.md)|Informações sobre o remetente da mensagem.|
|id|Cadeia de caracteres|ID do [chatMessage](../resources/chatmessage.md).|
|isDeleted|Booliano|Se definido como `true` , a mensagem original foi excluída.|
|messageType|chatMessageType|O tipo de mensagem de chat. Os valores possíveis são: `message`, `unknownFutureValue`, `systemEventMessage`.|
|eventDetail|[eventMessageDetail](../resources/eventmessagedetail.md)|Somente leitura.  Se presente, representa detalhes de um evento que aconteceu em um chat, um canal ou uma equipe, por exemplo, membros foram adicionados e assim por diante. Para mensagens de evento, a **propriedade messageType** será definida como `systemEventMessage` .|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageInfo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageInfo",
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "from": {
    "@odata.type": "microsoft.graph.chatMessageFromIdentitySet"
  },
  "createdDateTime": "String (timestamp)",
  "isDeleted": "Boolean",
  "messageType": "String",
  "eventDetail": {
    "@odata.type": "microsoft.graph.eventMessageDetail"
  }
}
```

## <a name="see-also"></a>Confira também

- [chat](../resources/chat.md)
- [chatMessage](../resources/chatmessage.md)

