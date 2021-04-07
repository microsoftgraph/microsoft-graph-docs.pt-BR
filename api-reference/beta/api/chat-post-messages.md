---
title: Enviar mensagem em um chat
description: Envie uma nova mensagem em um chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 79df3a5e6d6aae74cc0f9d19cdd2abb2003c8f46
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610656"
---
# <a name="send-message-in-a-chat"></a><span data-ttu-id="3eabf-103">Enviar mensagem em um chat</span><span class="sxs-lookup"><span data-stu-id="3eabf-103">Send message in a chat</span></span>

<span data-ttu-id="3eabf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3eabf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3eabf-105">Envie um [novo chatMessage](../resources/chatmessage.md) no chat [especificado](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="3eabf-105">Send a new [chatMessage](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="3eabf-106">Essa API não pode criar um novo chat; você deve usar o [método de chats de](chat-list.md) lista para recuperar a ID de um chat existente antes de criar uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="3eabf-106">This API cannot create a new chat; you must use the [list chats](chat-list.md) method to retrieve the ID of an existing chat before creating a chat message.</span></span>

> <span data-ttu-id="3eabf-107">**Observação**: não recomendamos que você use essa API para migração de dados.</span><span class="sxs-lookup"><span data-stu-id="3eabf-107">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="3eabf-108">Ele não tem a produtividade necessária para uma migração típica.</span><span class="sxs-lookup"><span data-stu-id="3eabf-108">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="3eabf-109">**Observação**: é uma violação dos termos [de](/legal/microsoft-apis/terms-of-use) uso usar o Microsoft Teams como um arquivo de log.</span><span class="sxs-lookup"><span data-stu-id="3eabf-109">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="3eabf-110">Envie apenas mensagens que as pessoas lerão.</span><span class="sxs-lookup"><span data-stu-id="3eabf-110">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="3eabf-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="3eabf-111">Permissions</span></span>

<span data-ttu-id="3eabf-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eabf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3eabf-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3eabf-114">Permission type</span></span>                        | <span data-ttu-id="3eabf-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3eabf-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3eabf-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3eabf-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="3eabf-117">ChatMessage.Send, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3eabf-117">ChatMessage.Send, Chat.ReadWrite</span></span> |
| <span data-ttu-id="3eabf-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3eabf-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3eabf-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3eabf-119">Not supported.</span></span> |
| <span data-ttu-id="3eabf-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3eabf-120">Application</span></span>                            | <span data-ttu-id="3eabf-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3eabf-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3eabf-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3eabf-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{chat-id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="3eabf-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3eabf-123">Request headers</span></span>

| <span data-ttu-id="3eabf-124">Nome</span><span class="sxs-lookup"><span data-stu-id="3eabf-124">Name</span></span>          | <span data-ttu-id="3eabf-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3eabf-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3eabf-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="3eabf-126">Authorization</span></span> | <span data-ttu-id="3eabf-127">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="3eabf-127">Bearer {code}.</span></span> <span data-ttu-id="3eabf-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3eabf-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3eabf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3eabf-129">Request body</span></span>

<span data-ttu-id="3eabf-130">No corpo da solicitação, fornece uma representação JSON de um [objeto chatMessage.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="3eabf-130">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3eabf-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3eabf-131">Response</span></span>

<span data-ttu-id="3eabf-132">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto chatMessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3eabf-132">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3eabf-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3eabf-133">Examples</span></span>

<span data-ttu-id="3eabf-134">Para obter uma lista mais abrangente de exemplos, consulte [Create chatMessage in a channel or a chat](chatmessage-post.md).</span><span class="sxs-lookup"><span data-stu-id="3eabf-134">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="3eabf-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3eabf-135">Request</span></span>

<span data-ttu-id="3eabf-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3eabf-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3eabf-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="3eabf-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_chatmessages_1"
}-->
```http
POST https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages
Content-type: application/json

{
  "body": {
     "content": "Hello world"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="3eabf-138">C#</span><span class="sxs-lookup"><span data-stu-id="3eabf-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-chatmessages-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3eabf-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3eabf-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-chatmessages-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3eabf-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3eabf-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-chatmessages-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3eabf-141">Java</span><span class="sxs-lookup"><span data-stu-id="3eabf-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-chatmessages-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3eabf-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3eabf-142">Response</span></span>

<span data-ttu-id="3eabf-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3eabf-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages/$entity",
    "id": "1616991463150",
    "replyToId": null,
    "etag": "1616991463150",
    "messageType": "message",
    "createdDateTime": "2021-03-29T04:17:43.15Z",
    "lastModifiedDateTime": "2021-03-29T04:17:43.15Z",
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
        "content": "Hello World"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
