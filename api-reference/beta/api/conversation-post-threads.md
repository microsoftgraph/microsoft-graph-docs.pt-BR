---
title: Criar thread
description: Crie um novo thread na conversa especificada.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7a78352847ff8ff5aa64249bf688168d3c9df2a1
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417806"
---
# <a name="create-thread"></a><span data-ttu-id="a327d-103">Criar thread</span><span class="sxs-lookup"><span data-stu-id="a327d-103">Create thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a327d-104">Crie um novo thread na conversa especificada.</span><span class="sxs-lookup"><span data-stu-id="a327d-104">Create a new thread in the specified conversation.</span></span>

<span data-ttu-id="a327d-p101">Um thread e uma postagem são criados conforme especificado. Use [responder ao thread](conversationthread-reply.md) para incluir postagens adicionais no thread. Ou, se receber a ID de postagem, você também poderá [responder](post-reply.md) a essa postagem no thread.</span><span class="sxs-lookup"><span data-stu-id="a327d-p101">A thread and post are created as specified. Use [reply thread](conversationthread-reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post-reply.md) to that post in that thread.</span></span>

<span data-ttu-id="a327d-108">Observação: Você também pode [Iniciar uma nova conversa criando primeiro um thread](group-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="a327d-108">Note: You can also [start a new conversation by first creating a thread](group-post-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a327d-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="a327d-109">Permissions</span></span>
<span data-ttu-id="a327d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a327d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a327d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a327d-112">Permission type</span></span>      | <span data-ttu-id="a327d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a327d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a327d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a327d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a327d-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a327d-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a327d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a327d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a327d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a327d-117">Not supported.</span></span>    |
|<span data-ttu-id="a327d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a327d-118">Application</span></span> | <span data-ttu-id="a327d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a327d-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a327d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a327d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="a327d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a327d-121">Request headers</span></span>
| <span data-ttu-id="a327d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a327d-122">Name</span></span>       | <span data-ttu-id="a327d-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="a327d-123">Type</span></span> | <span data-ttu-id="a327d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a327d-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a327d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a327d-125">Authorization</span></span>  | <span data-ttu-id="a327d-126">string</span><span class="sxs-lookup"><span data-stu-id="a327d-126">string</span></span>  | <span data-ttu-id="a327d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a327d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a327d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a327d-129">Request body</span></span>
<span data-ttu-id="a327d-130">No corpo da solicitação, forneça uma representação JSON do objeto [ConversationThread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="a327d-130">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a327d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a327d-131">Response</span></span>

<span data-ttu-id="a327d-132">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [ConversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a327d-132">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a327d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a327d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a327d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a327d-134">Request</span></span>
<span data-ttu-id="a327d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a327d-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a327d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a327d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_conversation"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
Content-type: application/json

{
  "topic": "topic-value",
  "posts": [{
      "body": {
        "contentType": "html",
        "content": "this is body content"
      }
  }]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a327d-137">C#</span><span class="sxs-lookup"><span data-stu-id="a327d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationthread-from-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a327d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a327d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationthread-from-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a327d-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a327d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationthread-from-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a327d-140">No corpo da solicitação, forneça uma representação JSON do objeto [ConversationThread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="a327d-140">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a327d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a327d-141">Response</span></span>

<span data-ttu-id="a327d-p104">Se for bem-sucedido, este método retornará um código de resposta `201 Created` e o `id` do novo thread no corpo da resposta. Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a327d-p104">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
