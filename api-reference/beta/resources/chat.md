---
title: tipo de recurso chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4d0f1009079c4994814385ae8758af6c211f17a2
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2019
ms.locfileid: "34344973"
---
# <a name="chat-resource-type"></a>tipo de recurso chat

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes. Os participantes podem ser usuários ou aplicativos.

## <a name="methods"></a>Métodos

|  Método       |  Tipo de retorno  | Descrição| 
|:---------------|:--------|:----------|
|[Listar chats](../api/chat-list.md) | coleção [chat](channel.md) | Obter a lista de chats de que um usuário faz parte.|
|[Obter bate-papo](../api/chat-get.md) | [chat](channel.md) | Leia as propriedades e as relações do chat.|
|[Listar membros de chat](../api/conversationmember-list.md) | coleção [conversationmember](conversationmember.md) | Obtenha a lista de todos os usuários no chat.|
|[Obter membro de chat](../api/conversationmember-get.md) | [conversationmember](conversationmember.md) | Obtenha um único usuário no chat.|
|[Listar mensagens em um bate-papo](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Receba mensagens em um bate-papo de um para um ou de grupo. |
|[Receba uma mensagem no bate-papo](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | Receba uma única mensagem em um bate-papo. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| id| String| O identificador exclusivo do chat. Somente leitura.|
| topic| String|  Opcion Assunto ou tópico do chat. Disponível apenas para bate-papos de grupo.|
| createdDateTime| dateTimeOffset|  Data e hora em que o chat foi criado. Somente leitura.|
| lastUpdatedDateTime| dateTimeOffset|  Data e hora em que o chat foi atualizado. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| membros | coleção [conversationMember](conversationmember.md) | Uma coleção de todas as pessoas no chat. Anulável. |
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
