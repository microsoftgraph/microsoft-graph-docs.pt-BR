---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações de alteração quando os dados de um recurso do Microsoft Graph são alterados.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 1301b8dc1b1e327b8bef573ec307ea25b066cf76
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643964"
---
# <a name="create-subscription"></a>Criar assinatura

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Inscreve um aplicativo de ouvinte para receber notificações de alterações quando o tipo de alteração solicitado ocorrer no recurso especificado no Microsoft Graph.

## <a name="permissions"></a>Permissões

A criação de uma assinatura requer permissão de leitura para o recurso. Por exemplo, para obter notificações de alteração em mensagens, seu aplicativo precisa da permissão mail. Read. 

 Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Recurso com suporte | Delegada (conta corporativa ou de estudante) | Delegada (conta pessoal da Microsoft) | Application |
|:-----|:-----|:-----|:-----|
|[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords) | Incompatível | Incompatível | CallRecords.Read.All  |
|[chat](../resources/chatmessage.md) (/Teams/{ID}/Channels/{ID}/Messages) | ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All | Sem suporte | ChannelMessage.Read.All  |
|[chat](../resources/chatmessage.md) (/Teams/allMessages--todas as mensagens do canal na organização) | Sem suporte | Sem suporte | ChannelMessage.Read.All  |
|[chat](../resources/chatmessage.md) (/chats/{ID}/Messages) | Chat.Read, Chat.ReadWrite | Sem suporte | Chat.Read.All  |
|[chat](../resources/chatmessage.md) (/chats/allMessages--todas as mensagens de chat na organização) | Sem suporte | Sem suporte | Chat.Read.All  |
|[contato](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário) | Sem suporte | Files.ReadWrite | Sem suporte |
|[driveItem](../resources/driveitem.md) (OneDrive for Business) | Files.ReadWrite.All | Sem suporte | Files.ReadWrite.All |
|[evento](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[grupo](../resources/group.md) | Group.Read.All | Sem suporte | Group.Read.All |
|[conversa em grupo](../resources/conversation.md) | Group.Read.All | Sem suporte | Sem suporte |
|[list](../resources/list.md) | Sites.ReadWrite.All | Sem suporte | Sites.ReadWrite.All |
|[message](../resources/message.md) | Mail.ReadBasic, Mail.Read | Mail.ReadBasic, Mail.Read | Mail.ReadBasic, Mail.Read |
|[presence](../resources/presence.md) | Presence.Read.All | Sem suporte | Sem suporte |
|[alerta de segurança](../resources/alert.md) | SecurityEvents.ReadWrite.All | Sem suporte | SecurityEvents.ReadWrite.All |
|[Usuário](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

### <a name="chatmessage"></a>chatMessage

as assinaturas do **chat** com permissões delegadas não dão suporte a dados de recurso (o**includeResourceData** deve ser `false` ) e não precisam de [criptografia](/graph/webhooks-with-resource-data).

as assinaturas do **chat** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data). A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado. Antes de criar uma assinatura do **chat** , você deve solicitar acesso. Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis). 

> **Observação:** `/teams/allMessages` e `/chats/allMessages` que estão atualmente em versão prévia, e você pode usar essa API sem taxas, sujeito aos [termos de uso das APIs da Microsoft](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context). A partir de agosto de 2020, só estará disponível para usuários e locatários que tenham as [licenças necessárias](/graph/teams-licenses). Como `/teams/allMessages` e `/chats/allMessages` enviar notificações para todos os usuários no locatário, todos os usuários no locatário devem ser licenciados. No futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados acessados por meio da API.

### <a name="driveitem"></a>driveItem

Limitações adicionais se aplicam a assinaturas em itens do OneDrive. As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.

No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade. No OneDrive for Business, você pode assinar somente a pasta raiz. As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia. Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.

### <a name="contact-event-and-message"></a>contato, evento e mensagem

Limitações adicionais se aplicam a assinaturas em itens do Outlook. As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.

- A permissão delegada oferece suporte à assinatura de itens em pastas somente na caixa de correio do usuário conectado. Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.
- Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:

  - Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.
  - Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.

### <a name="presence"></a>presença

as assinaturas de **presença** exigem [criptografia](/graph/webhooks-with-resource-data). A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [Subscription](../resources/subscription.md) no corpo da resposta.

Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).
Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.

Esta solicitação cria uma assinatura para notificações de alteração sobre novos emails recebidos pelo usuário conectado no momento.

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

---

Estes são os valores válidos para a Propriedade Resource.

| Tipo de recurso | Exemplos |
|:------ |:----- |
|[Registros de chamadas](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[Mensagem de chat](../resources/chatmessage.md) | `chats/{id}/messages`, `chats/allMessages`, `teams/{id}/channels/{id}/messages`, `teams/allMessages` |
|[Contatos](../resources/contact.md)|`me/contacts`|
|[Conversas](../resources/conversation.md)|`groups('{id}')/conversations`|
|[Unidades](../resources/driveitem.md)|`me/drive/root`|
|[Eventos](../resources/event.md)|`me/events`|
|[Grupos](../resources/group.md)|`groups`|
|[List](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[Email](../resources/message.md)|`me/mailfolders('inbox')/messages`, `me/messages`|
|[Presença](../resources/presence.md)| `/communications/presences/{id}`(usuário único), `/communications/presences?$filter=id in ({id},{id}…)` (vários usuários)|
|[Usuários](../resources/user.md)|`users`|
|[Alerta de segurança](../resources/alert.md)|`security/alerts?$filter=status eq 'New'`|

> **Observação:** Qualquer caminho iniciado com `me` também pode ser usado com `users/{id}` o ao invés de `me` direcionar um usuário específico, e não o usuário atual.

### <a name="response"></a>Resposta

O exemplo a seguir mostra a resposta. 

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

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
  "latestSupportedTlsVersion": "v1_2"
}
```

### <a name="notification-endpoint-validation"></a>Validação de ponto de extremidade de notificação

O ponto de extremidade de notificação de assinatura (especificado na propriedade **notificationUrl** ) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation). Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.

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
