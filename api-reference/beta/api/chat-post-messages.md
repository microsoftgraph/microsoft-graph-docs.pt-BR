---
title: Criar chat
description: Use esta API para criar um novo chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 62fbbabb3ad50b00706d717dd9b4d2a7a8db97de
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437814"
---
# <a name="create-chatmessage"></a><span data-ttu-id="b8cab-103">Criar chat</span><span class="sxs-lookup"><span data-stu-id="b8cab-103">Create chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8cab-104">Criar uma nova [mensagem](../resources/chatmessage.md) no [chat](../resources/chat.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="b8cab-104">Create a new [message](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8cab-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8cab-105">Permissions</span></span>

<span data-ttu-id="b8cab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8cab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8cab-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8cab-108">Permission type</span></span>                        | <span data-ttu-id="b8cab-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8cab-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b8cab-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8cab-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8cab-111">Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8cab-111">Chat.ReadWrite</span></span> |
| <span data-ttu-id="b8cab-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8cab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8cab-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8cab-113">Not supported.</span></span> |
| <span data-ttu-id="b8cab-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8cab-114">Application</span></span>                            | <span data-ttu-id="b8cab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8cab-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8cab-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8cab-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="b8cab-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8cab-117">Request headers</span></span>

| <span data-ttu-id="b8cab-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b8cab-118">Name</span></span>          | <span data-ttu-id="b8cab-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8cab-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b8cab-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8cab-120">Authorization</span></span> | <span data-ttu-id="b8cab-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="b8cab-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8cab-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8cab-122">Request body</span></span>

<span data-ttu-id="b8cab-123">No corpo da solicitação, forneça uma representação JSON do objeto [chat](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="b8cab-123">In the request body, supply a JSON representation of [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b8cab-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8cab-124">Response</span></span>

<span data-ttu-id="b8cab-125">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [chat](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8cab-125">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b8cab-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b8cab-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b8cab-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8cab-127">Request</span></span>

<span data-ttu-id="b8cab-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8cab-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b8cab-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8cab-129">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b8cab-130">C#</span><span class="sxs-lookup"><span data-stu-id="b8cab-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8cab-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="b8cab-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b8cab-132">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b8cab-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b8cab-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8cab-133">Response</span></span>

<span data-ttu-id="b8cab-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8cab-134">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b8cab-135">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b8cab-135">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b8cab-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8cab-136">All the properties will be returned from an actual call.</span></span>

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
