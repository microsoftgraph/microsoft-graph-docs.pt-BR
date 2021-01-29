---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4b4b05d659453ef0867d60f3d43d137f4b697874
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034069"
---
# <a name="delete-subscription"></a>Excluir assinatura

Namespace: microsoft.graph

Exclua uma assinatura.

## <a name="permissions"></a>Permissões

Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Recurso com suporte | Delegada (conta corporativa ou de estudante) | Delegada (conta pessoal da Microsoft) | Aplicativo |
|:-----|:-----|:-----|:-----|
|[callRecord](../resources/callrecords-callrecord.md) | Incompatível | Incompatível | CallRecords.Read.All |
|[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages) | Sem suporte | Sem suporte |  ChannelMessage.Read.Group*, ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização) | Sem suporte | Sem suporte | ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages) | Sem suporte | Sem suporte | Chat.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização) | Sem suporte | Sem suporte | Chat.Read.All  |
|[contato](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário) | Sem suporte | Files.ReadWrite | Sem suporte |
|[driveItem](../resources/driveitem.md) (OneDrive for Business) | Files.ReadWrite.All | Sem suporte | Files.ReadWrite.All |
|[evento](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[grupo](../resources/group.md) | Group.Read.All | Sem suporte | Group.Read.All |
|[conversa em grupo](../resources/conversation.md) | Group.Read.All | Sem suporte | Sem suporte |
|[list](../resources/list.md) | Sites.ReadWrite.All | Sem suporte | Sites.ReadWrite.All |
|[message](../resources/message.md) | Mail.ReadBasic, Mail.Read | Mail.ReadBasic, Mail.Read | Mail.ReadBasic, Mail.Read |
|[alerta de segurança](../resources/alert.md) | SecurityEvents.ReadWrite.All | Sem suporte | SecurityEvents.ReadWrite.All |
|[Usuário](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

> **Observação**: Permissões marcadas com * usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a>driveItem

As limitações adicionais se aplicam aos itens do OneDrive. As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).

No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade. No OneDrive for Business, você pode assinar somente a pasta raiz. As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia. Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.

### <a name="contact-event-and-message"></a>contato, evento e mensagem

As limitações adicionais se aplicam aos itens do Outlook. As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).

- A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado. Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.
- Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:

  - Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.
  - Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.


## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.
Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

