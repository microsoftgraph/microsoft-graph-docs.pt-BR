---
title: Excluir anexo
description: Exclua um anexo de um evento de calendário, mensagem, tarefa do Outlook ou postagem.
ms.openlocfilehash: dbabde6b1783e477e3a15db3ea4d138be6e41b12
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771783"
---
# <a name="delete-attachment"></a>Excluir anexo

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Exclua um anexo de um [evento](../resources/event.md)do calendário, [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postar](../resources/post.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

* Se acessando anexos em mensagens: Mail.ReadWrite
* Se acessando anexos em eventos: Calendars.ReadWrite
* Se acessando anexos em tarefas do Outlook: Tasks.ReadWrite
* Se acessando anexos em postagens de grupo: Group.ReadWrite.All

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a>Solicitação HTTP

Anexos para um [evento](../resources/event.md).

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
-->

Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

Anexos de uma [mensagem](../resources/message.md) contidos em uma pasta filho de um [mailFolder](../resources/mailfolder.md) na caixa de correio do usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada no filho de um filho e assim por diante.
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

Anexos para uma [tarefa do Outlook](../resources/outlooktask.md).
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}
```

Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Veja um exemplo da solicitação para excluir um anexo em um evento.
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
