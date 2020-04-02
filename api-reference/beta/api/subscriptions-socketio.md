---
author: learafa
ms.author: learafa
title: Obter ponto de extremidade do WebSocket
description: Não há suporte para o uso dessas APIs em aplicativos de produção.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 067fc455a0a122761c45ac1078712ea04b68845c
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43109184"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="76594-103">Obter ponto de extremidade do WebSocket</span><span class="sxs-lookup"><span data-stu-id="76594-103">Get websocket endpoint</span></span>

<span data-ttu-id="76594-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76594-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="76594-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="76594-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76594-106">Permite que você receba notificações de alteração quase em tempo real para uma [unidade][] e [lista][] usando o [Socket.Io][].</span><span class="sxs-lookup"><span data-stu-id="76594-106">Allows you to receive near-real-time change notifications for a [drive][] and [list][] using [socket.io][].</span></span>
<span data-ttu-id="76594-107">Socket.io é uma biblioteca de notificações popular para JavaScript que utiliza WebSockets.</span><span class="sxs-lookup"><span data-stu-id="76594-107">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="76594-108">Para saber mais, confira [Socket.Io](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="76594-108">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[list]: ../resources/list.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="76594-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="76594-112">Permissions</span></span>

<span data-ttu-id="76594-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76594-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76594-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76594-115">Permission type</span></span>                        | <span data-ttu-id="76594-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76594-116">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="76594-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76594-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="76594-118">Files. Read, files. ReadWrite, files. ReadWrite. All, sites. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="76594-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="76594-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76594-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76594-120">Files. Read, files. ReadWrite, files. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="76594-120">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="76594-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76594-121">Application</span></span>                            | <span data-ttu-id="76594-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76594-122">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="76594-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76594-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /lists/{list-id}/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="76594-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76594-124">Example</span></span>

### <a name="request"></a><span data-ttu-id="76594-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76594-125">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="76594-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="76594-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```msgraph-interactive
GET /me/drive/root/subscriptions/socketIo
```
# <a name="c"></a>[<span data-ttu-id="76594-127">C#</span><span class="sxs-lookup"><span data-stu-id="76594-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/drive-root-subscriptions-socketio-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76594-128">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76594-128">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/drive-root-subscriptions-socketio-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76594-129">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76594-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/drive-root-subscriptions-socketio-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="76594-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="76594-130">Response</span></span>

<span data-ttu-id="76594-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76594-131">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="76594-132">O `notificationUrl` retornado é uma URL de ponto de extremidade Socket.IO.</span><span class="sxs-lookup"><span data-stu-id="76594-132">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="76594-133">Para usá-lo com um cliente do socket.io, divida a cadeia `/callback?` de caracteres no token.</span><span class="sxs-lookup"><span data-stu-id="76594-133">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="76594-134">A parte da cadeia de caracteres `/callback?` antes é a URL de ponto de extremidade Socket.Io e a parte da cadeia de caracteres depois é uma cadeia de caracteres de consulta opaca que deve ser fornecida à biblioteca.</span><span class="sxs-lookup"><span data-stu-id="76594-134">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="76594-135">O exemplo a seguir mostra como usar o `notificationUrl` com Socket.Io em JavaScript.</span><span class="sxs-lookup"><span data-stu-id="76594-135">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
