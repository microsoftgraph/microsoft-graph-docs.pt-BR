---
author: learafa
title: Obter ponto de extremidade do websocket
description: Não há suporte para o uso dessas APIs em aplicativos de produção.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e56a4174808a7b30ecf063c2b782e0be272c6046
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721453"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="9a4b3-103">Obter ponto de extremidade do websocket</span><span class="sxs-lookup"><span data-stu-id="9a4b3-103">Get websocket endpoint</span></span>

<span data-ttu-id="9a4b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a4b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="9a4b3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9a4b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a4b3-106">Permite que você receba notificações de alteração quase em tempo real para uma [unidade][] e [uma lista][] usando [socket.io][].</span><span class="sxs-lookup"><span data-stu-id="9a4b3-106">Allows you to receive near-real-time change notifications for a [drive][] and [list][] using [socket.io][].</span></span>
<span data-ttu-id="9a4b3-107">Socket.io é uma biblioteca de notificações popular para JavaScript que utiliza WebSockets.</span><span class="sxs-lookup"><span data-stu-id="9a4b3-107">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="9a4b3-108">Para saber mais, confira [socket.io](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="9a4b3-108">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[list]: ../resources/list.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="9a4b3-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a4b3-112">Permissions</span></span>

<span data-ttu-id="9a4b3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a4b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a4b3-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a4b3-115">Permission type</span></span>                        | <span data-ttu-id="9a4b3-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a4b3-116">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="9a4b3-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a4b3-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a4b3-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a4b3-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="9a4b3-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a4b3-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a4b3-120">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a4b3-120">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="9a4b3-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a4b3-121">Application</span></span>                            | <span data-ttu-id="9a4b3-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a4b3-122">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="9a4b3-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a4b3-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /drives/{driveId}/list/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="9a4b3-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a4b3-124">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a4b3-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a4b3-125">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9a4b3-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a4b3-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```msgraph-interactive
GET /me/drive/root/subscriptions/socketIo
```
# <a name="c"></a>[<span data-ttu-id="9a4b3-127">C#</span><span class="sxs-lookup"><span data-stu-id="9a4b3-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/drive-root-subscriptions-socketio-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a4b3-128">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a4b3-128">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/drive-root-subscriptions-socketio-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a4b3-129">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a4b3-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/drive-root-subscriptions-socketio-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a4b3-130">Java</span><span class="sxs-lookup"><span data-stu-id="9a4b3-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/drive-root-subscriptions-socketio-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9a4b3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a4b3-131">Response</span></span>

<span data-ttu-id="9a4b3-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a4b3-132">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="9a4b3-133">O `notificationUrl` retornado é uma URL socket.io ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="9a4b3-133">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="9a4b3-134">Para usá-lo com um socket.io cliente, divida a cadeia de caracteres no `/callback?` token.</span><span class="sxs-lookup"><span data-stu-id="9a4b3-134">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="9a4b3-135">A parte da cadeia de caracteres antes é socket.io URL do ponto de extremidade e a parte da cadeia de caracteres depois é uma cadeia de caracteres de consulta opaca que deve ser dada `/callback?` à biblioteca.</span><span class="sxs-lookup"><span data-stu-id="9a4b3-135">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="9a4b3-136">O exemplo a seguir mostra como usar o com socket.io `notificationUrl` em JavaScript.</span><span class="sxs-lookup"><span data-stu-id="9a4b3-136">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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


