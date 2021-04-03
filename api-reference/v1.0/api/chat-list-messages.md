---
title: Listar mensagens em um chat
description: 'Recuperar a lista de mensagens em um chat. '
localization_priority: Priority
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 39464badbf5c00a6d87a5a97877334cd657b56f2
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582876"
---
# <a name="list-messages-in-a-chat"></a><span data-ttu-id="bde9c-103">Listar mensagens em um chat</span><span class="sxs-lookup"><span data-stu-id="bde9c-103">List messages in a chat</span></span>

<span data-ttu-id="bde9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bde9c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bde9c-105">Recupere a lista de [mensagens](../resources/chatmessage.md) em um [bate-papo](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="bde9c-105">Retrieve the list of [messages](../resources/chatmessage.md) in a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="bde9c-106">**Observação**: Esta API oferece suporte à inscrição para alterações (criar, atualizar e excluir) usando [notificações de alteração](../resources/webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="bde9c-106">**Note**: This API supports subscribing to changes (create, update, and delete) using [change notifications](../resources/webhooks.md).</span></span> <span data-ttu-id="bde9c-107">Isso permite aos chamadores assinar e obter alterações em tempo real.</span><span class="sxs-lookup"><span data-stu-id="bde9c-107">This allows callers to subscribe and get changes in real time.</span></span> <span data-ttu-id="bde9c-108">Para obter detalhes, confira [obter notificações de](/graph/teams-changenotifications-chatmessage)de mensagens.</span><span class="sxs-lookup"><span data-stu-id="bde9c-108">For details, see [Get notifications for messages](/graph/teams-changenotifications-chatmessage).</span></span>

## <a name="permissions"></a><span data-ttu-id="bde9c-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="bde9c-109">Permissions</span></span>

<span data-ttu-id="bde9c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bde9c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bde9c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bde9c-112">Permission type</span></span>      | <span data-ttu-id="bde9c-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bde9c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bde9c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bde9c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bde9c-115">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bde9c-115">Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="bde9c-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bde9c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bde9c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bde9c-117">Not supported.</span></span>    |
|<span data-ttu-id="bde9c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bde9c-118">Application</span></span> | <span data-ttu-id="bde9c-119">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bde9c-119">Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="bde9c-120">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bde9c-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="bde9c-121">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="bde9c-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="bde9c-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bde9c-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{chat-id}/messages
GET /users/{user-id}/chats/{chat-id}/messages
GET /chats/{chat-id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bde9c-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bde9c-123">Optional query parameters</span></span>

<span data-ttu-id="bde9c-124">Você pode usar o parâmetro de consulta [$top](/graph/query-parameters#top-parameter) para controlar o número de itens por resposta.</span><span class="sxs-lookup"><span data-stu-id="bde9c-124">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="bde9c-125">O valor `$top` máximo permitido é 50.</span><span class="sxs-lookup"><span data-stu-id="bde9c-125">Maximum allowed `$top` value is 50.</span></span>
<span data-ttu-id="bde9c-126">No momento, não há suporte para os outros [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bde9c-126">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bde9c-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bde9c-127">Request headers</span></span>

| <span data-ttu-id="bde9c-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bde9c-128">Header</span></span>       | <span data-ttu-id="bde9c-129">Valor</span><span class="sxs-lookup"><span data-stu-id="bde9c-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bde9c-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="bde9c-130">Authorization</span></span>  | <span data-ttu-id="bde9c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bde9c-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bde9c-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bde9c-133">Request body</span></span>

<span data-ttu-id="bde9c-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bde9c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bde9c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="bde9c-135">Response</span></span>

<span data-ttu-id="bde9c-136">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatMessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bde9c-136">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bde9c-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bde9c-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="bde9c-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bde9c-138">Request</span></span>

<span data-ttu-id="bde9c-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bde9c-139">The following is an example of the request.</span></span> <span data-ttu-id="bde9c-140">`$top=2` é passado para recuperar duas mensagens.</span><span class="sxs-lookup"><span data-stu-id="bde9c-140">`$top=2` is passed to retrieve two messages.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_allchatmessages_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages?$top=2
```

### <a name="response"></a><span data-ttu-id="bde9c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="bde9c-141">Response</span></span>
<span data-ttu-id="bde9c-142">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="bde9c-142">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages",
    "@odata.count": 2,
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages?$top=2&$skiptoken=M2UyZDAwMDAwMDMxMzkzYTMyNjQ2MTM0NjMzMjM5NjYzNjY0MzczMDM0MzE2NTYzNjEzNzMwNjIzNjMzMzg2MjM0MzM2NDM0MzUzNDMzMzc0MDc0Njg3MjY1NjE2NDJlNzYzMjAxZThmYjY4M2Y3ODAxMDAwMDg4NjA5ODdhNzgwMTAwMDB8MTYxNjk2NDUwOTgzMg%3d%3d",
    "value": [
        {
            "id": "1616964509832",
            "replyToId": null,
            "etag": "1616964509832",
            "messageType": "message",
            "createdDateTime": "2021-03-28T20:48:29.832Z",
            "lastModifiedDateTime": "2021-03-28T20:48:29.832Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
            "importance": "normal",
            "locale": "en-us",
            "webUrl": null,
            "channelIdentity": null,
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Hello world"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1615971548136",
            "replyToId": null,
            "etag": "1615971548136",
            "messageType": "message",
            "createdDateTime": "2021-03-17T08:59:08.136Z",
            "lastModifiedDateTime": "2021-03-17T08:59:08.136Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
            "importance": "normal",
            "locale": "en-us",
            "webUrl": null,
            "channelIdentity": null,
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div><div><div><span><img height=\"63\" src=\"https://graph.microsoft.com/v1.0/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents/aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv/$value\" width=\"67\" style=\"vertical-align:bottom; width:67px; height:63px\"></span></div></div></div>"
            },
            "attachments": [],
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

