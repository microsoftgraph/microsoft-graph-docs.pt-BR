---
title: Obter ponto de extremidade do WebSocket
description: Não há suporte para o uso dessas APIs em aplicativos de produção.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: ''
ms.openlocfilehash: 6b2036d8d49cd13c15bf0c481aee0795306e0809
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324410"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="ca16c-103">Obter ponto de extremidade do WebSocket</span><span class="sxs-lookup"><span data-stu-id="ca16c-103">Get websocket endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="ca16c-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ca16c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca16c-105">Permite que você receba notificações de alteração quase em tempo real para uma [unidade][] usando o [Socket.Io][].</span><span class="sxs-lookup"><span data-stu-id="ca16c-105">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="ca16c-106">Socket.io é uma biblioteca de notificações popular para JavaScript que utiliza WebSockets.</span><span class="sxs-lookup"><span data-stu-id="ca16c-106">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="ca16c-107">Para saber mais, confira [Socket.Io](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="ca16c-107">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="ca16c-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca16c-110">Permissions</span></span>

<span data-ttu-id="ca16c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca16c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca16c-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca16c-113">Permission type</span></span>                        | <span data-ttu-id="ca16c-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca16c-114">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="ca16c-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca16c-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca16c-116">Files. Read, files. ReadWrite, files. ReadWrite. All, sites. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ca16c-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="ca16c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca16c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca16c-118">Files. Read, files. ReadWrite, files. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ca16c-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="ca16c-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca16c-119">Application</span></span>                            | <span data-ttu-id="ca16c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca16c-120">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="ca16c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca16c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="ca16c-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca16c-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca16c-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca16c-123">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ca16c-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca16c-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ca16c-125">C#</span><span class="sxs-lookup"><span data-stu-id="ca16c-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/drive-root-subscriptions-socketio-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ca16c-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca16c-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/drive-root-subscriptions-socketio-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ca16c-127">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ca16c-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/drive-root-subscriptions-socketio-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ca16c-128">Java</span><span class="sxs-lookup"><span data-stu-id="ca16c-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/drive-root-subscriptions-socketio-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ca16c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca16c-129">Response</span></span>

<span data-ttu-id="ca16c-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca16c-130">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="ca16c-131">O `notificationUrl` retornado é uma URL de ponto de extremidade Socket.IO.</span><span class="sxs-lookup"><span data-stu-id="ca16c-131">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="ca16c-132">Para usá-lo com um cliente do socket.io, divida a cadeia `/callback?` de caracteres no token.</span><span class="sxs-lookup"><span data-stu-id="ca16c-132">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="ca16c-133">A parte da cadeia de caracteres `/callback?` antes é a URL de ponto de extremidade Socket.Io e a parte da cadeia de caracteres depois é uma cadeia de caracteres de consulta opaca que deve ser fornecida à biblioteca.</span><span class="sxs-lookup"><span data-stu-id="ca16c-133">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="ca16c-134">O exemplo a seguir mostra como usar o `notificationUrl` com Socket.Io em JavaScript.</span><span class="sxs-lookup"><span data-stu-id="ca16c-134">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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
