---
author: daspek
ms.author: dspektor
title: Obter ponto de extremidade do WebSocket
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f14f13d3c84d3f352d03ea5533649614367b7e48
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276990"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="d94f5-102">Obter ponto de extremidade do WebSocket</span><span class="sxs-lookup"><span data-stu-id="d94f5-102">Get websocket endpoint</span></span>

<span data-ttu-id="d94f5-103">Permite que você receba notificações de alteração quase em tempo real para uma [unidade][] usando o [Socket.Io][].</span><span class="sxs-lookup"><span data-stu-id="d94f5-103">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="d94f5-104">Socket.io é uma biblioteca de notificações popular para JavaScript que utiliza WebSockets.</span><span class="sxs-lookup"><span data-stu-id="d94f5-104">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="d94f5-105">Para saber mais, confira [Socket.Io](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="d94f5-105">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="d94f5-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d94f5-108">Permissions</span></span>

<span data-ttu-id="d94f5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d94f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d94f5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d94f5-111">Permission type</span></span>                        | <span data-ttu-id="d94f5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d94f5-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="d94f5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d94f5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d94f5-114">Files. Read, files. ReadWrite, files. ReadWrite. All, sites. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d94f5-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="d94f5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d94f5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d94f5-116">Files. Read, files. ReadWrite, files. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d94f5-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="d94f5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d94f5-117">Application</span></span>                            | <span data-ttu-id="d94f5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d94f5-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="d94f5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d94f5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="d94f5-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d94f5-120">Example</span></span>

### <a name="request"></a><span data-ttu-id="d94f5-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d94f5-121">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="d94f5-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="d94f5-122">Response</span></span>

<span data-ttu-id="d94f5-123">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d94f5-123">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d94f5-124">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d94f5-124">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d94f5-125">C#</span><span class="sxs-lookup"><span data-stu-id="d94f5-125">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/drive_root_subscriptions_socketIo-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d94f5-126">Javascript</span><span class="sxs-lookup"><span data-stu-id="d94f5-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/drive_root_subscriptions_socketIo-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d94f5-127">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d94f5-127">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/drive_root_subscriptions_socketIo-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="d94f5-128">O `notificationUrl` retornado é uma URL de ponto de extremidade Socket.IO.</span><span class="sxs-lookup"><span data-stu-id="d94f5-128">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="d94f5-129">Para usá-lo com um cliente do socket.io, divida a cadeia `/callback?` de caracteres no token.</span><span class="sxs-lookup"><span data-stu-id="d94f5-129">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="d94f5-130">A parte da cadeia de caracteres `/callback?` antes é a URL de ponto de extremidade Socket.Io e a parte da cadeia de caracteres depois é uma cadeia de caracteres de consulta opaca que deve ser fornecida à biblioteca.</span><span class="sxs-lookup"><span data-stu-id="d94f5-130">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="d94f5-131">O exemplo a seguir mostra como usar o `notificationUrl` com Socket.Io em JavaScript.</span><span class="sxs-lookup"><span data-stu-id="d94f5-131">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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
    "Error: /api-reference/v1.0/api/driveItem-subscriptions-socketio.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/driveItem-subscriptions-socketio.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveItem-subscriptions-socketio.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
