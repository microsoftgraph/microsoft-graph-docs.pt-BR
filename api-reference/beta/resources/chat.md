---
title: tipo de recurso chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1091021235a50d3dfa237467e319da9b131b7a72
ms.sourcegitcommit: 4bdcb5cd3227ff009e10868f2936b3153372b87a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/25/2019
ms.locfileid: "33301843"
---
# <a name="chat-resource-type"></a>tipo de recurso chat

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes. Os participantes podem ser usuários ou aplicativos.

## <a name="methods"></a>Métodos

|  Método       |  Tipo de retorno  | Descrição| 
|:---------------|:--------|:----------|
|[Listar chats](../api/chat-list.md) | coleção [chat](channel.md) | Obter a lista de chats de que um usuário faz parte.|
|[Obter chat](../api/chat-get.md) | [chat](channel.md) | Leia as propriedades e as relações do chat.|
|[Listar mensagens em um chat](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Obter mensagens em um bate-papo de grupo ou 1:1. |
|[Obter mensagem no chat](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | Obter uma única mensagem em um chat. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| id| Cadeia de caracteres| O identificador exclusivo do chat. Somente leitura.|
| topic| String|  Opcion Assunto ou tópico do chat. Disponível apenas para bate-papos de grupo.|
| createdDateTime| dateTimeOffset|  Data e hora em que o chat foi criado. Somente leitura.|
| lastUpdatedDateTime| dateTimeOffset|  Data e hora em que o chat foi atualizado. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| messages | [chatMessage](chatmessage.md) collection | Uma coleção de todas as mensagens no chat. Anulável. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chat"
}-->

```json
{
  "id": "string (identifier)",
  "topic": "string",
  "createdDateTime": "dateTimeOffset",
  "lastUpdatedDateTime": "dateTimeOffset"
}

```

## <a name="see-also"></a>Confira também

- [channel](channel.md)
- [chatMessage](chatmessage.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
