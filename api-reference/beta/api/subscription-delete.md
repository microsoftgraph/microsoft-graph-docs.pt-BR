---
title: Excluir assinatura
description: Exclua uma assinatura.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: b1f54db3641993160b46a0ec6a79a96f2f349de3
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335371"
---
# <a name="delete-subscription"></a>Excluir assinatura

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exclua uma assinatura.

Consulte a tabela na seção [Permissões](#permissions) para obter a lista de recursos que oferecem suporte à inscrição para alterar notificações.

## <a name="permissions"></a>Permissões

Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API. Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).

| Recurso com suporte | Delegada (conta corporativa ou de estudante) | Delegada (conta pessoal da Microsoft) | Aplicativo |
|:-----|:-----|:-----|:-----|
|[callRecord](../resources/callrecords-callrecord.md) | Incompatível | Incompatível | CallRecords.Read.All  |
|[canais](../resources/channel.md) (/teams/getAllChannels todos – os canais em uma organização) | Incompatível  | Sem suporte | Channel.ReadBasic.All, ChannelSettings.Read.All |
|[canais](../resources/channel.md) (/teams/{id}/channels) | Channel.ReadBasic.All, ChannelSettings.Read.All  | Incompatível | Channel.ReadBasic.All, ChannelSettings.Read.All  |
|[chat](../resources/chat.md) chat (/conversa – todos os chats em uma organização) | Incompatível | Incompatível | Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[chat](../resources/chat.md) (/chats/{id}) | Chat.ReadBasic, Chat.Read, Chat.ReadWrite | Sem suporte | ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages) | ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All | Sem suporte | ChannelMessage.Read.Group*, ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização) | Sem suporte | Sem suporte | ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages) | Chat.Read, Chat.ReadWrite | Sem suporte | Chat.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização) | Sem suporte | Sem suporte | Chat.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/users/{id}/chats/getAllMessages -- mensagens de chat para todos os chats dos quais um usuário específico faz parte) | Chat.Read, Chat.ReadWrite | Sem suporte | Chat.Read.All, Chat.ReadWrite.All |
|[contato](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers) | Incompatível | Sem suporte | ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[conversationMember](../resources/conversationmember.md) (/chats/{id}/members) | ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite | Incompatível | ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[conversationMember](../resources/conversationmember.md) (/teams/getAllMembers) | Incompatível | Sem suporte | TeamMember.Read.All, TeamMember.ReadWrite.All |
|[conversationMember](../resources/conversationmember.md) (/teams/{id}/members) | TeamMember.Read.All | Incompatível | TeamMember.Read.All |
|[conversationMember](../resources/conversationmember.md) (/teams/{id}/channels/getAllMembers) | Incompatível | Incompatível | ChannelMember.Read.All |
|[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário) | Sem suporte | Files.ReadWrite | Sem suporte |
|[driveItem](../resources/driveitem.md) (OneDrive for Business) | Files.ReadWrite.All | Sem suporte | Files.ReadWrite.All |
|[evento](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[grupo](../resources/group.md) | Group.Read.All | Sem suporte | Group.Read.All |
|[conversa em grupo](../resources/conversation.md) | Group.Read.All | Sem suporte | Sem suporte |
|[list](../resources/list.md) | Sites.ReadWrite.All | Sem suporte | Sites.ReadWrite.All |
|[message](../resources/message.md) | Mail.ReadBasic, Mail.Read | Mail.ReadBasic, Mail.Read | Mail.ReadBasic, Mail.Read |
|[presence](../resources/presence.md) | Presence.Read.All | Incompatível | Incompatível |
|[printer](../resources/printer.md) | Sem suporte | Sem suporte | Printer.Read.All, Printer.ReadWrite.All |
|[printTaskDefinition](../resources/printtaskdefinition.md) | Sem suporte | Sem suporte | PrintTaskDefinition.ReadWrite.All |
|[alerta de segurança](../resources/alert.md) | SecurityEvents.ReadWrite.All | Sem suporte | SecurityEvents.ReadWrite.All |
|[teams](../resources/team.md) (/teams – todas as equipes em uma organização) | Sem suporte | Incompatível | Team.ReadBasic.All, TeamSettings.Read.All |
|[teams](../resources/team.md) (/teams/{id}) | Team.ReadBasic.All, TeamSettings.Read.All | Incompatível | Team.ReadBasic.All, TeamSettings.Read.All |
|[todoTask](../resources/todotask.md) | Tasks.ReadWrite | Tasks.ReadWrite | Sem suporte |
|[baseTask](../resources/basetask.md) | Tasks.ReadWrite | Tasks.ReadWrite | Incompatível |
|[user](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

> **Observação**: Permissões marcadas com * usam [consentimento específico de recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a>driveItem

As limitações adicionais se aplicam aos itens do OneDrive. As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).

No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade. No OneDrive for Business, você pode assinar somente a pasta raiz. As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia. Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.

### <a name="contact-event-and-message"></a>contato, evento e mensagem

Você Outlook pode assinar as alterações nos recursos de **contato, evento** ou mensagem e, opcionalmente **, especificar** na carga de solicitação POST se deve incluir dados de recursos criptografados em notificações.

[!INCLUDE [outlook-subscription-notes](../../includes/outlook-subscription-notes.md)]

### <a name="presence"></a>presença

**assinaturas** de presença exigem [criptografia](/graph/webhooks-with-resource-data). A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.

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
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
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

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-subscription-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-subscription-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

