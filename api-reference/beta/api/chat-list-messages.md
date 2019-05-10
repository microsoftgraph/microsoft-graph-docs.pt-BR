---
title: Listar mensagens de bate-papo
description: 'Recupere a lista de mensagens em um bate-papo. '
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 85c8aa1a01ba4a9446ed6c1c5349fae3a66e77c1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591604"
---
# <a name="list-chat-messages"></a><span data-ttu-id="455a7-103">Listar mensagens de bate-papo</span><span class="sxs-lookup"><span data-stu-id="455a7-103">List chat messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="455a7-104">Recupere a lista de [mensagens](../resources/chatmessage.md) em um [bate-papo](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="455a7-104">Retrieve the list of [messages](../resources/chatmessage.md) in a [chat](../resources/chat.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="455a7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="455a7-105">Permissions</span></span>

<span data-ttu-id="455a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="455a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="455a7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="455a7-108">Permission type</span></span>      | <span data-ttu-id="455a7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="455a7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="455a7-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="455a7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="455a7-111">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="455a7-111">Chat.Read</span></span>   |
|<span data-ttu-id="455a7-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="455a7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="455a7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="455a7-113">Not supported.</span></span>    |
|<span data-ttu-id="455a7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="455a7-114">Application</span></span> | <span data-ttu-id="455a7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="455a7-115">Not supported.</span></span>   |

## <a name="http-request"></a><span data-ttu-id="455a7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="455a7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}/messages
GET /users/{id}/chats/{id}/messages
GET /chats/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="455a7-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="455a7-117">Optional query parameters</span></span>

<span data-ttu-id="455a7-118">Esta operação não é atualmente compatível com [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="455a7-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="455a7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="455a7-119">Request headers</span></span>

| <span data-ttu-id="455a7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="455a7-120">Header</span></span>       | <span data-ttu-id="455a7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="455a7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="455a7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="455a7-122">Authorization</span></span>  | <span data-ttu-id="455a7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="455a7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="455a7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="455a7-125">Request body</span></span>

<span data-ttu-id="455a7-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="455a7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="455a7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="455a7-127">Response</span></span>

<span data-ttu-id="455a7-128">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatMessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="455a7-128">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="455a7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="455a7-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="455a7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="455a7-130">Request</span></span>

<span data-ttu-id="455a7-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="455a7-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chat_messages"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="455a7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="455a7-132">Response</span></span>
<span data-ttu-id="455a7-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="455a7-133">Here is an example of the response.</span></span> 

><span data-ttu-id="455a7-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="455a7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "lastModifiedDateTime": null,
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="455a7-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="455a7-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="455a7-137">C#</span><span class="sxs-lookup"><span data-stu-id="455a7-137">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_chat_messages-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="455a7-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="455a7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_chat_messages-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/chat-list-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chat-list-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
