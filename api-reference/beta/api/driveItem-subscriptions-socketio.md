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
# <a name="get-websocket-endpoint"></a><span data-ttu-id="e8530-103">Obtenha o ponto de extremidade do websocket</span><span class="sxs-lookup"><span data-stu-id="e8530-103">Get websocket endpoint</span></span>

> <span data-ttu-id="e8530-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e8530-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span>
<span data-ttu-id="e8530-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e8530-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8530-106">Permite que você receber notificações de alteração de quase em tempo real para uma [unidade][] usando o [socket.io][].</span><span class="sxs-lookup"><span data-stu-id="e8530-106">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="e8530-107">Socket.IO é uma biblioteca de notificações populares para JavaScript que utiliza o WebSocket.</span><span class="sxs-lookup"><span data-stu-id="e8530-107">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="e8530-108">Para saber mais, consulte [socket.io](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="e8530-108">To learn more, see [socket.io](https://socket.io).</span></span>

[unidade]: ../resources/drive.md
[drive]: ../resources/drive.md
[Socket.IO]: https://socket.io/
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="e8530-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="e8530-111">Permissions</span></span>

<span data-ttu-id="e8530-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8530-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8530-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8530-114">Permission type</span></span>                        | <span data-ttu-id="e8530-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8530-115">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="e8530-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8530-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8530-117">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8530-117">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="e8530-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8530-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8530-119">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8530-119">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="e8530-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8530-120">Application</span></span>                            | <span data-ttu-id="e8530-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8530-121">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="e8530-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8530-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="e8530-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8530-123">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8530-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8530-124">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="e8530-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8530-125">Response</span></span>

<span data-ttu-id="e8530-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [inscrição](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8530-126">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="e8530-127">O `notificationUrl` retornado é uma URL de ponto de extremidade socket.io.</span><span class="sxs-lookup"><span data-stu-id="e8530-127">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="e8530-128">Para usá-la com um cliente socket.io, dividir a cadeia de caracteres no `/callback?` token.</span><span class="sxs-lookup"><span data-stu-id="e8530-128">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="e8530-129">A parte da cadeia de caracteres antes `/callback?` é a URL do ponto de extremidade de socket.io e a parte da cadeia de caracteres após é uma sequência de caracteres de consulta opaco que deve ser fornecida para a biblioteca.</span><span class="sxs-lookup"><span data-stu-id="e8530-129">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="e8530-130">O exemplo a seguir mostra como usar o `notificationUrl` com socket.io em JavaScript.</span><span class="sxs-lookup"><span data-stu-id="e8530-130">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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
