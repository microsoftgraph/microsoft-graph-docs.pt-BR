---
title: Criar assinatura
description: Assinar um aplicativo de escuta para receber notificações quando as alterações de dados em um recurso do Microsoft Graph.
localization_priority: Normal
ms.openlocfilehash: 5b7f465e556d1fb752bcb2d3c962fd6444d462c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805050"
---
# <a name="create-subscription"></a>Criar assinatura

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Assinar um aplicativo de escuta para receber notificações quando as alterações de dados em um recurso do Microsoft Graph.

## <a name="permissions"></a>Permissions

Criar uma assinatura requer a permissão de leitura para o recurso para o qual o aplicativo receberá notificações. Por exemplo, para obter notificações sobre mensagens, seu aplicativo precisa o `Mail.Read` permissão. A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de recurso/item        | Permissão          |
|-----------------------------|---------------------|
| Contatos                    | Contacts.Read       |
| Conversas               | Group.Read.All      |
| Eventos                      | Calendars.Read      |
| Mensagens                    | Mail.Read           |
| Grupos                      | Group.Read.All      |
| Usuários                       | User.Read.All       |
| Drive (o OneDrive do usuário)    | Files.ReadWrite     |
| Drives (conteúdo do SharePoint shared e unidades) | Files.ReadWrite.All |
| Alerta de segurança              | SecurityEvents.ReadWrite.All |

> **Observação:** O ponto de extremidade /beta permite que as permissões de aplicativo para a maioria dos recursos. Não há suporte para conversas em itens de raiz uma unidade OneDrive e de grupo com permissões de aplicativo.

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

No corpo da solicitação, fornece uma representação JSON do objeto de [inscrição](../resources/subscription.md) .
O `clientState` campo é opcional.

Esta amostra da solicitação cria uma assinatura de notificações sobre novos emails recebidos pelo usuário atualmente conectado.
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

A seguir estão os valores válidos para a propriedade de recurso:

| Tipo de recurso | Exemplos |
|:------ |:----- |
|Email|me/mailfolders('inbox')/messages<br />me/messages|
|Contatos|me/contacts|
|Calendários|me/events|
|Usuários|users|
|Grupos|grupos|
|Conversas|groups('*{id}*')/conversations|
|Unidades|me/drive/root|
|Alerta de segurança|alertas de segurança /? $filter = status eq 'Novo'|

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

O ponto de extremidade de notificação de inscrição (especificado no `notificationUrl` propriedade) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [Configurar notificações para que as alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation). Se a validação falhar, a solicitação para criar a assinatura retornará um erro de solicitação inválida a 400.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
