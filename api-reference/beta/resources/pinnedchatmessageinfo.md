---
title: Tipo de recurso pinnedChatMessageInfo
description: Representa uma mensagem fixa individual em uma entidade de chat.
author: sumanac
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d9ee744cfe71a2c9a8c05b0a8ed86c046827428d
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653589"
---
# <a name="pinnedchatmessageinfo-resource-type"></a>Tipo de recurso pinnedChatMessageInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma mensagem fixa individual em um [chat](chat.md).


Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mensagens fixadas no chat](../api/chat-list-pinnedmessages.md)|[Coleção pinnedChatMessageInfo](../resources/pinnedchatmessageinfo.md)|Obtenha uma lista de mensagens fixadas em um chat.|
|[Fixar uma mensagem no chat](../api/chat-post-pinnedmessages.md)|[pinnedChatMessageInfo](../resources/pinnedchatmessageinfo.md)|Fixe uma mensagem de chat em um chat.|
|[Desafixar uma mensagem do chat](../api/chat-delete-pinnedmessages.md)|Nenhum|Desafixar uma mensagem de um chat.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| id| Cadeia de caracteres| A ID do [chatMessage](../resources/chatmessage.md). Somente leitura. |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
| mensagem | [chatMessage](../resources/chatmessage.md) | Representa detalhes sobre a mensagem de chat fixada.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.pinnedChatMessageInfo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.pinnedChatMessageInfo",
  "id": "String (identifier)"
}
```

