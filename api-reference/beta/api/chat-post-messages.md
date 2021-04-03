---
title: Enviar mensagem em um chat
description: Envie uma nova mensagem em um chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4f84bc4bcbcdadd050e6e300aabc89578b5e96e2
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51583009"
---
# <a name="send-message-in-a-chat"></a><span data-ttu-id="64408-103">Enviar mensagem em um chat</span><span class="sxs-lookup"><span data-stu-id="64408-103">Send message in a chat</span></span>

<span data-ttu-id="64408-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64408-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64408-105">Envie um [novo chatMessage](../resources/chatmessage.md) no chat [especificado](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="64408-105">Send a new [chatMessage](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="64408-106">Essa API não pode criar um novo chat; você deve usar o [método de chats de](chat-list.md) lista para recuperar a ID de um chat existente antes de criar uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="64408-106">This API cannot create a new chat; you must use the [list chats](chat-list.md) method to retrieve the ID of an existing chat before creating a chat message.</span></span>

> <span data-ttu-id="64408-107">**Observação**: não recomendamos que você use essa API para migração de dados.</span><span class="sxs-lookup"><span data-stu-id="64408-107">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="64408-108">Ele não tem a produtividade necessária para uma migração típica.</span><span class="sxs-lookup"><span data-stu-id="64408-108">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="64408-109">**Observação**: é uma violação dos termos [de](/legal/microsoft-apis/terms-of-use) uso usar o Microsoft Teams como um arquivo de log.</span><span class="sxs-lookup"><span data-stu-id="64408-109">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="64408-110">Envie apenas mensagens que as pessoas lerão.</span><span class="sxs-lookup"><span data-stu-id="64408-110">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="64408-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="64408-111">Permissions</span></span>

<span data-ttu-id="64408-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64408-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64408-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64408-114">Permission type</span></span>                        | <span data-ttu-id="64408-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64408-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="64408-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64408-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="64408-117">ChatMessage.Send, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64408-117">ChatMessage.Send, Chat.ReadWrite</span></span> |
| <span data-ttu-id="64408-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64408-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64408-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64408-119">Not supported.</span></span> |
| <span data-ttu-id="64408-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64408-120">Application</span></span>                            | <span data-ttu-id="64408-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64408-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64408-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64408-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{chat-id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="64408-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64408-123">Request headers</span></span>

| <span data-ttu-id="64408-124">Nome</span><span class="sxs-lookup"><span data-stu-id="64408-124">Name</span></span>          | <span data-ttu-id="64408-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="64408-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="64408-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="64408-126">Authorization</span></span> | <span data-ttu-id="64408-127">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="64408-127">Bearer {code}.</span></span> <span data-ttu-id="64408-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64408-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64408-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64408-129">Request body</span></span>

<span data-ttu-id="64408-130">No corpo da solicitação, fornece uma representação JSON de um [objeto chatMessage.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="64408-130">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="64408-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="64408-131">Response</span></span>

<span data-ttu-id="64408-132">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto chatMessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64408-132">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64408-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="64408-133">Examples</span></span>

<span data-ttu-id="64408-134">Para obter uma lista mais abrangente de exemplos, consulte [Create chatMessage in a channel or a chat](chatmessage-post.md).</span><span class="sxs-lookup"><span data-stu-id="64408-134">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="64408-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64408-135">Request</span></span>

<span data-ttu-id="64408-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64408-136">The following is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="64408-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="64408-137">Response</span></span>

<span data-ttu-id="64408-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64408-138">The following is an example of the response.</span></span>

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
