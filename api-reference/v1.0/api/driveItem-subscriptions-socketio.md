---
author: daspek
ms.author: dspektor
title: Obter ponto de extremidade do WebSocket
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4d4577ea69c65d6ce003af96b0d96b55fe178fb5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562752"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="f2ddf-102">Obter ponto de extremidade do WebSocket</span><span class="sxs-lookup"><span data-stu-id="f2ddf-102">Get websocket endpoint</span></span>

<span data-ttu-id="f2ddf-103">Permite que você receba notificações de alteração quase em tempo real para uma [unidade][] usando o [Socket.Io][].</span><span class="sxs-lookup"><span data-stu-id="f2ddf-103">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="f2ddf-104">Socket.io é uma biblioteca de notificações popular para JavaScript que utiliza webSockets.</span><span class="sxs-lookup"><span data-stu-id="f2ddf-104">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="f2ddf-105">Para saber mais, confira [Socket.Io](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="f2ddf-105">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[Socket.Io]: https://socket.io/
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="f2ddf-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2ddf-108">Permissions</span></span>

<span data-ttu-id="f2ddf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2ddf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2ddf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2ddf-111">Permission type</span></span>                        | <span data-ttu-id="f2ddf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2ddf-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="f2ddf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2ddf-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2ddf-114">Files. Read, files. ReadWrite, files. ReadWrite. All, sites. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f2ddf-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="f2ddf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2ddf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2ddf-116">Files. Read, files. ReadWrite, files. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f2ddf-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="f2ddf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2ddf-117">Application</span></span>                            | <span data-ttu-id="f2ddf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2ddf-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="f2ddf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2ddf-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="f2ddf-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2ddf-120">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2ddf-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2ddf-121">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="f2ddf-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2ddf-122">Response</span></span>

<span data-ttu-id="f2ddf-123">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2ddf-123">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="f2ddf-124">O `notificationUrl` retornado é uma URL de ponto de extremidade Socket.IO.</span><span class="sxs-lookup"><span data-stu-id="f2ddf-124">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="f2ddf-125">Para usá-lo com um cliente do socket.io, divida a cadeia `/callback?` de caracteres no token.</span><span class="sxs-lookup"><span data-stu-id="f2ddf-125">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="f2ddf-126">A parte da cadeia de caracteres `/callback?` antes é a URL de ponto de extremidade Socket.Io e a parte da cadeia de caracteres depois é uma cadeia de caracteres de consulta opaca que deve ser fornecida à biblioteca.</span><span class="sxs-lookup"><span data-stu-id="f2ddf-126">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="f2ddf-127">O exemplo a seguir mostra como usar o `notificationUrl` com Socket.Io em JavaScript.</span><span class="sxs-lookup"><span data-stu-id="f2ddf-127">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveItem-subscriptions-socketio.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
