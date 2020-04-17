---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações quando os dados de um recurso do Microsoft Graph são alterados.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: fb14da71db128d3180555d47405e0be0148118ab
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543342"
---
# <a name="create-subscription"></a>Criar assinatura

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Assinar um aplicativo de escuta para receber notificações quando o tipo de alterações solicitadas ocorrer em recursos específicos no Microsoft Graph.

## <a name="permissions"></a>Permissões

A criação de uma assinatura requer permissão de leitura para o recurso. Por exemplo, para obter notificações sobre mensagens, seu aplicativo precisa da permissão mail. Read. 
 
 Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Recurso com suporte | Delegada (conta corporativa ou de estudante) | Delegada (conta pessoal da Microsoft) | Aplicativo |
|:-----|:-----|:-----|:-----|
|[callRecord](../resources/callrecords-callrecord.md) (/Communications/callRecords) | Sem suporte | Sem suporte | CallRecords.Read.All  |
|[chat](../resources/chatmessage.md) (/Teams/{ID}/Channels/{ID}/Messages) | Sem suporte | Sem suporte | ChannelMessage.Read.All  |
|[chat](../resources/chatmessage.md) (/Teams/allMessages--todas as mensagens do canal na organização) | Sem suporte | Sem suporte | ChannelMessage.Read.All  |
|[chat](../resources/chatmessage.md) (/chats/{ID}/Messages) | Sem suporte | Sem suporte | Chat.Read.All  |
|[chat](../resources/chatmessage.md) (/chats/allMessages--todas as mensagens de chat na organização) | Sem suporte | Sem suporte | Chat.Read.All  |
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

### <a name="chatmessage-microsoft-teams"></a>Chat (Microsoft Teams)

as assinaturas do **chat** exigem [criptografia](/graph/webhooks-with-resource-data). A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado. Antes de criar uma assinatura do **chat** , você deve solicitar acesso. Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis). 

> **Observação:** `/teams/allMessages` e `/chats/allMessages` estão atualmente em versão prévia. Durante a visualização, você pode usar essa API sem taxas, sujeita aos [termos de uso das APIs da Microsoft](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context). No entanto, os usuários de aplicativos que usam a API podem ser solicitados a ter assinaturas para ofertas específicas do Microsoft 365. Na disponibilidade geral, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados acessados por meio da API.

### <a name="driveitem-onedrive"></a>driveItem (OneDrive)

Limitações adicionais se aplicam a assinaturas em itens do OneDrive. As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.

No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade. No OneDrive for Business, você pode assinar somente a pasta raiz. As notificações são enviadas pelos tipos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outras instâncias **driveItem** na sua hierarquia. Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.

### <a name="contact-event-and-message-outlook"></a>contato, evento e mensagem (Outlook)

Limitações adicionais se aplicam a assinaturas em itens do Outlook. As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.

- A permissão delegada oferece suporte à assinatura de itens em pastas somente na caixa de correio do usuário conectado. Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.
- Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:

  - Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.
  - Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.

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

Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [Subscription](../resources/subscription.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).
Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.

Esta solicitação cria uma assinatura para notificações sobre novos emails recebidos pelo usuário conectado no momento.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "updated",
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
|Email|me/mailfolders('inbox')/messages<br />me/messages|
|Contatos|me/contacts|
|Calendários|me/events|
|Usuários|usuários|
|Grupos|grupos|
|Conversas|groups('*{id}*')/conversations|
|Unidades|me/drive/root|
|Listar|sites/{site-ID}/Lists/{List-ID}|
|Alerta de segurança|security/alerts?$filter=status eq ‘New’|
|Registros de chamadas|comunicações/callRecords|

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
  "changeType": "updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

## <a name="notification-endpoint-validation"></a>Validação de ponto de extremidade da notificação

O ponto de extremidade de notificação de assinatura (especificado na propriedade **notificationUrl** ) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation). Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.

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
