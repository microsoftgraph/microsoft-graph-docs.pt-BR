---
title: Criar e enviar uma notificação (preterida)
description: Crie e envie uma notificação voltada para um usuário por meio do Microsoft Graph.
ms.localizationpriority: medium
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 33346ef8a625b08652c3b11d8ac9e4e3b17e6060
ms.sourcegitcommit: 7a0f9f1a535795c6f77c80e02fd97581c36f1273
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/27/2021
ms.locfileid: "61608910"
---
# <a name="create-and-send-a-notification-deprecated"></a>Criar e enviar uma notificação (preterida)

Namespace: microsoft.graph

> [!IMPORTANT]
> A API Graph de notificações da Microsoft está preterida e interromperá o retorno de dados até o final de janeiro de 2022. Para obter uma experiência de notificação alternativa, [consulte Microsoft Azure Hubs](/azure/notification-hubs)de Notificação e confira [esta postagem de blog](https://devblogs.microsoft.com/microsoft365dev/retiring-microsoft-graph-notifications/) para obter mais informações.

Crie e envie uma notificação voltada para um usuário por meio do Microsoft Graph. A notificação é armazenada no armazenamento de feed de notificação do Microsoft Graph e é enviada a todos os clientes de aplicativos em todos os pontos de extremidade do dispositivo aos que o usuário está conectado.  

## <a name="permissions"></a>Permissões
Seu serviço de aplicativo não exige permissões adicionais para postar notificações ao usuário direcionado.  

> [!IMPORTANT]
> Se você optar por postar notificações em nome de um usuário por meio de permissões delegadas, uma das seguintes permissões será necessária para chamar essa API. Não recomendamos essa opção para criar notificações. Se você quiser saber mais, incluindo como escolher permissões, consulte [Permissões](/graph/permissions-reference).

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
|Autorização | O header de autorização é usado para passar as credenciais do chamador. Portador {token}. Obrigatório. |
|X-UNS-ID | O UserNotificationSubscriptionId retornado pelo serviço de notificação do Microsoft Graph após a criação de uma assinatura e é usado para direcionar o usuário específico. Obrigatório. |
|Content-type | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de um [objeto de](../resources/projectrome-notification.md) notificação.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta que indica que a notificação foi criada `201 Created` e armazenada com êxito. A notificação será subsequentemente fanned-out para todos os pontos de extremidade especificados com uma assinatura válida. 

A tabela a seguir lista os códigos de erro e resposta possíveis que podem ser retornados.

|Código de erro             | Descrition                              |
|:-----------------------------------|:----------------------------------------------------------|
|HttpStatusCode.BadRequest           | Body é uma matriz (não há suporte para várias notificações).|
|HttpStatusCode.BadRequest           | Body não combina com o contrato da API.               |
|HttpStatusCode.Forbidden            | O chamador está na lista bloqueada.                          |
|HttpStatusCode.MethodNotAllowed     | O método HTTP usado não é suportado.                     |
|HttpStatusCode.BadRequest           | Os headers sem suporte estão presentes na solicitação. Não há suporte para dois headers:<br/><br/>If-Modified-Since<br/>If-Range |                    
|HttpStatusCode.UnsupportedMediaType | O header Content-Encoding está presente e tem valores de algoritmo de compactação diferentes `Deflate` ou `Gzip` .  |
|HttpStatusCode.BadRequest           | Carga inválida.                                           |
|HttpStatusCode.Forbidden            | O chamador não está autorizado a agir em nome do usuário ou enviar notificação ao usuário.                         |
|HttpStatusCode.Unauthorized         |    O corpo da solicitação contém tipos de dados de atividade inválidos.        |
|HttpStatusCode.OK                   |     Atividade criada com êxito.                            |
|HttpStatusCode.NotAcceptable        |    A solicitação foi acelerada ou o servidor está ocupado.    |


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
A seguir, um exemplo da resposta correspondente.

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


