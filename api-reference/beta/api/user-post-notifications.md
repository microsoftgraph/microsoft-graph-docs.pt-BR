---
title: Criar e enviar uma notificação
description: Criar e enviar uma notificação direcionada a um usuário por meio do Microsoft Graph.
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: b66544406372c2eaa7be6f8f4261c75cbd7c6c5e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451662"
---
# <a name="create-and-send-a-notification"></a>Criar e enviar uma notificação

Namespace: Microsoft. Graph[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar e enviar uma notificação direcionada a um usuário por meio do Microsoft Graph. A notificação é armazenada no repositório de feeds de notificação do Microsoft Graph e é enviada a todos os clientes de aplicativos em todos os pontos de extremidade do dispositivo nos quais o usuário está conectado.  

## <a name="permissions"></a>Permissões
O serviço de aplicativo não requer nenhuma permissão adicional para postar notificações para o usuário de destino.  

> [!IMPORTANT]
> Se você optar por publicar notificações em nome de um usuário via permissões delegadas, uma das seguintes permissões é necessária para chamar essa API. Não recomendamos esta opção para a criação de notificações. Se quiser saber mais, incluindo como escolher permissões, consulte [permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Notifications.ReadWrite.CreatedByApp    |
|Delegado (conta pessoal da Microsoft) | Notifications.ReadWrite.CreatedByApp    |
|Aplicativo | Sem suporte.|



## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome | Descrição|
|:----|:-----------|
|Autorização | O cabeçalho de autorização é usado para passar as credenciais da parte de chamada. Portador {token}. Obrigatório. |
|X-UNS-ID | O UserNotificationSubscriptionId retornado pelo serviço de notificação do Microsoft Graph após a criação de uma assinatura e é usado para direcionar o usuário específico. Obrigatório. |
|Content-type | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON de um objeto [Notification](../resources/projectrome-notification.md) .

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201 Created` um código de resposta que indica que a notificação foi criada e armazenada com êxito. A notificação será subseqüentemente fanned a todos os pontos de extremidade especificados com uma assinatura válida. 

A tabela a seguir lista os possíveis códigos de erro e resposta que podem ser retornados.

|Código de erro             | Descrition                             |
|:-----------------------------------|:----------------------------------------------------------|
|HttpStatusCode. BadRequest           | O corpo é uma matriz (não há suporte para várias notificações).|
|HttpStatusCode. BadRequest           | O corpo não corresponde ao contrato da API.               |
|HttpStatusCode. proibido            | O chamador está na lista de bloqueados.                          |
|HttpStatusCode. MethodNotAllowed     | Não há suporte para o método HTTP usado.                     |
|HttpStatusCode. BadRequest           | Cabeçalhos sem suporte estão presentes na solicitação. Não há suporte para dois cabeçalhos:<br/><br/>If-Modified-Since<br/>If-Range |                    
|HttpStatusCode. UnsupportedMediaType | O cabeçalho Content-Encoding está presente e tem valores de algoritmo de compactação diferentes de `Deflate` ou `Gzip`.  |
|HttpStatusCode. BadRequest           | Carga inválida.                                           |
|HttpStatusCode. proibido            | O chamador não está autorizado a atuar em nome do usuário ou enviar notificação para o usuário.                         |
|HttpStatusCode. não autorizado         |  O corpo da solicitação contém tipos de dados de atividade inválidos.        |
|HttpStatusCode. OK                   |  Atividade criada com êxito.                            |
|HttpStatusCode. não aceito        |  A solicitação foi limitada ou o servidor está ocupado.    |


## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

```http
POST https://graph.microsoft.com/beta/me/notifications/
Content-type: application/json

{
    "targetHostName": "graphnotifications.sample.windows.com",
    "appNotificationId": "testDirectToastNotification",
    "expirationDateTime": "2019-10-30T23:59:00.000Z",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    },
    "targetPolicy": {
        "platformTypes": [
    "windows",
    "ios",
    "android"
        ]
    },
    "priority": "High",
    "groupName": "TestGroup",
    "displayTimeToLive": "60"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta correspondente.

```http
HTTP/1.1 201
client-request-id: 71e62feb-8d72-4912-8b2c-4cee9d89e781
content-length: 356
content-type: application/json
location: https://graph.microsoft.com/beta/me/activities/119081f2-f19d-4fa8-817c-7e01092c0f7d
request-id: 71e62feb-8d72-4912-8b2c-4cee9d89e781

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('graphnotify%40contoso.com')/notifications/$entity",
    "displayTimeToLive": 59,
    "expirationDateTime": "2019-10-28T22:05:36.25Z",
    "groupName": "TestGroup",
    "id": "119081f2-f19d-4fa8-817c-7e01092c0f7d",
    "priority": "High",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    }
}
```
