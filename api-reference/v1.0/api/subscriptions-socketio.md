---
author: daspek
ms.author: dspektor
title: Obter ponto de extremidade do WebSocket
localization_priority: Normal
ms.prod: sharepoint
description: Permite que você receba notificações de alteração quase em tempo real para uma unidade usando o socket.io.
doc_type: apiPageType
ms.openlocfilehash: 3249bba061257b4bae715734ab4e3ba348131c63
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43109091"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="ba260-103">Obter ponto de extremidade do WebSocket</span><span class="sxs-lookup"><span data-stu-id="ba260-103">Get websocket endpoint</span></span>

<span data-ttu-id="ba260-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba260-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba260-105">Permite que você receba notificações de alteração quase em tempo real para uma [unidade][] e [lista][] usando o [Socket.Io][].</span><span class="sxs-lookup"><span data-stu-id="ba260-105">Allows you to receive near-real-time change notifications for a [drive][] and [list][] using [socket.io][].</span></span>
<span data-ttu-id="ba260-106">Socket.io é uma biblioteca de notificações popular para JavaScript que utiliza WebSockets.</span><span class="sxs-lookup"><span data-stu-id="ba260-106">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="ba260-107">Para saber mais, confira [Socket.Io](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="ba260-107">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[list]: ../resources/list.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="ba260-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba260-111">Permissions</span></span>

<span data-ttu-id="ba260-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba260-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba260-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba260-114">Permission type</span></span>                        | <span data-ttu-id="ba260-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba260-115">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="ba260-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba260-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba260-117">Files. Read, files. ReadWrite, files. ReadWrite. All, sites. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ba260-117">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="ba260-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba260-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba260-119">Files. Read, files. ReadWrite, files. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ba260-119">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="ba260-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba260-120">Application</span></span>                            | <span data-ttu-id="ba260-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba260-121">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="ba260-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba260-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /lists/{list-id}/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="ba260-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba260-123">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba260-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba260-124">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ba260-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba260-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```msgraph-interactive
GET /me/drive/root/subscriptions/socketIo
```
# <a name="c"></a>[<span data-ttu-id="ba260-126">C#</span><span class="sxs-lookup"><span data-stu-id="ba260-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/drive-root-subscriptions-socketio-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba260-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba260-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/drive-root-subscriptions-socketio-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba260-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba260-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/drive-root-subscriptions-socketio-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba260-129">Java</span><span class="sxs-lookup"><span data-stu-id="ba260-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/drive-root-subscriptions-socketio-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ba260-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba260-130">Response</span></span>

<span data-ttu-id="ba260-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba260-131">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="ba260-132">O `notificationUrl` retornado é uma URL de ponto de extremidade Socket.IO.</span><span class="sxs-lookup"><span data-stu-id="ba260-132">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>

<span data-ttu-id="ba260-133">O exemplo a seguir mostra como usar o `notificationUrl` com Socket.Io em JavaScript.</span><span class="sxs-lookup"><span data-stu-id="ba260-133">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

```javascript
// this is the notificationUrl returned from this API
var notificationUrl = "https://f3hb0mpua.svc.ms/zbaehwg/callback?snthgk=1ff3-2345672zz831837523";

// 'io' comes from the socket.io client library
var socket = io(notificationUrl);

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
