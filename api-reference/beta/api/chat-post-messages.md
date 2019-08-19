---
title: Criar chat
description: Use esta API para criar um novo chat.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 96099cf2628b31a03013ae680439e97a55f952c5
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460819"
---
# <a name="create-chatmessage"></a><span data-ttu-id="ec578-103">Criar chat</span><span class="sxs-lookup"><span data-stu-id="ec578-103">Create chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec578-104">Criar uma nova [mensagem](../resources/chatmessage.md) no [chat](../resources/chat.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="ec578-104">Create a new [message](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="ec578-105">Esta API não pode criar um novo chat, você deve usar o método [list chats](chat-list.md) para recuperar a ID de um chat existente antes de criar uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="ec578-105">This API cannot create an new chat, you must use the [list chats](chat-list.md) method to retreive the Id of an existing chat before creating a chat message.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec578-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec578-106">Permissions</span></span>

<span data-ttu-id="ec578-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec578-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec578-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec578-109">Permission type</span></span>                        | <span data-ttu-id="ec578-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec578-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ec578-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec578-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec578-112">Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec578-112">Chat.ReadWrite</span></span> |
| <span data-ttu-id="ec578-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec578-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec578-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec578-114">Not supported.</span></span> |
| <span data-ttu-id="ec578-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec578-115">Application</span></span>                            | <span data-ttu-id="ec578-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec578-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec578-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec578-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="ec578-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec578-118">Request headers</span></span>

| <span data-ttu-id="ec578-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ec578-119">Name</span></span>          | <span data-ttu-id="ec578-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec578-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ec578-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec578-121">Authorization</span></span> | <span data-ttu-id="ec578-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="ec578-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec578-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec578-123">Request body</span></span>

<span data-ttu-id="ec578-124">No corpo da solicitação, forneça uma representação JSON do objeto [chat](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="ec578-124">In the request body, supply a JSON representation of [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ec578-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec578-125">Response</span></span>

<span data-ttu-id="ec578-126">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [chat](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec578-126">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ec578-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ec578-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ec578-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec578-128">Request</span></span>

<span data-ttu-id="ec578-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec578-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ec578-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec578-130">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ec578-131">C#</span><span class="sxs-lookup"><span data-stu-id="ec578-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ec578-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec578-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ec578-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ec578-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ec578-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec578-134">Response</span></span>

<span data-ttu-id="ec578-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ec578-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="ec578-136">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ec578-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ec578-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec578-137">All the properties will be returned from an actual call.</span></span>

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
