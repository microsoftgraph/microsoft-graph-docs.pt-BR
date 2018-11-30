---
title: Obtenha o ponto de extremidade do websocket
description: Não há suporte para o uso dessas APIs em aplicativos de produção.
ms.openlocfilehash: c84bc3bdd3096a745cf21f282273694e63ab3afb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034577"
---
# <a name="get-websocket-endpoint"></a>Obtenha o ponto de extremidade do websocket

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.
Não há suporte para o uso dessas APIs em aplicativos de produção.

Permite que você receber notificações de alteração de quase em tempo real para uma [unidade][] usando o [socket.io][].
Socket.IO é uma biblioteca de notificações populares para JavaScript que utiliza o WebSocket. Para saber mais, consulte [socket.io](https://socket.io).

[unidade]: ../resources/drive.md
[Socket.IO]: https://socket.io/

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)
|:---------------------------------------|:-------------------------------------------
| Delegado (conta corporativa ou de estudante)     | Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All
| Delegado (conta pessoal da Microsoft) | Files.Read, Files.ReadWrite, Files.ReadWrite.All
| Aplicativo                            | Sem suporte.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [inscrição](../resources/subscription.md) no corpo da resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "opaqueId-fj3hd7yf283jfk193726nvc2w3i2diemdu8",
  "notificationUrl": "https://f3hb0mpua.svc.ms/zbaehwg/callback?snthgk=1ff3-2345672zz831837523"
}
```

O `notificationUrl` retornado é uma URL de ponto de extremidade socket.io.
Para usá-la com um cliente socket.io, dividir a cadeia de caracteres no `/callback?` token.
A parte da cadeia de caracteres antes `/callback?` é a URL do ponto de extremidade de socket.io e a parte da cadeia de caracteres após é uma sequência de caracteres de consulta opaco que deve ser fornecida para a biblioteca.

O exemplo a seguir mostra como usar o `notificationUrl` com socket.io em JavaScript.

```javascript
// this is the notificationUrl returned from this API
var notificationUrl = "https://f3hb0mpua.svc.ms/zbaehwg/callback?snthgk=1ff3-2345672zz831837523";

// after the split, split[0] will be everything leading up to '/callback?' and split[1] will be everything after.
var split = notificationUrl.split("/callback?");

// 'io' comes from the socket.io client library
var socket = io(split[0], { query: split[1] });

// these examples log to the console.
// your app would provide its own callbacks
socket.on("connect", ()=>console.log("Connected!"));
socket.on("notification", (data)=>console.log("Notification!", data));
```

<!-- {
  "type": "#page.annotation"
}-->
