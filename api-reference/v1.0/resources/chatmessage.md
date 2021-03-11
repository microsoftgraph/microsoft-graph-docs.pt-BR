---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread definido pela **propriedade replyToId** na mensagem de chat.
doc_type: resourcePageType
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 8099efac4132a070bfcf8443ef290989305d6737
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626128"
---
# <a name="chatmessage-resource-type"></a>Tipo de recurso chatMessage

Namespace: microsoft.graph

Representa uma mensagem de chat individual dentro [de um canal](./channel.md) ou chat (em [beta).](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true) A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread de resposta definido pela **propriedade replyToId** na mensagem de chat.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|**Mensagens de canal**| | |
|[ChatMessage de canal de lista](../api/channel-list-messages.md) | [chatMessage](chatmessage.md) collection | Lista de todas as mensagens de chat raiz em um canal.|
|[Obter chatMessages em um delta de canal](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | Obter mensagens de chat incrementais em um canal. |
|[Criar assinatura para novas mensagens de canal](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Ouça mensagens de canal novas e editadas e reações a elas. |
|[Obter chatMessage de canal](../api/channel-get-message.md) | [chatMessage](chatmessage.md) | Obter uma única mensagem de chat raiz de um canal.|
|[Criar chatMessage em um canal](../api/channel-post-message.md) | [chatMessage](../resources/chatmessage.md) | Envie uma mensagem para um canal. |
|[Atualizar chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Atualize a **propriedade policyViolation** de uma mensagem de chat.|
|**Respostas de mensagem de canal**| | |
|[Listar respostas a um chatMessage](../api/channel-list-messagereplies.md) | [chatMessage](chatmessage.md) collection| Lista de todas as respostas a uma mensagem de chat no canal.|
|[Obter uma resposta para um chatMessage](../api/channel-get-messagereply.md) | [chatMessage](chatmessage.md)| Obter uma única resposta a uma mensagem de chat em um canal.|
|[Responder a um chatMessage em um canal](../api/channel-post-messagereply.md) | [chatMessage](chatmessage.md)| Responder a uma mensagem de chat existente em um canal.|
|[Atualizar chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Atualize a **propriedade policyViolation** de uma mensagem de chat.|
|**Conteúdo hospedado**| | |
|[Listar todo o conteúdo hospedado](../api/chatmessage-list-chatmessagehostedcontents.md) | [coleção chatMessageHostedContent](../resources/chatmessagehostedcontent.md)| Obter todo o conteúdo hospedado em uma mensagem de chat.|
|[Obter conteúdo hospedado](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) | Obter conteúdo hospedado de uma mensagem de chat.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID exclusiva da mensagem.|
|replyToId| cadeia de caracteres | Somente leitura. ID da mensagem de chat pai ou da mensagem de chat raiz do thread. (Aplica-se apenas a mensagens de chat em canais e não chats) |
|from|[identitySet](identityset.md)| Somente leitura. Detalhes do remetente da mensagem de chat.|
|etag| cadeia de caracteres | Somente leitura. Número da versão da mensagem de chat. |
|messageType|cadeia de caracteres|O tipo de mensagem de chat. Os valores possíveis são: `message` .|
|createdDateTime|dateTimeOffset|Somente leitura. Timestamp de quando a mensagem de chat foi criada.|
|lastModifiedDateTime|dateTimeOffset|Somente leitura. Timestamp quando a mensagem de chat é criada (configuração inicial) ou editada, incluindo quando uma reação é adicionada ou removida. |
|lastEditedDateTime|dateTimeOffset|Somente leitura. Timestamp quando as edições para a mensagem de chat foram feitas. Dispara um sinalizador "Editado" na interface do usuário do Microsoft Teams. Se nenhuma edição for feita, o valor será `null` .|
|deletedDateTime|dateTimeOffset|Somente leitura. Timestamp no qual a mensagem de chat foi excluída ou nula se não for excluída. |
|assunto|cadeia de caracteres| O assunto da mensagem de chat, em texto sem formatção.|
|corpo|[itemBody](itembody.md)|Representação plaintext/HTML do conteúdo da mensagem de chat. A representação é especificada pelo contentType dentro do corpo. O conteúdo estará sempre em HTML se a mensagem de chat contiver [um chatMessageMention](chatmessagemention.md). |
|summary|cadeia de caracteres| Texto de resumo da mensagem de chat que pode ser usada para notificações por push e exibições de resumo ou exibições de retorno. Aplica-se apenas a mensagens de chat de canal, não mensagens de chat em um chat. |
|attachments|[chatMessageAttachment](chatmessageattachment.md) collection |Arquivos anexos. No momento, os anexos são somente leitura, não há suporte para o envio de anexos. |
|mentions|[chatMessageMention](chatmessagemention.md) collection| Lista de entidades mencionadas na mensagem de chat. Atualmente, dá suporte a usuário, bot, equipe, canal.|
|importância| cadeia de caracteres | A importância da mensagem de chat. Os valores possíveis são: `normal`, `high`, `urgent`.|
| policyViolation | [chatMessagePolicyViolation](../resources/chatmessagepolicyviolation.md) |Define as propriedades de uma violação de política definida por um aplicativo de prevenção contra perda de dados (DLP).|
|localidade|cadeia de caracteres|Localidade da mensagem de chat definida pelo cliente.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "mentions",
    "subject",
    "summary",
    "policyViolation",
    "locale"
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
  "policyViolation": {"@odata.type": "microsoft.graph.chatMessagePolicyViolation"},
  "locale": "string"
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
