---
title: Criar assinatura
description: Inscreve um aplicativo ouvinte para receber notificações de alteração quando os dados em um recurso microsoft Graph alterações.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 3746db66d1f79c27d0910de55f9a20b08214b653
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395654"
---
# <a name="create-subscription"></a>Criar assinatura

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Inscreve um aplicativo de ouvinte para receber notificações de alterações quando o tipo de alteração solicitado ocorrer no recurso especificado no Microsoft Graph.

Consulte a tabela na seção [Permissões](#permissions) para obter a lista de recursos que oferecem suporte à inscrição para alterar notificações.

Alguns recursos suportam a opção de incluir dados de recursos criptografados em notificações de alteração. Esses recursos [incluem chatMessage](../resources/chatmessage.md), [contato](../resources/contact.md), [evento](../resources/event.md), [mensagem](../resources/message.md), [onlineMeetings](../resources/onlinemeeting.md) e [presença](../resources/presence.md). Para obter mais informações, consulte [Configurar notificações de alteração que incluem dados de recursos](/graph/webhooks-with-resource-data) e [Notificações de alteração para recursos do Outlook no Microsoft Graph](/graph/outlook-change-notification-overview).

## <a name="permissions"></a>Permissões

A criação de uma assinatura requer permissão de leitura para o recurso. Por exemplo, para receber notificações de alteração nas mensagens, seu aplicativo precisa da permissão Mail.Read. 

Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API. Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).

| Recurso com suporte | Delegada (conta corporativa ou de estudante) | Delegada (conta pessoal da Microsoft) | Application |
|:-----|:-----|:-----|:-----|
|[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords) | Incompatível | Incompatível | CallRecords.Read.All  |
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
|[reunião online](../resources/onlinemeeting.md) | Incompatível | Sem suporte | OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All |
|[presence](../resources/presence.md) | Presence.Read.All | Incompatível | Incompatível |
|[printer](../resources/printer.md) | Sem suporte | Sem suporte | Printer.Read.All, Printer.ReadWrite.All |
|[printTaskDefinition](../resources/printtaskdefinition.md) | Sem suporte | Sem suporte | PrintTaskDefinition.ReadWrite.All |
|[alerta de segurança](../resources/alert.md) | SecurityEvents.ReadWrite.All | Sem suporte | SecurityEvents.ReadWrite.All |
|[teams](../resources/team.md) (/teams – todas as equipes em uma organização) | Sem suporte | Incompatível | Team.ReadBasic.All, TeamSettings.Read.All |
|[teams](../resources/team.md) (/teams/{id}) | Team.ReadBasic.All, TeamSettings.Read.All | Incompatível | Team.ReadBasic.All, TeamSettings.Read.All |
|[todoTask](../resources/todotask.md) | Tasks.ReadWrite | Tasks.ReadWrite | Sem suporte |
|[baseTask](../resources/basetask.md) | Tasks.ReadWrite | Tasks.ReadWrite | Incompatível |
|[Usuário](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

> **Observação**: Permissões marcadas com * usam [consentimento específico de recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a>driveItem

As limitações adicionais se aplicam aos itens do OneDrive. As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).

No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade. No OneDrive for Business, você pode assinar somente a pasta raiz. As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia. Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.

OneDrive for Business e Microsoft Office SharePoint Online suportam o envio de notificações de aplicações de eventos de segurança que ocorrem em um **driveItem**. Para se inscrever nestes eventos, adicionar o cabeçalho `prefer:includesecuritywebhooks` a sua solicitação para criar uma assinatura. Após a criação da assinatura, você receberá notificações quando as permissões sobre uma mudança de item forem alteradas. Este cabeçalho é aplicável às contas Microsoft Office SharePoint Online e OneDrive for Business, mas não às contas OneDrive de consumo.

### <a name="contact-event-and-message"></a>contato, evento e mensagem

Você Outlook pode assinar as alterações nos recursos de **contato, evento** ou mensagem e, opcionalmente **, especificar** na carga de solicitação POST se deve incluir dados de recursos criptografados em notificações.

[!INCLUDE [outlook-subscription-notes](../../includes/outlook-subscription-notes.md)]

### <a name="presence"></a>presença

As assinaturas na **presença** exigem que todos os dados de recursos incluídos em uma notificação de alteração sejam criptografados. Sempre especifique o parâmetro **encryptionCertificate** ao [criar uma assinatura](/graph/webhooks-with-resource-data#creating-a-subscription) para evitar falha. Veja mais informações sobre como[ configurar notificações de mudança para incluir dados de recursos](/graph/webhooks-with-resource-data).

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do objeto de [assinatura](../resources/subscription.md).

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [subscription](../resources/subscription.md) no corpo da resposta.

Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

No corpo da solicitação, forneça uma representação JSON do objeto de [assinatura](../resources/subscription.md). Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.

Essa solicitação cria uma assinatura para notificações de alteração sobre novos emails recebidos pelo usuário atualmente inscrito.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-subscription-from-subscriptions-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-subscription-from-subscriptions-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

No corpo da solicitação, forneça uma representação JSON do objeto de [assinatura](../resources/subscription.md). Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.

#### <a name="resources-examples"></a>Exemplos de recursos

Os valores a seguir são válidos para a propriedade resource.

| Tipo de recurso | Exemplos |
|:------ |:----- |
|[Registros de chamadas](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[Canais](../resources/channel.md)|`/teams/getAllChannels`, `/teams/{id}/channels`|
|[Chat](../resources/chat.md)|`/chats`, `/chats/{id}`|
|[Mensagem de chat](../resources/chatmessage.md) | `chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages` |
|[Contatos](../resources/contact.md)|`me/contacts`|
|[ConversationMember](../resources/conversationmember.md)|`/chats/{id}/members`, `/chats/getAllMembers`, `/teams/{id}/members`, `/teams/getAllMembers`, `/teams/{id}/channels/getAllMembers`|
|[Conversas](../resources/conversation.md)|`groups('{id}')/conversations`|
|[Unidades](../resources/driveitem.md)|`me/drive/root`|
|[Eventos](../resources/event.md)|`me/events`|
|[Grupos](../resources/group.md)|`groups`|
|[Lista](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[Email](../resources/message.md)|`me/mailfolders('inbox')/messages`, `me/messages`|
|[OnlineMeetings](../resources/onlinemeeting.md)|`/communications/onlineMeetings/?$filter=JoinWebUrl eq '{WebJoinUrl}'`|
|[Presença](../resources/presence.md)| `/communications/presences/{id}` (usuário único), `/communications/presences?$filter=id in ('{id}','{id}',…)` (vários usuários)|
|[impressora](../resources/printer.md) |`print/printers/{id}/jobs`|
|[printTaskDefinition](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[Teams](../resources/team.md)|`/teams`, `/teams/{id}`|
|[Usuários](../resources/user.md)|`users`|
|[todoTask](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[baseTask](../resources/basetask.md) | `/me/tasks/lists/{baseTaskListId}/tasks`, `/me/tasks/alltasks`
|[Alerta de segurança](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> **Observação:** qualquer caminho iniciado por `me` também pode ser usado com `users/{id}` em vez de `me` para direcionar um usuário específico, em vez de usar o usuário atual.

### <a name="response"></a>Resposta

O exemplo a seguir mostra a resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "notificationContentType": "application/json"
}
```

#### <a name="notification-endpoint-validation"></a>Validação de ponto de extremidade da notificação

O ponto de extremidade de notificação de assinatura (especificado na propriedade **notificationUrl** ) deve ser capaz de responder a uma solicitação de validação conforme descrito em Configurar notificações para alterações nos dados [do usuário](/graph/webhooks#notification-endpoint-validation). Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.

[error-response]: /graph/errors

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

