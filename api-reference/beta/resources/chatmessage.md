---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual em uma entidade de canal ou chat. A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread definido pela propriedade **replyToId** na mensagem de chat.
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 53c4a22d66ced56a038e89a504f918a184c33a02
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874044"
---
# <a name="chatmessage-resource-type"></a>Tipo de recurso chatMessage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma mensagem de bate-papo individual em um [canal](channel.md) ou [bate-papo](chat.md). A mensagem pode ser uma mensagem raiz ou parte de um thread definido pela propriedade **replyToId** na mensagem.

> **Observação:** esse recurso dá suporte à assinatura de alterações (criar, atualizar e excluir) usando [notificações de alteração.](../resources/webhooks.md) Isso permite aos chamadores assinar e obter alterações em tempo real. Para obter detalhes, confira [obter notificações de](/graph/teams-changenotifications-chatMessage)de mensagens.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|**Mensagens de canal**| | |
|[Listar chatMessage de canal](../api/channel-list-messages.md) | [chatMessage](chatmessage.md) collection | Lista de todas as mensagens de chat raiz em um canal.|
|[Obter chatMessages em um delta de canal](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | Obter mensagens de chat incremental em um canal. |
|[Criar assinatura para novas mensagens de canal](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Ouça mensagens de canal novas e editadas e reações a elas. |
|[Obter chatMessage de canal](../api/channel-get-message.md) | [chatMessage](chatmessage.md) | Obter uma única mensagem de chat raiz de um canal.|
|[Criar chatMessage em um canal ou chat](../api/chatmessage-post.md) | [chatMessage](chatmessage.md)| Crie uma nova mensagem de chat de nível superior em um canal.|
|[Atualizar chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Atualize **a propriedade policyViolation** de uma mensagem de chat.|
|**Respostas de mensagem de canal**| | |
|[Listar respostas a um chatMessage](../api/channel-list-messagereplies.md) | [chatMessage](chatmessage.md) collection| Lista de todas as respostas a uma mensagem de chat no canal.|
|[Obter uma resposta a um chatMessage](../api/channel-get-messagereply.md) | [chatMessage](chatmessage.md)| Obter uma única resposta para uma mensagem de chat em um canal.|
|[Responder a um chatMessage em um canal](../api/channel-post-messagereply.md) | [chatMessage](chatmessage.md)| Responder a uma mensagem de chat existente em um canal.|
|[Atualizar chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Atualize **a propriedade policyViolation** de uma mensagem de chat.|
|**Mensagens de bate-papo de grupo e 1:1**| | |
|[Obter chatMessage no chat](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | Obter uma única mensagem de chat em um chat. |
|[Listar chatMessages em um chat](../api/chat-list-message.md)  | [chatMessage](../resources/chatmessage.md) | Listar mensagens de chat em um chat de grupo ou 1:1. |
|[Obter todas as mensagens de chat para o usuário](../api/chats-getallmessages.md)| [coleção de chat](chat.md)| Obter mensagens de todos os chats dos quais um usuário é participante, incluindo chats 1:1, chats em grupo e chats de reunião. |
|[Criar assinatura para novas mensagens de chat](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Ouça mensagens de chat novas e editadas e reações a elas. |
|[Criar chatMessage em um chat](../api/chat-post-message.md) | [chatMessage](chatmessage.md)| Envie uma mensagem de chat em uma conversa de chat em grupo ou 1:1 existente.|
|[Atualizar chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Atualize **a propriedade policyViolation** de uma mensagem de chat.|
|**Conteúdo hospedado**| | |
|[Listar todo o conteúdo hospedado](../api/chatmessage-list-chatmessagehostedcontents.md) | [Coleção chatMessageHostedContent](../resources/chatmessagehostedcontent.md)| Obter todo o conteúdo hospedado em uma mensagem de chat.|
|[Obter conteúdo hospedado](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) | Obter conteúdo hospedado de uma mensagem de chat.|


## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID única da mensagem.|
|replyToId| string | Somente leitura. ID da mensagem de chat pai ou da mensagem de chat raiz do thread. (Aplica-se somente a mensagens de chat em canais, não chats.) |
|from|[identitySet](identityset.md)| Somente leitura. Detalhes do remetente da mensagem de chat.|
|etag| string | Somente leitura. Número da versão da mensagem de chat. |
|messageType|string|O tipo de mensagem de chat. Os valores possíveis são: `message` .|
|createdDateTime|dateTimeOffset|Somente leitura. O timestamp de quando a mensagem de chat foi criada.|
|lastModifiedDateTime|dateTimeOffset|Somente leitura. O timestamp quando a mensagem de chat é criada (configuração inicial) ou modificada, incluindo quando uma reação é adicionada ou removida. |
|lastEditedDateTime|dateTimeOffset|Somente leitura. O timestamp quando as edições da mensagem de chat foram feitas. Aciona um sinalizador "Editado" na interface do usuário do Teams. Se nenhuma edição for feita, o valor será `null` .|
|deletedDateTime|dateTimeOffset|Somente leitura. O timestamp no qual a mensagem de chat foi excluída ou nulo se não foi excluído. |
|assunto|string| O assunto da mensagem de chat, em texto não criptografado.|
|body|[itemBody](itembody.md)|Representação de texto sem formatação/HTML do conteúdo da mensagem de chat. A representação é especificada pelo contentType dentro do corpo. O conteúdo estará sempre em HTML se a mensagem de chat contiver [um chatMessageMention](chatmessagemention.md). |
|summary|string| Texto de resumo da mensagem de chat que poderia ser usado para notificações por push e exibições de resumo ou exibições de fall back. Aplica-se somente a mensagens de chat de canal, não mensagens de chat em um chat. |
|attachments|[chatMessageAttachment](chatmessageattachment.md) collection |Arquivos anexos. No momento, os anexos são somente leitura, não há suporte para o envio de anexos. |
|mentions|[chatMessageMention](chatmessagemention.md) collection| Lista de entidades mencionada na mensagem de chat. Atualmente, dá suporte a usuário, bot, equipe, canal.|
|importância|string | A importância da mensagem de chat. Os valores possíveis são: `normal`, `high`, `urgent`.|
|reactions| [chatMessageReaction](./chatmessagereaction.md) collection | Reações para essa mensagem de chat (por exemplo, Like).|
|localidade|string|Localidade da mensagem de chat definida pelo cliente.|
| policyViolation | [chatMessagePolicyViolation](../resources/chatmessagepolicyviolation.md) |Define as propriedades de uma violação de política definida por um aplicativo de prevenção de perda de dados (DLP).|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "reactions",
    "mentions",
    "subject",
    "summary"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessage"
}-->


```json
{
  "id": "string (identifier)",
  "replyToId": "string (identifier)",
  "from": {"@odata.type": "microsoft.graph.identitySet"},
  "etag": "string",
  "messageType": "string",
  "createdDateTime": "string (timestamp)",
  "lastModifiedDateTime": "string (timestamp)",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string",
  "policyViolation": {"@odata.type": "microsoft.graph.chatMessagePolicyViolation"},
  "deleted": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
