---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual em um canal ou entidade de chat. A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread definido pela **propriedade replyToId** na mensagem de chat.
doc_type: resourcePageType
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: e3c109ca11e901fdca2449daf4c98b7c78a558c3
ms.sourcegitcommit: f99dc2b6c8b4cb6f9f74cd780dccc47a2bccfaa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2021
ms.locfileid: "58667469"
---
# <a name="chatmessage-resource-type"></a>Tipo de recurso chatMessage

Namespace: microsoft.graph

Representa uma mensagem de bate-papo individual em um [canal](channel.md) ou [bate-papo](chat.md). A mensagem pode ser uma mensagem raiz ou parte de um thread definido pela propriedade **replyToId** na mensagem.

> **Observação**: este recurso dá suporte à assinatura de alterações (criar, atualizar e excluir) usando [notificações de alteração.](../resources/webhooks.md) Isso permite aos chamadores assinar e obter alterações em tempo real. Para obter detalhes, confira [obter notificações de](/graph/teams-changenotifications-chatMessage)de mensagens.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|**Mensagens de canal**| | |
|[Listar mensagens no canal](../api/channel-list-messages.md) | [chatMessage](chatmessage.md) collection | Lista de todas as mensagens raiz em um canal.|
|[Obter delta de mensagens no canal](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | Obtenha mensagens incrementais em um canal. |
|[Criar assinatura para novas mensagens de canal](../api/subscription-post-subscriptions.md) | [assinatura](subscription.md) | Ouça mensagens novas, editadas e excluídas e reações a elas. |
|[Obter mensagem no canal](../api/chatmessage-get.md) | [chatMessage](chatmessage.md) | Obter uma única mensagem raiz em um canal.|
|[Enviar mensagem no canal](../api/chatmessage-post.md) | [chatMessage](chatmessage.md)| Crie uma nova mensagem raiz em um canal.|
|[Atualizar mensagem no canal](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Atualize a **propriedade policyViolation** de uma mensagem de chat.|
|**Respostas de mensagem de canal**| | |
|[Listar respostas à mensagem](../api/chatmessage-list-replies.md) | [chatMessage](chatmessage.md) collection| Lista de todas as respostas a uma mensagem de chat no canal.|
|[Obter mensagem de resposta no canal](../api/chatmessage-get.md) | [chatMessage](chatmessage.md) | Obter uma única mensagem de resposta em um canal.|
|[Responder a uma mensagem no canal](../api/chatmessage-post-replies.md) | [chatMessage](chatmessage.md)| Responder a uma mensagem de chat existente em um canal.|
|[Atualizar mensagem de resposta](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Atualize a **propriedade policyViolation** de uma mensagem de chat.|
|**Mensagens de chat**| | |
|[Listar mensagens no chat](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Listar mensagens de chat em um chat. |
|[Receba uma mensagem no bate-papo](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | Obter uma única mensagem de chat em um chat. |
|[Criar assinatura para novas mensagens de chat](../api/subscription-post-subscriptions.md) | [assinatura](subscription.md) | Ouça novas, editadas e excluídas mensagens de chat e reações a elas. |
|[Enviar mensagem no chat](../api/chat-post-messages.md) | [chatMessage](chatmessage.md)| Envie uma mensagem de chat em uma conversa 1:1 ou chat em grupo existente.|
|[Atualizar mensagem no chat](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Atualize a **propriedade policyViolation** de uma mensagem de chat.|
|**Conteúdo hospedado**| | |
|[Listar todo o conteúdo hospedado](../api/chatmessage-list-hostedcontents.md) | [coleção chatMessageHostedContent](../resources/chatmessagehostedcontent.md)| Obter todo o conteúdo hospedado associado a uma mensagem.|
|[Obter conteúdo hospedado](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) | Obter conteúdo hospedado (e seus bytes) para uma mensagem.|


## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID única da mensagem.|
|replyToId| cadeia de caracteres | Somente leitura. ID da mensagem de chat pai ou da mensagem de chat raiz do thread. (Aplica-se apenas a mensagens de chat em canais, não chats.) |
|from|[chatMessageFromIdentitySet](chatmessagefromidentityset.md)| Detalhes do remetente da mensagem de chat. Só pode ser definido durante a [migração](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).|
|etag| cadeia de caracteres | Somente leitura. Número da versão da mensagem de chat. |
|messageType|chatMessageType|O tipo de mensagem de chat. Os valores possíveis são: `message`, `chatEvent`, `typing`, `unknownFutureValue`, `systemEventMessage`. Observe que você deve usar o cabeçalho de `Prefer: include-unknown-enum-members` solicitação para obter o seguinte valor nessa [enumeração evolutiva](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `systemEventMessage`.|
|createdDateTime|dateTimeOffset|Timestamp de quando a mensagem de chat foi criada.|
|lastModifiedDateTime|dateTimeOffset|Somente leitura. Timestamp quando a mensagem de chat é criada (configuração inicial) ou modificada, incluindo quando uma reação é adicionada ou removida. |
|lastEditedDateTime|dateTimeOffset|Somente leitura. Timestamp quando as edições para a mensagem de chat foram feitas. Dispara um sinalizador "Editado" na interface Teams interface do usuário. Se nenhuma edição for feita, o valor será `null` .|
|deletedDateTime|dateTimeOffset|Somente leitura. Timestamp no qual a mensagem de chat foi excluída ou nula se não for excluída. |
|assunto|cadeia de caracteres| O assunto da mensagem de chat, em texto sem formatção.|
|body|[itemBody](itembody.md)|Representação plaintext/HTML do conteúdo da mensagem de chat. A representação é especificada pelo contentType dentro do corpo. O conteúdo estará sempre em HTML se a mensagem de chat contiver [um chatMessageMention](chatmessagemention.md). |
|summary|string| Texto de resumo da mensagem de chat que pode ser usada para notificações por push e exibições de resumo ou exibições de retorno. Aplica-se apenas a mensagens de chat de canal, não mensagens de chat em um chat. |
|attachments|[chatMessageAttachment](chatmessageattachment.md) collection |Referências a objetos anexados, como arquivos, guias, reuniões etc.|
|mentions|[chatMessageMention](chatmessagemention.md) collection| Lista de entidades mencionadas na mensagem de chat. As entidades com suporte são: usuário, bot, equipe e canal.|
|importância|string | A importância da mensagem de chat. Os valores possíveis são: `normal`, `high`, `urgent`.|
|reactions| [chatMessageReaction](chatmessagereaction.md) collection | Reações para essa mensagem de chat (por exemplo, Like).|
|localidade|string|Localidade da mensagem de chat definida pelo cliente. Sempre definido para `en-us`.|
|policyViolation | [chatMessagePolicyViolation](chatmessagepolicyviolation.md) |Define as propriedades de uma violação de política definida por um aplicativo de prevenção contra perda de dados (DLP).|
|chatId|cadeia de caracteres|Se a mensagem foi enviada em um chat, representa a identidade do chat.|
|channelIdentity|[channelIdentity](channelidentity.md)|Se a mensagem foi enviada em um canal, representa a identidade do canal.|
|webUrl|cadeia de caracteres|Somente leitura. Link para a mensagem em Microsoft Teams.|

## <a name="relationships"></a>Relações

| Relação   | Tipo    | Descrição |
|:---------------|:--------|:----------|
|respostas|[chatMessage](chatmessage.md)| Respostas para uma mensagem especificada. |
|hostedContents|[chatMessageHostedContent](chatmessagehostedcontent.md)| Conteúdo em uma mensagem hospedada por Microsoft Teams - por exemplo, imagens ou trechos de código. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "replyToId",
    "lastEditedDateTime",
    "deletedDateTime",
    "subject",
    "summary",
    "attachments",
    "mentions",
    "reactions",
    "policyViolation",
    "chatId",
    "channelIdentity"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessage"
}-->


```json
{
  "id": "string (identifier)",
  "replyToId": "string (identifier)",
  "from": {"@odata.type": "microsoft.graph.chatMessageFromIdentitySet"},
  "etag": "string",
  "messageType": "string",
  "createdDateTime": "string (timestamp)",
  "lastModifiedDateTime": "string (timestamp)",
  "lastEditedDateTime": "string (timestamp)",
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
  "chatId": "string",
  "channelIdentity": {"@odata.type": "microsoft.graph.channelIdentity"},
  "webUrl": "string"
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
