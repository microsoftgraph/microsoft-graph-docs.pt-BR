---
title: Criar chat
description: Use esta API para criar um novo chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cb9f939e6c58ce83ad1386e9303d95978e0a6d58
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261448"
---
# <a name="create-chatmessage"></a><span data-ttu-id="be87b-103">Criar chat</span><span class="sxs-lookup"><span data-stu-id="be87b-103">Create chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be87b-104">Criar uma nova [mensagem](../resources/chatmessage.md) no [chat](../resources/chat.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="be87b-104">Create a new [message](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="be87b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="be87b-105">Permissions</span></span>

<span data-ttu-id="be87b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be87b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be87b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be87b-108">Permission type</span></span>                        | <span data-ttu-id="be87b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be87b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="be87b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be87b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="be87b-111">Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be87b-111">Chat.ReadWrite</span></span> |
| <span data-ttu-id="be87b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be87b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be87b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be87b-113">Not supported.</span></span> |
| <span data-ttu-id="be87b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be87b-114">Application</span></span>                            | <span data-ttu-id="be87b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be87b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be87b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be87b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="be87b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be87b-117">Request headers</span></span>

| <span data-ttu-id="be87b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="be87b-118">Name</span></span>          | <span data-ttu-id="be87b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="be87b-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="be87b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="be87b-120">Authorization</span></span> | <span data-ttu-id="be87b-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="be87b-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="be87b-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be87b-122">Request body</span></span>

<span data-ttu-id="be87b-123">No corpo da solicitação, forneça uma representação JSON do objeto [chat](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="be87b-123">In the request body, supply a JSON representation of [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="be87b-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="be87b-124">Response</span></span>

<span data-ttu-id="be87b-125">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [chat](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be87b-125">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be87b-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="be87b-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be87b-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be87b-127">Request</span></span>

<span data-ttu-id="be87b-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="be87b-128">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be87b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="be87b-129">Response</span></span>

<span data-ttu-id="be87b-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="be87b-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="be87b-131">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="be87b-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="be87b-132">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be87b-132">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="be87b-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="be87b-133">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="be87b-134">C#</span><span class="sxs-lookup"><span data-stu-id="be87b-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_chat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="be87b-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="be87b-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_chat-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="be87b-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="be87b-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_chat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chat-post-messages.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chat-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/chat-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}-->
