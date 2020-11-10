---
title: Criar thread
description: Crie um novo thread na conversa especificada.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 31142bb2277f32aec1556d20e0915b97e621645a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956803"
---
# <a name="create-thread"></a><span data-ttu-id="b99de-103">Criar thread</span><span class="sxs-lookup"><span data-stu-id="b99de-103">Create thread</span></span>

<span data-ttu-id="b99de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b99de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b99de-105">Crie um novo thread na conversa especificada.</span><span class="sxs-lookup"><span data-stu-id="b99de-105">Create a new thread in the specified conversation.</span></span>

<span data-ttu-id="b99de-p101">Um thread e uma postagem são criados conforme especificado. Use [responder ao thread](conversationthread-reply.md) para incluir postagens adicionais no thread. Ou, se receber a ID de postagem, você também poderá [responder](post-reply.md) a essa postagem no thread.</span><span class="sxs-lookup"><span data-stu-id="b99de-p101">A thread and post are created as specified. Use [reply thread](conversationthread-reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post-reply.md) to that post in that thread.</span></span>

<span data-ttu-id="b99de-109">Observação: Você também pode [Iniciar uma nova conversa criando primeiro um thread](group-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="b99de-109">Note: You can also [start a new conversation by first creating a thread](group-post-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b99de-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="b99de-110">Permissions</span></span>
<span data-ttu-id="b99de-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b99de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b99de-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b99de-113">Permission type</span></span>      | <span data-ttu-id="b99de-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b99de-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b99de-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b99de-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b99de-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b99de-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b99de-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b99de-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b99de-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b99de-118">Not supported.</span></span>    |
|<span data-ttu-id="b99de-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b99de-119">Application</span></span> | <span data-ttu-id="b99de-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b99de-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b99de-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b99de-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="b99de-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b99de-122">Request headers</span></span>
| <span data-ttu-id="b99de-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b99de-123">Name</span></span>       | <span data-ttu-id="b99de-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b99de-124">Type</span></span> | <span data-ttu-id="b99de-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b99de-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b99de-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b99de-126">Authorization</span></span>  | <span data-ttu-id="b99de-127">string</span><span class="sxs-lookup"><span data-stu-id="b99de-127">string</span></span>  | <span data-ttu-id="b99de-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b99de-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b99de-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b99de-130">Request body</span></span>
<span data-ttu-id="b99de-131">No corpo da solicitação, forneça uma representação JSON do objeto [ConversationThread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="b99de-131">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b99de-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b99de-132">Response</span></span>

<span data-ttu-id="b99de-133">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [ConversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b99de-133">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b99de-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b99de-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b99de-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b99de-135">Request</span></span>
<span data-ttu-id="b99de-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b99de-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b99de-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b99de-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b99de-138">C#</span><span class="sxs-lookup"><span data-stu-id="b99de-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationthread-from-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b99de-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b99de-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationthread-from-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b99de-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b99de-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationthread-from-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b99de-141">Java</span><span class="sxs-lookup"><span data-stu-id="b99de-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversationthread-from-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b99de-142">No corpo da solicitação, forneça uma representação JSON do objeto [ConversationThread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="b99de-142">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b99de-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b99de-143">Response</span></span>

<span data-ttu-id="b99de-p104">Se for bem-sucedido, este método retornará um código de resposta `201 Created` e o `id` do novo thread no corpo da resposta. Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b99de-p104">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span>
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


