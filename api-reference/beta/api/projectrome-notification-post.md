---
title: Criar e enviar uma notificação
description: 'Criar e enviar uma notificação direcionada a um usuário por meio do Microsoft Graph. A notificação é armazenada no repositório de feeds de notificação do Microsoft Graph e é enviada a todos os clientes de aplicativos em todos os pontos de extremidade do dispositivo nos quais o usuário está conectado.  '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 86e67d040dcae3a013d8848c638ffadca41e4f5f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331930"
---
# <a name="create-and-send-a-notification"></a>Criar e enviar uma notificação
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar e enviar uma notificação direcionada a um usuário por meio do Microsoft Graph. A notificação é armazenada no repositório de feeds de notificação do Microsoft Graph e é enviada a todos os clientes de aplicativos em todos os pontos de extremidade do dispositivo nos quais o usuário está conectado.  
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Notifications.ReadWrite.CreatedByApp    |
|Delegado (conta pessoal da Microsoft) | Notifications.ReadWrite.CreatedByApp    |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|Autorização | string |O cabeçalho de autorização é usado para passar as credenciais da parte de chamada. Portador {token}. Obrigatório. |
## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON de um objeto [Notification](../resources/projectrome-notification.md) .

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201 Created` o código de resposta que indica que a notificação foi criada e armazenada com êxito. 
## <a name="example"></a>Exemplo
#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

```http
POST https://graph.microsoft.com/beta/me/notifications/
Content-type: application/json

{
    "targetHostName": "graphnotifications.sample.windows.com",
    "appNotificationId": "testDirectToastNotification",
    "expirationDateTime": "2018-08-29T23:51:33.000Z",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    },
    "targetPolicy": {
        "platformTypes": [
        "windows",
        "android"
        ]
    },
    "priority": "High",
    "groupName": "TestGroup",
    "displayTimeToLive": "23"
}
```

#### <a name="response"></a>Resposta
Este é um exemplo de resposta.

```http
HTTP/1.1 201
Content-Type: application/json
location: https://graph.microsoft.com/beta/me/notifications/518c4fb1-c565-4d67-95c4-bcc3eb8eda1b

{
    "@odata.context": "https://graph.microsoft.com/test872018/$metadata#users('graphNotificationsUser%40contoso.com')/notifications/$entity",
    "appNotificationId": "testDirectToastNotification",
    "displayTimeToLive": 23,
    "expirationDateTime": "2018-08-24T12:31:53.858Z",
    "groupName": "TestGroup",
    "id": "cd5c5e6a-99ce-470a-9982-c47635e73620",
    "priority": "1",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    }
}
```


