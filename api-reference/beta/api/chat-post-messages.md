---
title: Criar chat
description: Use esta API para criar um novo chat.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 917b5ec5ac140079f30f6c03db485de849d6b56b
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44287511"
---
# <a name="create-chatmessage"></a><span data-ttu-id="5d3d7-103">Criar chat</span><span class="sxs-lookup"><span data-stu-id="5d3d7-103">Create chatMessage</span></span>

<span data-ttu-id="5d3d7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d3d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d3d7-105">Criar uma nova [mensagem](../resources/chatmessage.md) no [chat](../resources/chat.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="5d3d7-105">Create a new [message](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="5d3d7-106">Esta API não pode criar um novo chat, você deve usar o método [list chats](chat-list.md) para recuperar a ID de um chat existente antes de criar uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="5d3d7-106">This API cannot create an new chat, you must use the [list chats](chat-list.md) method to retreive the Id of an existing chat before creating a chat message.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d3d7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d3d7-107">Permissions</span></span>

<span data-ttu-id="5d3d7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d3d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5d3d7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d3d7-110">Permission type</span></span>                        | <span data-ttu-id="5d3d7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d3d7-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5d3d7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d3d7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d3d7-113">Chat. Send, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d3d7-113">ChatMessage.Send, Chat.ReadWrite</span></span> |
| <span data-ttu-id="5d3d7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d3d7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d3d7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d3d7-115">Not supported.</span></span> |
| <span data-ttu-id="5d3d7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d3d7-116">Application</span></span>                            | <span data-ttu-id="5d3d7-117">Chat. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5d3d7-117">Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d3d7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d3d7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="5d3d7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d3d7-119">Request headers</span></span>

| <span data-ttu-id="5d3d7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5d3d7-120">Name</span></span>          | <span data-ttu-id="5d3d7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d3d7-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5d3d7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d3d7-122">Authorization</span></span> | <span data-ttu-id="5d3d7-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="5d3d7-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d3d7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d3d7-124">Request body</span></span>

<span data-ttu-id="5d3d7-125">No corpo da solicitação, forneça uma representação JSON do objeto [chat](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="5d3d7-125">In the request body, supply a JSON representation of [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5d3d7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d3d7-126">Response</span></span>

<span data-ttu-id="5d3d7-127">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [chat](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d3d7-127">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5d3d7-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5d3d7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5d3d7-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d3d7-129">Request</span></span>

<span data-ttu-id="5d3d7-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d3d7-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d3d7-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d3d7-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_chat"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
     "content" : "Hello world"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="5d3d7-132">C#</span><span class="sxs-lookup"><span data-stu-id="5d3d7-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d3d7-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d3d7-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d3d7-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d3d7-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5d3d7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d3d7-135">Response</span></span>

<span data-ttu-id="5d3d7-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5d3d7-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="5d3d7-137">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5d3d7-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5d3d7-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d3d7-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "replyToId": "replyToId-value",
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "87ea812c-8816-40e9-b770-5c165fa31397",
      "displayName": "Test User"
    }
  },
  "messageType": "message",
  "body": {
     "content": "Hello world",
     "contentType": "text"
  }
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
