---
title: tipo de recurso chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 43ed088889a4b81d59cb9e1361ed978c9cb61141
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864200"
---
# <a name="chat-resource-type"></a>tipo de recurso chat

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes. Os participantes podem ser usuários ou aplicativos.

## <a name="methods"></a>Methods

|  Método       |  Tipo de retorno  | Descrição| Permissões |
|:---------------|:--------|:----------|-----------|
|[Listar chats](../api/chat-list.md) | coleção [chat](channel.md) | Obter a lista de chats de que um usuário faz parte.| **Somente delegada** |
|[Obter bate-papo](../api/chat-get.md) | [chat](channel.md) | Leia as propriedades e as relações do chat.| **Somente delegada** |
|[Listar membros de chat](../api/conversationmember-list.md) | coleção [conversationmember](conversationmember.md) | Ver a lista de todos os usuários no bate-papo.| Delegado e aplicativo * |
|[Obter membro de chat](../api/conversationmember-get.md) | [conversationmember](conversationmember.md) | Obter um único usuário no bate-papo.| Delegado e aplicativo * |
|[Listar mensagens em um bate-papo](../api/chatmessage-list.md)  | [chatMessage](../resources/chatmessage.md) | Receba mensagens em um bate-papo de um para um ou de grupo. | Delegado e aplicativo * |
|[Receba uma mensagem no bate-papo](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | Receba uma única mensagem em um bate-papo. | Delegado e aplicativo * |

\*> **Observação:** Ao usar permissões de aplicativo, certifique-se de saber como você vai obter a ID de chat. Como a lista de chats com permissões de aplicativo não é suportada, nem todos os cenários são possíveis. É possível obter IDs de chat com permissões delegadas e de notificações de [alteração para o/chats/allMessages](../api/subscription-post-subscriptions.md) com permissões de aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
| id| String| O identificador exclusivo do chat. Somente leitura.|
| topic| String|  Opcion Assunto ou tópico do chat. Disponível apenas para bate-papos de grupo.|
| createdDateTime| dateTimeOffset|  Data e hora em que o chat foi criado. Somente leitura.|
| lastUpdatedDateTime| dateTimeOffset|  Data e hora em que o chat foi atualizado. Somente leitura.|

## <a name="relationships"></a>Relacionamento

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
| installedApps | Coleção [teamsAppInstallation](teamsappinstallation.md) | Uma coleção de todos os aplicativos no chat. Anulável. |
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
