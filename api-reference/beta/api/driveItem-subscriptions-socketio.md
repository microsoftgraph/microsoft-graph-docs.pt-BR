---
title: Obtenha o ponto de extremidade do websocket
description: Não há suporte para o uso dessas APIs em aplicativos de produção.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 736684812d2cbc10affed82a3f946d75731f6768
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519791"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="b8956-103">Obtenha o ponto de extremidade do websocket</span><span class="sxs-lookup"><span data-stu-id="b8956-103">Get websocket endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="b8956-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b8956-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8956-105">Permite que você receber notificações de alteração de quase em tempo real para uma [unidade][] usando o [socket.io][].</span><span class="sxs-lookup"><span data-stu-id="b8956-105">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="b8956-106">Socket.IO é uma biblioteca de notificações populares para JavaScript que utiliza o WebSocket.</span><span class="sxs-lookup"><span data-stu-id="b8956-106">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="b8956-107">Para saber mais, consulte [socket.io](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="b8956-107">To learn more, see [socket.io](https://socket.io).</span></span>

[unidade]: ../resources/drive.md
[drive]: ../resources/drive.md
[Socket.IO]: https://socket.io/
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="b8956-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8956-110">Permissions</span></span>

<span data-ttu-id="b8956-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8956-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8956-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8956-113">Permission type</span></span>                        | <span data-ttu-id="b8956-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8956-114">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="b8956-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8956-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8956-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8956-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="b8956-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8956-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8956-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8956-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="b8956-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8956-119">Application</span></span>                            | <span data-ttu-id="b8956-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8956-120">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="b8956-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8956-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="b8956-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8956-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8956-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8956-123">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="b8956-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8956-124">Response</span></span>

<span data-ttu-id="b8956-125">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [inscrição](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8956-125">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="b8956-126">O `notificationUrl` retornado é uma URL de ponto de extremidade socket.io.</span><span class="sxs-lookup"><span data-stu-id="b8956-126">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="b8956-127">Para usá-la com um cliente socket.io, dividir a cadeia de caracteres no `/callback?` token.</span><span class="sxs-lookup"><span data-stu-id="b8956-127">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="b8956-128">A parte da cadeia de caracteres antes `/callback?` é a URL do ponto de extremidade de socket.io e a parte da cadeia de caracteres após é uma sequência de caracteres de consulta opaco que deve ser fornecida para a biblioteca.</span><span class="sxs-lookup"><span data-stu-id="b8956-128">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="b8956-129">O exemplo a seguir mostra como usar o `notificationUrl` com socket.io em JavaScript.</span><span class="sxs-lookup"><span data-stu-id="b8956-129">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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
