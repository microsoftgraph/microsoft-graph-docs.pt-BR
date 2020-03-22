---
author: daspek
ms.author: dspektor
title: Obter ponto de extremidade do WebSocket
localization_priority: Normal
ms.prod: sharepoint
description: Permite que você receba notificações de alteração quase em tempo real para uma unidade usando o socket.io.
doc_type: apiPageType
ms.openlocfilehash: ca15c21ecd08b2a74700d2b729e23632e427a72f
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892650"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="946b7-103">Obter ponto de extremidade do WebSocket</span><span class="sxs-lookup"><span data-stu-id="946b7-103">Get websocket endpoint</span></span>

<span data-ttu-id="946b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="946b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="946b7-105">Permite que você receba notificações de alteração quase em tempo real para uma [unidade][] usando o [Socket.Io][].</span><span class="sxs-lookup"><span data-stu-id="946b7-105">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="946b7-106">Socket.io é uma biblioteca de notificações popular para JavaScript que utiliza WebSockets.</span><span class="sxs-lookup"><span data-stu-id="946b7-106">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="946b7-107">Para saber mais, confira [Socket.Io](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="946b7-107">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="946b7-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="946b7-110">Permissions</span></span>

<span data-ttu-id="946b7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="946b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="946b7-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="946b7-113">Permission type</span></span>                        | <span data-ttu-id="946b7-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="946b7-114">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="946b7-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="946b7-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="946b7-116">Files. Read, files. ReadWrite, files. ReadWrite. All, sites. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="946b7-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="946b7-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="946b7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="946b7-118">Files. Read, files. ReadWrite, files. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="946b7-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="946b7-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="946b7-119">Application</span></span>                            | <span data-ttu-id="946b7-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="946b7-120">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="946b7-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="946b7-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="946b7-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="946b7-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="946b7-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="946b7-123">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="946b7-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="946b7-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```msgraph-interactive
GET /me/drive/root/subscriptions/socketIo
```
# <a name="c"></a>[<span data-ttu-id="946b7-125">C#</span><span class="sxs-lookup"><span data-stu-id="946b7-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/drive-root-subscriptions-socketio-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="946b7-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="946b7-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/drive-root-subscriptions-socketio-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="946b7-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="946b7-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/drive-root-subscriptions-socketio-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="946b7-128">Java</span><span class="sxs-lookup"><span data-stu-id="946b7-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/drive-root-subscriptions-socketio-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="946b7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="946b7-129">Response</span></span>

<span data-ttu-id="946b7-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="946b7-130">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="946b7-131">O `notificationUrl` retornado é uma URL de ponto de extremidade Socket.IO.</span><span class="sxs-lookup"><span data-stu-id="946b7-131">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>

<span data-ttu-id="946b7-132">O exemplo a seguir mostra como usar o `notificationUrl` com Socket.Io em JavaScript.</span><span class="sxs-lookup"><span data-stu-id="946b7-132">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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
