---
title: Obter chatMessage
description: Recupere uma única mensagem em um bate-papo.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 29b272769928d873c419122b092471a688a43084
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718412"
---
# <a name="get-chatmessage"></a><span data-ttu-id="2da96-103">Obter chatMessage</span><span class="sxs-lookup"><span data-stu-id="2da96-103">Get chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2da96-104">Recupere uma única [mensagem](../resources/chatmessage.md) em um [bate-papo](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="2da96-104">Retrieve a single [message](../resources/chatmessage.md) in a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2da96-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2da96-105">Permissions</span></span>

<span data-ttu-id="2da96-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2da96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2da96-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2da96-108">Permission type</span></span>      | <span data-ttu-id="2da96-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2da96-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2da96-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2da96-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2da96-111">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2da96-111">Chat.Read, Chat.ReadWrite</span></span>   |
|<span data-ttu-id="2da96-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2da96-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2da96-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2da96-113">Not supported.</span></span>    |
|<span data-ttu-id="2da96-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2da96-114">Application</span></span> | <span data-ttu-id="2da96-115">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="2da96-115">Chat.Read.All</span></span>   |

> [!NOTE]
> <span data-ttu-id="2da96-116">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2da96-116">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="2da96-117">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="2da96-117">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="2da96-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2da96-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}/messages/{id}
GET /users/{id}/chats/{id}/messages/{id}
GET /chats/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2da96-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2da96-119">Optional query parameters</span></span>

<span data-ttu-id="2da96-120">Esta operação não é atualmente compatível com [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2da96-120">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2da96-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2da96-121">Request headers</span></span>
| <span data-ttu-id="2da96-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2da96-122">Header</span></span>       | <span data-ttu-id="2da96-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2da96-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2da96-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2da96-124">Authorization</span></span>  | <span data-ttu-id="2da96-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2da96-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2da96-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2da96-127">Request body</span></span>
<span data-ttu-id="2da96-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2da96-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2da96-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2da96-129">Response</span></span>

<span data-ttu-id="2da96-130">Se bem-sucedido, esse método retornará um `200 OK` código de resposta e um objeto [chatmessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2da96-130">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2da96-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2da96-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2da96-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2da96-132">Request</span></span>
<span data-ttu-id="2da96-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2da96-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2da96-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2da96-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/chats/{id}/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2da96-135">C#</span><span class="sxs-lookup"><span data-stu-id="2da96-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2da96-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2da96-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2da96-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2da96-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2da96-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2da96-138">Response</span></span>
<span data-ttu-id="2da96-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2da96-139">Here is an example of the response.</span></span> 

><span data-ttu-id="2da96-140">**Observação:** O objeto de resposta mostrado aqui é encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2da96-140">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="2da96-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2da96-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf%40unq.gbl.spaces')/messages/$entity",
    "id": "1555631722147",
    "replyToId": null,
    "etag": "1555631722147",
    "messageType": "message",
    "createdDateTime": "2019-04-18T23:55:22.147Z",
    "lastModifiedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "device": null,
        "user": null,
        "conversation": null,
        "application": {
            "id": "877192bd-9183-47d3-a74c-8aa0426716cf",
            "displayName": "TestBot",
            "applicationIdentityType": "bot"
        }
    },
    "body": {
        "contentType": "html",
        "content": "<attachment id=\"bcb243ec589a4537b3c650356421e696\"></attachment>"
    },
    "attachments": [
        {
            "id": "bcb243ec589a4537b3c650356421e696",
            "contentType": "application/vnd.microsoft.card.signin",
            "contentUrl": null,
            "content": "{\r\n  \"text\": \"Please sign in to sample to proceed.\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"signin\",\r\n      \"title\": \"Sign In\",\r\n      \"value\": \"https://token.botframework.com/api/oauth/signin?signin=921d46120f7695632ce6ca4b0da2e3ae15fea54c47\"\r\n    }\r\n  ]\r\n}",
            "name": null,
            "thumbnailUrl": null
        }
    ],
    "mentions": [],
    "reactions": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
