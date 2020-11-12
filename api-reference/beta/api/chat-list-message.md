---
title: Listar mensagens de bate-papo
description: 'Recupere a lista de mensagens em um bate-papo. '
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 03bf5aeb24aab47b51bd0a5f468df29044347f63
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000508"
---
# <a name="list-chat-messages"></a><span data-ttu-id="9e7b7-103">Listar mensagens de bate-papo</span><span class="sxs-lookup"><span data-stu-id="9e7b7-103">List chat messages</span></span>

<span data-ttu-id="9e7b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e7b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e7b7-105">Recupere a lista de [mensagens](../resources/chatmessage.md) em um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="9e7b7-105">Retrieve the list of [messages](../resources/chatmessage.md) in a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="9e7b7-106">**Observação** : Esta API oferece suporte à inscrição para alterações (criar, atualizar e excluir) usando [notificações de alteração](../resources/webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="9e7b7-106">**Note** : This API supports subscribing to changes (create, update, and delete) using [change notifications](../resources/webhooks.md).</span></span> <span data-ttu-id="9e7b7-107">Isso permite aos chamadores assinar e obter alterações em tempo real.</span><span class="sxs-lookup"><span data-stu-id="9e7b7-107">This allows callers to subscribe and get changes in real time.</span></span> <span data-ttu-id="9e7b7-108">Para obter detalhes, confira [obter notificações de](/graph/teams-changenotifications-chatmessage)de mensagens.</span><span class="sxs-lookup"><span data-stu-id="9e7b7-108">For details, see [Get notifications for messages](/graph/teams-changenotifications-chatmessage).</span></span>

## <a name="permissions"></a><span data-ttu-id="9e7b7-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="9e7b7-109">Permissions</span></span>

<span data-ttu-id="9e7b7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e7b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e7b7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e7b7-112">Permission type</span></span>      | <span data-ttu-id="9e7b7-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e7b7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e7b7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e7b7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9e7b7-115">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9e7b7-115">Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="9e7b7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e7b7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e7b7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e7b7-117">Not supported.</span></span>    |
|<span data-ttu-id="9e7b7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e7b7-118">Application</span></span> | <span data-ttu-id="9e7b7-119">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e7b7-119">Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="9e7b7-120">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e7b7-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="9e7b7-121">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="9e7b7-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="9e7b7-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e7b7-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}/messages
GET /users/{id}/chats/{id}/messages
GET /chats/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e7b7-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9e7b7-123">Optional query parameters</span></span>

<span data-ttu-id="9e7b7-124">Esta operação não é atualmente compatível com [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9e7b7-124">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e7b7-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e7b7-125">Request headers</span></span>

| <span data-ttu-id="9e7b7-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e7b7-126">Header</span></span>       | <span data-ttu-id="9e7b7-127">Valor</span><span class="sxs-lookup"><span data-stu-id="9e7b7-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9e7b7-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e7b7-128">Authorization</span></span>  | <span data-ttu-id="9e7b7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e7b7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9e7b7-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e7b7-131">Request body</span></span>

<span data-ttu-id="9e7b7-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e7b7-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e7b7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e7b7-133">Response</span></span>

<span data-ttu-id="9e7b7-134">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatMessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e7b7-134">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e7b7-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e7b7-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e7b7-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e7b7-136">Request</span></span>

<span data-ttu-id="9e7b7-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e7b7-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e7b7-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e7b7-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages
```
# <a name="c"></a>[<span data-ttu-id="9e7b7-139">C#</span><span class="sxs-lookup"><span data-stu-id="9e7b7-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e7b7-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e7b7-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e7b7-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e7b7-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9e7b7-142">Java</span><span class="sxs-lookup"><span data-stu-id="9e7b7-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chat-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9e7b7-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e7b7-143">Response</span></span>
<span data-ttu-id="9e7b7-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e7b7-144">Here is an example of the response.</span></span> 

><span data-ttu-id="9e7b7-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e7b7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf%40unq.gbl.spaces')/messages",
    "@odata.count": 4,
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces/messages?$skiptoken=M2Y1YjAwMDAwMDMxMzkzYTM4NjIzMDM4MzE2NTY2MzYyZDM0MzczOTMyMmQzNDY0NjU2NjJkNjIzMjYzMzkyZDYzMzMzNjMzNjEzMTYyNjYzNDMxNjQzNTVmMzgzNzM3MzEzOTMyNjI2NDJkMzkzMTM4MzMyZDM0Mzc2NDMzMmQ2MTM3MzQ2MzJkMzg2MTYxMzAzNDMyMzYzNzMxMzY2MzY2NDA3NTZlNzEyZTY3NjI2YzJlNzM3MDYxNjM2NTczMDE5N2Y3ZGMzMjZhMDEwMDAwMDg1YjNmNGI2YTAxMDAwMDAwfDE1NTU2MzE3MjIxNDc%3d",
    "value": [
        {
            "id": "1555631722147",
            "replyToId": null,
            "etag": "1555631722147",
            "messageType": "message",
            "createdDateTime": "2019-04-18T23:55:22.147Z",
            "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
            "lastEditedDateTime": null,
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
                "content": "<attachment id=\"a7bda643d32b4541b74ec1f4ace7f391\"></attachment>"
            },
            "attachments": [
                {
                    "id": "a7bda643d32b4541b74ec1f4ace7f391",
                    "contentType": "application/vnd.microsoft.card.signin",
                    "contentUrl": null,
                    "content": "{\r\n  \"text\": \"Please sign in to sample to proceed.\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"signin\",\r\n      \"title\": \"Sign In\",\r\n      \"value\": \"https://token.botframework.com/api/oauth/signin?signin=921d46120f7695632ce6ca4b0da2e3ae15fea54c47\"\r\n    }\r\n  ]\r\n}",
                    "name": null,
                    "thumbnailUrl": null
                }
            ],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1555631540287",
            "replyToId": null,
            "etag": "1555631540287",
            "messageType": "message",
            "createdDateTime": "2019-04-18T23:52:20.287Z",
            "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
            "summary": null,
            "importance": "normal",
            "locale": "en-us",
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
                    "displayName": "MOD Administrator",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "yo"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1555631512068",
            "replyToId": null,
            "etag": "1555631512068",
            "messageType": "message",
            "createdDateTime": "2019-04-18T23:51:52.068Z",
            "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
            "lastEditedDateTime": null,
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
                "content": "<attachment id=\"6309ad5424a04c5899efd130342b165a\"></attachment>"
            },
            "attachments": [
                {
                    "id": "6309ad5424a04c5899efd130342b165a",
                    "contentType": "application/vnd.microsoft.card.signin",
                    "contentUrl": null,
                    "content": "{\r\n  \"text\": \"Please sign in to sample to proceed.\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"signin\",\r\n      \"title\": \"Sign In\",\r\n      \"value\": \"https://token.botframework.com/api/oauth/signin?signin=921d46120f978574f2993640bf9cbc5e438824a645\"\r\n    }\r\n  ]\r\n}",
                    "name": null,
                    "thumbnailUrl": null
                }
            ],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1555631511115",
            "replyToId": null,
            "etag": "1555631511115",
            "messageType": "message",
            "createdDateTime": "2019-04-18T23:51:51.115Z",
            "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
            "lastEditedDateTime": null,
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
                "content": "<attachment id=\"9b6e6d3bde7741bcac561bb15ec2721b\"></attachment>"
            },
            "attachments": [
                {
                    "id": "9b6e6d3bde7741bcac561bb15ec2721b",
                    "contentType": "application/vnd.microsoft.card.signin",
                    "contentUrl": null,
                    "content": "{\r\n  \"text\": \"Please sign in to sample to proceed.\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"signin\",\r\n      \"title\": \"Sign In\",\r\n      \"value\": \"https://token.botframework.com/api/oauth/signin?signin=921d46120f01039912d88040739e2780ef54656557\"\r\n    }\r\n  ]\r\n}",
                    "name": null,
                    "thumbnailUrl": null
                }
            ],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chat messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

