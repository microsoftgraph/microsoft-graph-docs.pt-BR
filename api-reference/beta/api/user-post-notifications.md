---
title: Criar e enviar uma notificação
description: Criar e enviar uma notificação direcionada a um usuário por meio do Microsoft Graph.
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 8eb35ea0ade2e7d471674d8d064ba0ac38b361cc
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996260"
---
# <a name="create-and-send-a-notification"></a>Criar e enviar uma notificação
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar e enviar uma notificação direcionada a um usuário por meio do Microsoft Graph. A notificação é armazenada no repositório de feeds de notificação do Microsoft Graph e é enviada a todos os clientes de aplicativos em todos os pontos de extremidade do dispositivo nos quais o usuário está conectado.  

## <a name="permissions"></a>Permissions
O serviço de aplicativo não requer nenhuma permissão adicional para postar notificações para o usuário de destino.  

> [!IMPORTANT]
> Se você optar por publicar notificações em nome de um usuário via permissões delegadas, uma das seguintes permissões é necessária para chamar essa API. Não recomendamos esta opção para postar notificações, mas se você quiser saber mais, incluindo como escolher permissões, consulte [permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Notifications.ReadWrite.CreatedByApp    |
|Delegado (conta pessoal da Microsoft) | Notifications.ReadWrite.CreatedByApp    |
| Aplicativo                           | Sem suporte. |


## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|Autorização | string |O cabeçalho de autorização é usado para passar as credenciais da parte de chamada. Portador {token}. Obrigatório. |
|X-UNS-ID | string |O UserNotificationSubscriptionId retornado pelo serviço de notificação do Microsoft Graph após a criação de uma assinatura no lado do cliente e é usado para direcionar o usuário específico. Obrigatório. |
|Content-type| application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON de um objeto [Notification](../resources/projectrome-notification.md) .

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201 Created` um código de resposta que indica que a notificação foi criada e armazenada com êxito. A notificação será subseqüentemente fanned a todos os pontos de extremidade especificados com uma assinatura válida. 

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_notification_from_user"
}-->

```http
POST https://graph.microsoft.com/beta/me/notifications
Content-type: application/json

{
  "notification": {
    "targetHostName": "targetHostName-value",
    "appNotificationId": "appNotificationID-value",
    "expirationDateTime": "datetime-value",
    "targetPolicy": {
      "platformTypes": [
        "platformTypes-value"
        ]
      }, 
    "payload": {
      "rawContent": "rawContent-value",
      "visualContent": {
        "title": "title-value",
        "body": "body-value"
      }
    },
    "displayTimeToLive": 99,
    "priority": "priority-value",
    "groupName": "groupName-value"
  }
}
```
# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-notification-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notification"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "notification": {
    "targetHostName": "targetHostName-value",
    "expirationDateTime": "datetime-value",
    "payload": {
      "rawContent": "rawContent-value",
      "visualContent": {
        "title": "title-value",
        "body": "body-value"
      }
    },
    "displayTimeToLive": 99,
    "priority": "priority-value",
    "groupName": "groupName-value"
  }
}
```
