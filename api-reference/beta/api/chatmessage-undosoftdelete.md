---
title: 'chatMessage: undoSoftDelete'
description: Restaurar uma única mensagem ou uma resposta de mensagem em um canal ou chat.
author: Ramjot Singh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.localizationpriority: medium
ms.openlocfilehash: 353b41cee2ab489f88eaec8b5a6d6f3d19560722
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768343"
---
# <a name="chatmessage-undosoftdelete"></a>chatMessage: undoSoftDelete

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Desfaça a exclusão [reversível de uma única mensagem](../resources/chatmessage.md) ou [uma resposta de mensagem](../resources/chatmessage.md) em um [canal](../resources/channel.md) ou [chat](../resources/chat.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

### <a name="permissions-for-channel"></a>Permissões para o canal

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
|Delegada (conta corporativa ou de estudante)| ChannelMessage.ReadWrite |
|Delegado (conta pessoal da Microsoft)| Sem suporte |
|Aplicativo| Sem suporte |

> **Observação**: as permissões marcadas com ** têm suporte apenas para compatibilidade com versões anteriores. Recomendamos que você atualize suas soluções para usar uma permissão alternativa listada na tabela anterior e evite usar essas permissões daqui para frente.

### <a name="permissions-for-chat"></a>Permissões para o chat

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
|Delegada (conta corporativa ou de estudante)| ChatMessage.ReadWrite |
|Delegado (conta pessoal da Microsoft)| Sem suporte |
|Aplicativo| Sem suporte |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{userId}/chats/{chatsId}/messages/{chatMessageId}/undoSoftDelete
POST /teams/{teamsId}/channels/{channelId}/messages/{chatMessageId}/undoSoftDelete
POST /teams/{teamId}/channels/{channelId}/messages/{messageId}/replies/{replyId}/undoSoftDelete
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

### <a name="example-1-undo-soft-deletion-of-a-message-in-a-chat"></a>Exemplo 1: Desfazer exclusão reversível de uma mensagem em um chat

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "chatmessagethis-undosoftdelete1"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/8f98f01d-1a73-401a-b9e9-9fd1e6f5e5ap/chats/19:22273db3497f4b32bue61f6e82be21c5@thread.tacv2/messages/1649864053377/undoSoftDelete
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-undo-soft-deletion-of-a-message-in-a-channel"></a>Exemplo 2: Desfazer exclusão reversível de uma mensagem em um canal

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "chatmessagethis2undosoftdelete2"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/172b0cce-e65d-44ce-9a49-91d9f2e8593a/channels/19:22273db3497f4b32bue61f6e82be21c5@thread.tacv2/messages/1649864053377/undoSoftDelete
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-undo-soft-deletion-of-a-message-of-a-reply-in-a-channel"></a>Exemplo 3: Desfazer a exclusão reversível de uma mensagem de uma resposta em um canal

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "chatmessagethis-undosoftdelete3"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/172b0cce-e65d-44ce-9a49-91d9f2e8593a/channels/19:22273db3497f4b32bue61f6e82be21c5@thread.tacv2/messages/1649864053377/undoSoftDelete
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->

``` http
HTTP/1.1 204 No Content
```
