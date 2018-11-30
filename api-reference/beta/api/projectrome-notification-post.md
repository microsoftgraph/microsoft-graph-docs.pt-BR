---
title: Criar e enviar uma notificação
description: 'Criar e enviar uma notificação de direcionamento de um usuário por meio do Microsoft Graph. A notificação é armazenada na notificação Microsoft Graph feed repositório e é enviada a todos os clientes de aplicativo em todos os pontos de extremidade do dispositivo que o usuário está conectado ao.  '
ms.openlocfilehash: 7855d8b369a2efc6dada33c66c12ae76384a2760
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038498"
---
# <a name="create-and-send-a-notification"></a>Criar e enviar uma notificação
> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Criar e enviar uma notificação de direcionamento de um usuário por meio do Microsoft Graph. A notificação é armazenada na notificação Microsoft Graph feed repositório e é enviada a todos os clientes de aplicativo em todos os pontos de extremidade do dispositivo que o usuário está conectado ao.  
## <a name="permissions"></a>Permissions
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
|Autorização | string |O cabeçalho de autorização é usado para passar as credenciais do chamador. Portador {token}. Obrigatório. |
## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de um objeto de [notificação](../resources/projectrome-notification.md) .

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará o `201 Created` código de resposta que indica que a notificação foi criada com êxito e armazenada. 
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


