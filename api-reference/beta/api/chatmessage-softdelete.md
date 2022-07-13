---
title: 'chatMessage: softDelete'
description: Exclua uma única mensagem ou resposta de mensagem em um canal ou chat.
author: Ramjot Singh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.localizationpriority: medium
ms.openlocfilehash: df9262e051c59760d3890e772dbc3857afc6182b
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768337"
---
# <a name="chatmessage-softdelete"></a>chatMessage: softDelete

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exclua [uma única mensagem](../resources/chatmessage.md) [ou uma resposta de mensagem](../resources/chatmessage.md) em [um canal ou](../resources/channel.md) [chat](../resources/chat.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

### <a name="permissions-for-channel"></a>Permissões para o canal

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
|Delegada (conta corporativa ou de estudante)| ChannelMessage.ReadWrite |
|Delegada (conta pessoal da Microsoft)| Sem suporte. |
|Aplicativo| Sem suporte. |

### <a name="permissions-for-chat"></a>Permissões para o chat

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
|Delegada (conta corporativa ou de estudante)| ChatMessage.ReadWrite |
|Delegada (conta pessoal da Microsoft)| Sem suporte. |
|Aplicativo| Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{userId}/chats/{chatsId}/messages/{chatMessageId}/softDelete
POST /teams/{teamsId}/channels/{channelId}/messages/{chatMessageId}/softDelete
POST /teams/{teamId}/channels/{channelId}/messages/{messageId}/replies/{replyId}/softDelete
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="example-1-soft-delete-message-in-a-chat"></a>Exemplo 1: Mensagem de exclusão reversível em um chat

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "chatmessagethis-softdelete1"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/8f98f01d-1a73-401a-b9e9-9fd1e6f5e5ar/chats/19:22273db3497f4b32bue61f6e82be21c5@thread.tacv2/messages/1649864053377/softDelete
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-soft-delete-message-in-a-channel"></a>Exemplo 2: Mensagem de exclusão reversível em um canal

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "chatmessagethis-softdelete2"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/172b0cce-e65d-44ce-9a49-91d9f2e8593a/channels/19:22273db3497f4b32bue61f6e82be21c5@thread.tacv2/messages/1649864053377/softDelete
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-soft-delete-message-of-a-reply"></a>Exemplo 3: Mensagem de exclusão reversível de uma resposta

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "chatmessagethis-softdelete3"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/172b0cce-e65d-44ce-9a49-91d9f2e8593a/channels/19:22273db3497f4b32bue61f6e82be21c5@thread.tacv2/messages/1649864053377/replies/1649852161658/softDelete
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->

``` http
HTTP/1.1 204 No Content
```
