---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações quando os dados de um recurso do Microsoft Graph são alterados.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: a8b8189780ac0b820551fb885adcf843c9ebe8f4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140163"
---
# <a name="create-subscription"></a>Criar assinatura

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Assina um aplicativo de escuta para receber notificações quando o tipo solicitado de alterações ocorre no recurso especificado no Microsoft Graph.

## <a name="permissions"></a>Permissões

A criação de uma assinatura requer o escopo de leitura para o recurso. Por exemplo, para obter notificações sobre mensagens, seu aplicativo precisa da `Mail.Read` permissão. 
 
 Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o menos privilegiado necessário para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Recurso com suporte | Delegada (conta corporativa ou de estudante) | Delegada (conta pessoal da Microsoft) | Application |
|:-----|:-----|:-----|:-----|
|[contato](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[driveItem](../resources/driveitem.md) (OneDrive pessoal do usuário) | Sem suporte | Files.ReadWrite | Sem suporte |
|[driveItem](../resources/driveitem.md) (OneDrive for Business) | Files.ReadWrite.All | Sem suporte | Files.ReadWrite.All |
|[event](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[grupo](../resources/group.md) | Group.Read.All | Sem suporte | Group.Read.All |
|[conversa de grupo](../resources/conversation.md) | Group.Read.All | Sem suporte | Sem suporte |
|[message](../resources/message.md) | Mail.Read | Mail.Read | Mail.Read |
|[alerta de segurança](../resources/alert.md) | SecurityEvents.ReadWrite.All | Sem suporte | SecurityEvents.ReadWrite.All |
|[user](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

> **Observação:** Há limitações adicionais para assinaturas em itens do OneDrive e do Outlook. As limitações se aplicam à criação e ao gerenciamento de assinaturas (obtendo, atualizando e excluindo assinaturas).

- No OneDrive pessoal, você pode inscrever-se na pasta raiz ou em qualquer subpasta nessa unidade. No OneDrive for Business, você pode inscrever-se apenas na pasta raiz. As notificações são enviadas para os tipos solicitados de alterações na pasta inscrita ou qualquer arquivo, pasta ou outra instância do **driveItem** em sua hierarquia. Você não pode se inscrever em instâncias de **unidade** ou **driveItem** que não são pastas, como arquivos individuais.

- No Outlook, a permissão delegada oferece suporte à assinatura de itens em pastas somente na caixa de correio do usuário conectado. Isso significa que, por exemplo, não é possível usar os calendários de permissão delegada. Leia para inscrever-se em eventos na caixa de correio de outro usuário.
- Para inscrever-se para alterar as notificações de contatos, eventos ou mensagens do Outlook em pastas compartilhadas _ou delegadas_ :

  - Use a permissão de aplicativo correspondente para inscrever-se nas alterações de itens em uma pasta ou em uma caixa de correio de _qualquer_ usuário no locatário.
  - Não use as permissões de compartilhamento do Outlook (Contacts. Read. Shared, caLendars. Read. Shared, mail. Read. Shared e suas contrapartes de leitura/gravação), já que eles **não** oferecem suporte à inscrição para alterar notificações em itens em pastas compartilhadas ou delegadas.

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

Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

No corpo da solicitação, forneça uma representação JSON do objeto [Subscription](../resources/subscription.md) .
O `clientState` campo é opcional.

Este exemplo de solicitação cria uma assinatura para notificações sobre novos emails recebidos pelo usuário conectado no momento.
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

Estes são os valores válidos para a propriedade de recurso:

| Tipo de recurso | Exemplos |
|:------ |:----- |
|Email|me/mailfolders('inbox')/messages<br />me/messages|
|Contatos|me/contacts|
|Calendários|me/events|
|Usuários|users|
|Grupos|Agrupe|
|Conversas|groups('*{id}*')/conversations|
|Unidades|me/drive/root|
|Alerta de segurança|segurança/alertas? $filter = status eq ' novo '|

##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
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
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a>Validação de ponto de extremidade de notificação

O ponto de extremidade de notificação de assinatura `notificationUrl` (especificado na propriedade) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation). Se a validação falhar, a solicitação para criar a assinatura retornará um erro de solicitação inVálida 400.

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
    "Error: /api-reference/beta/api/subscription-post-subscriptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
