---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual em um canal ou em uma entidade de chat. A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread que é definido pela propriedade **replyToId** na mensagem de chat.
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: f1af347d0c043ec2b0ca2da05ba44331aab925d2
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193460"
---
# <a name="chatmessage-resource-type"></a>Tipo de recurso chatMessage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Representa uma mensagem de bate-papo individual em um [canal](channel.md) ou [bate-papo](chat.md). A mensagem pode ser uma mensagem raiz ou parte de um thread definido pela propriedade **replyToId** na mensagem.


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|**Mensagens de canal**| | |
|[Listar canal chat](../api/channel-list-messages.md) | [chatMessage](chatmessage.md) collection | Lista de todas as mensagens de chat raiz em um canal.|
|[Obter chatMessages em um Delta de canal](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | Obter mensagens de chat incrementais em um canal. |
|[Criar assinatura para novas mensagens de canal](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Ouvir mensagens de canal novas e editadas e reações para elas. |
|[Obter canal chat](../api/channel-get-message.md) | [chatMessage](chatmessage.md) | Obtenha uma única mensagem de chat raiz de um canal.|
|[Criar chat em um canal ou chat](../api/chatmessage-post.md) | [chatMessage](chatmessage.md)| Criar uma nova mensagem de chat de nível superior em um canal.|
|[Atualizar chat](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Atualizar a propriedade **policyViolation** de uma mensagem de chat.|
|**Respostas de mensagens de canal**| | |
|[Listar respostas a um chat](../api/channel-list-messagereplies.md) | [chatMessage](chatmessage.md) collection| Lista de todas as respostas para uma mensagem de chat no canal.|
|[Obter uma resposta para um chat](../api/channel-get-messagereply.md) | [chatMessage](chatmessage.md)| Obter uma única resposta para uma mensagem de chat em um canal.|
|[Responder a um chat em um canal](../api/channel-post-messagereply.md) | [chatMessage](chatmessage.md)| Responder a uma mensagem de chat existente em um canal.|
|[Atualizar chat](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Atualizar a propriedade **policyViolation** de uma mensagem de chat.|
|**1:1 e mensagens de chat de grupo**| | |
|[Obter chat no chat](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | Obter uma única mensagem de chat em um chat. |
|[Listar chatMessages em um chat](../api/chat-list-message.md)  | [chatMessage](../resources/chatmessage.md) | Listar mensagens de chat em um bate-papo de grupo ou 1:1. |
|[Criar assinatura para novas mensagens de chat](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Ouvir mensagens de chat novas e editadas e reações para elas. |
|[Criar chat em um chat](../api/chat-post-message.md) | [chatMessage](chatmessage.md)| Envie uma mensagem de chat em uma conversa existente de chat de grupo ou 1:1.|
|[Atualizar chat](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Atualizar a propriedade **policyViolation** de uma mensagem de chat.|
|**Conteúdo hospedado**| | |
|[Listar todo o conteúdo hospedado](../api/chatmessage-list-chatmessagehostedcontents.md) | coleção [chatMessageHostedContent](../resources/chatmessagehostedcontent.md)| Obter todo o conteúdo hospedado em uma mensagem de chat.|
|[Obter conteúdo hospedado](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) | Obter conteúdo hospedado de uma mensagem de chat.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID única da mensagem.|
|replyToId| string | Somente leitura. ID da mensagem de chat pai ou mensagem de chat raiz do thread. (Só se aplica a mensagens de chat em canais, não chats.) |
|from|[identitySet](identityset.md)| Somente leitura. Detalhes do remetente da mensagem de chat.|
|etag| string | Somente leitura. Número de versão da mensagem de chat. |
|messageType|string|O tipo de mensagem de chat. Os valores possíveis são: `message` .|
|createdDateTime|dateTimeOffset|Somente leitura. Carimbo de data/hora de quando a mensagem de chat foi criada.|
|lastModifiedDateTime|dateTimeOffset|Somente leitura. Carimbo de data/hora em que a mensagem de chat é criada (configuração inicial) ou modificada, incluindo quando uma reação é adicionada ou removida. |
|lastEditedDateTime|dateTimeOffset|Somente leitura. Carimbo de data/hora em que foram feitas edições na mensagem de chat. Dispara um sinalizador "editado" na interface do usuário do Microsoft Teams. Se não for feita nenhuma edição, o valor será `null` .|
|deletedDateTime|dateTimeOffset|Somente leitura. Carimbo de data/hora em que a mensagem de chat foi excluída ou nula se não for excluída. |
|assunto|string| O assunto da mensagem de chat, em texto não criptografado.|
|body|[itemBody](itembody.md)|Representação de texto não criptografado/HTML do conteúdo da mensagem de chat. A representação é especificada pelo contentType dentro do corpo. O conteúdo estará sempre em HTML se a mensagem de chat contiver um [chatMessageMention](chatmessagemention.md). |
|summary|string| Texto de resumo da mensagem de chat que pode ser usado para notificações por push e visualizações de resumo ou exibições de retorno. Aplica-se somente a mensagens de chat de canal, e não a mensagens de chat em um chat. |
|attachments|[chatMessageAttachment](chatmessageattachment.md) collection |Arquivos anexos. No momento, os anexos são somente leitura, não há suporte para o envio de anexos. |
|mentions|[chatMessageMention](chatmessagemention.md) collection| Lista de entidades mencionadas na mensagem de chat. Atualmente, dá suporte a usuário, bot, equipe, canal.|
|importância|string | A importância da mensagem de chat. Os valores possíveis são: `normal`, `high`, `urgent`.|
|reactions| [chatMessageReaction](./chatmessagereaction.md) collection | Reações para esta mensagem de chat (por exemplo, como).|
|localidade|string|Local da mensagem de chat definida pelo cliente.|
| policyViolation | [chatMessagePolicyViolation](../resources/chatmessagepolicyviolation.md) |Define as propriedades de uma violação de política definida por um aplicativo DLP (prevenção de perda de dados).|

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

