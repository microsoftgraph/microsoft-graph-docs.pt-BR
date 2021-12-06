---
title: Listar assinaturas
description: " consulte os cenários abaixo para obter detalhes."
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 578e512509ecd202f30ab32bef6102b1b3253be0
ms.sourcegitcommit: e75969aa44a1aab722ac44d09c37508ffbad8738
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/04/2021
ms.locfileid: "61307633"
---
# <a name="list-subscriptions"></a>Listar assinaturas

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de assinaturas de webhook. 

O conteúdo da resposta depende do contexto no qual o aplicativo está chamando; para obter detalhes, consulte os cenários na [seção](#permissions) Permissões.

## <a name="permissions"></a>Permissões

Esta API suporta os seguintes escopos de permissão; para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Recurso com suporte | Delegada (conta corporativa ou de estudante) | Delegada (conta pessoal da Microsoft) | Application |
|:-----|:-----|:-----|:-----|
|[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords) | Incompatível | Incompatível | CallRecords.Read.All  |
|[canais](../resources/channel.md) (/teams/getAllChannels – todos os canais em uma organização) | Incompatível  | Incompatível | Channel.ReadBasic.All, ChannelSettings.Read.All |
|[canais](../resources/channel.md) (/teams/{id}/channels) | Channel.ReadBasic.All, ChannelSettings.Read.All, Subscription.Read.All  | Sem suporte | Channel.ReadBasic.All, ChannelSettings.Read.All  |
|[chat](../resources/chat.md) (/chats – todos os chats em uma organização) | Incompatível | Incompatível | Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[chat](../resources/chat.md) (/chats/{id}) | Chat.ReadBasic, Chat.Read, Chat.ReadWrite, Subscription.Read.All | Sem suporte | ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages) | ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All, Subscription.Read.All | Sem suporte | ChannelMessage.Read.Group*, ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização) | Sem suporte | Sem suporte | ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages) | Chat.Read, Chat.ReadWrite, Subscription.Read.All | Sem suporte | Chat.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização) | Sem suporte | Sem suporte | Chat.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/users/{id}/chats/getAllMessages -- mensagens de chat para todos os chats de que um determinado usuário faz parte) | Chat.Read, Chat.ReadWrite, Subscription.Read.All | Sem suporte | Chat.Read.All, Chat.ReadWrite.All |
|[contato](../resources/contact.md) | Contacts.Read, Subscription.Read.All | Contacts.Read, Subscription.Read.All | Contacts.Read |
|[conversationMember](../resources/conversationmember.md) (/teams/{id}/channels/getAllMembers) | Incompatível | Incompatível | ChannelMember.Read.All |
|[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers) | Incompatível | Sem suporte | ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[conversationMember](../resources/conversationmember.md) (/chats/{id}/members) | ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite, Subscription.Read.All | Incompatível | ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[conversationMember](../resources/conversationmember.md) (/teams/{id}/members) | TeamMember.Read.All, Subscription.Read.All | Incompatível | TeamMember.Read.All |
|[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário) | Sem suporte | Files.ReadWrite, Subscription.Read.All | Sem suporte |
|[driveItem](../resources/driveitem.md) (OneDrive for Business) | Files.ReadWrite.All, Subscription.Read.All | Sem suporte | Files.ReadWrite.All |
|[evento](../resources/event.md) | Calendars.Read, Subscription.Read.All | Calendars.Read, Subscription.Read.All | Calendars.Read |
|[grupo](../resources/group.md) | Group.Read.All, Subscription.Read.All | Sem suporte | Group.Read.All |
|[conversa em grupo](../resources/conversation.md) | Group.Read.All, Subscription.Read.All | Incompatível | Sem suporte |
|[list](../resources/list.md) | Sites.ReadWrite.All, Subscription.Read.All | Sem suporte | Sites.ReadWrite.All |
|[message](../resources/message.md) | Mail.ReadBasic, Mail.Read, Subscription.Read.All | Mail.ReadBasic, Mail.Read, Subscription.Read.All | Mail.ReadBasic, Mail.Read |
|[presence](../resources/presence.md) | Presence.Read.All, Subscription.Read.All | Sem suporte | Incompatível |
|[printer](../resources/printer.md) | Sem suporte | Sem suporte | Printer.Read.All, Printer.ReadWrite.All |
|[printTaskDefinition](../resources/printtaskdefinition.md) | Sem suporte | Sem suporte | PrintTaskDefinition.ReadWrite.All |
|[alerta de segurança](../resources/alert.md) | SecurityEvents.ReadWrite.All, Subscription.Read.All | Sem suporte | SecurityEvents.ReadWrite.All |
|[teams](../resources/team.md) (/teams – todas as equipes em uma organização) | Sem suporte | Incompatível | Team.ReadBasic.All, TeamSettings.Read.All |
|[teams](../resources/team.md) (/teams/{id}) | Team.ReadBasic.All, TeamSettings.Read.All, Subscription.Read.All | Incompatível | Team.ReadBasic.All, TeamSettings.Read.All |
|[todoTask](../resources/todotask.md) | Tasks.ReadWrite, Subscription.Read.All | Tasks.ReadWrite, Subscription.Read.All | Incompatível |
|[user](../resources/user.md) | User.Read.All, Subscription.Read.All | User.Read.All | User.Read.All |

> **Observação**: Permissões marcadas com * usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).

Os resultados da resposta são baseados no contexto do aplicativo de chamada. As seções a seguir descrevem os cenários comuns.

### <a name="basic-scenarios"></a>Cenários Básicos

Comumente, um aplicativo deseja recuperar assinaturas originalmente criadas para o usuário atualmente conectado ou para todos os usuários no diretório (contas corporativas/de estudante). Esses cenários não exigem permissões especiais além daquelas usadas originalmente pelo aplicativo para criar suas assinaturas.

| Contexto do aplicativo de chamada | A resposta contém |
|:-----|:---------------- |
| O aplicativo está chamando em nome do usuário conectado (permissão delegada). <br/>-e-<br/>O aplicativo tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).<br/><br/>**Observação:** Isso se aplica a contas pessoais da Microsoft e contas de trabalho/escola. | Assinaturas criadas por **este aplicativo** apenas para o usuário conectado. |
| O aplicativo está chamando em nome de si mesmo (permissão de aplicativo).<br/>-e-<br/>O aplicativo tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).<br/><br/>Nota: Isso se aplica apenas a contas de trabalho/escola.| Assinaturas criadas por **este aplicativo** para si ou para qualquer usuário no diretório.|

### <a name="advanced-scenarios"></a>Cenários avançados

Em alguns casos, um aplicativo deseja recuperar assinaturas criadas por outros aplicativos. Por exemplo, um usuário deseja ver todas as assinaturas criadas por qualquer aplicativo em seu nome. Ou, um administrador pode querer ver todas as assinaturas de todos os aplicativos em seu diretório.
Para esses cenários, é necessária uma permissão delegada Subscription.Read.All.

| Contexto do aplicativo de chamada | A resposta contém |
|:-----|:---------------- |
| O aplicativo está chamando em nome do usuário conectado (permissão delegada). *O usuário é um não administrador*. <br/>-e-<br/>O aplicativo tem a permissão Subscription.Read.All<br/><br/>Nota: Isso se aplica a contas pessoais da Microsoft e contas de trabalho/escola. | Assinaturas criadas por **qualquer aplicativo** apenas para o usuário conectado. |
| O aplicativo está chamando em nome do usuário conectado (permissão delegada). *O usuário é um administrador*.<br/>-e-<br/>O aplicativo tem a permissão Subscription.Read.All<br/><br/>Nota: Isso se aplica apenas a contas de trabalho/escola. | Assinaturas criadas por **qualquer aplicativo** para **qualquer usuário** no diretório.|

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método não dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem sucedido, este método retorna um código de resposta `200 OK` e uma lista de objetos de [assinatura](../resources/subscription.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-subscriptions-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta. 

>**Observação:** A resposta mostrada aqui pode ser reduzida para a capacidade de leitura.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions",
  "value": [
    {
      "id": "0fc0d6db-0073-42e5-a186-853da75fb308",
      "resource": "Users",
      "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
      "changeType": "updated,deleted",
      "clientState": null,
      "notificationUrl": "https://webhookappexample.azurewebsites.net/api/notifications",
      "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
      "latestSupportedTlsVersion": "v1_2",
      "encryptionCertificate": "",
      "encryptionCertificateId": "",
      "includeResourceData": false,
      "notificationContentType": "application/json"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

> **Observação:** o valor da propriedade `clientState` não é retornado para fins de segurança.

Quando uma solicitação retorna várias páginas de dados, a resposta inclui uma propriedade `@odata.nextLink` para ajudá-lo a gerenciar os resultados. Para saber mais, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).
