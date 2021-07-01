---
title: Tipo de recurso chatMessageInfo
description: Representa uma visualização de um recurso chatMessage.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dc03ee6743aa8115f5a231b3766cc2d6c3d5537b
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236286"
---
# <a name="chatmessageinfo-resource-type"></a>Tipo de recurso chatMessageInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma visualização de um [recurso chatMessage.](../resources/chatmessage.md) Esse objeto só pode ser buscado como parte de uma lista de [chats](../resources/chat.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|corpo|[itemBody](../resources/itembody.md)|Corpo do [chatMessage](../resources/chatmessage.md). Isso ainda conterá marcadores para @mentions e anexos, mesmo que o objeto não retorne @mentions e anexos.|
|createdDateTime|DateTimeOffset|Objeto date time representando a hora em que a mensagem foi criada.|
|from|[chatMessageFromIdentitySet](../resources/chatmessagefromidentityset.md)|Informações sobre o remetente da mensagem.|
|id|String|ID do [chatMessage](../resources/chatmessage.md).|
|isDeleted|Booleano|Se definido como `true` , a mensagem original foi excluída.|

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
  "isDeleted": "Boolean"
}
```

## <a name="see-also"></a>Confira também

- [chat](../resources/chat.md)
- [chatMessage](../resources/chatmessage.md)

