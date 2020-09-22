---
title: Criar thread
description: Crie um novo thread na conversa especificada.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 886c0f0e11032f758bf9004e2d42d7c46da5a830
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002797"
---
# <a name="create-thread"></a><span data-ttu-id="0fa33-103">Criar thread</span><span class="sxs-lookup"><span data-stu-id="0fa33-103">Create thread</span></span>

<span data-ttu-id="0fa33-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fa33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fa33-105">Crie um novo thread na conversa especificada.</span><span class="sxs-lookup"><span data-stu-id="0fa33-105">Create a new thread in the specified conversation.</span></span>

<span data-ttu-id="0fa33-p101">Um thread e uma postagem são criados conforme especificado. Use [responder ao thread](conversationthread-reply.md) para incluir postagens adicionais no thread. Ou, se receber a ID de postagem, você também poderá [responder](post-reply.md) a essa postagem no thread.</span><span class="sxs-lookup"><span data-stu-id="0fa33-p101">A thread and post are created as specified. Use [reply thread](conversationthread-reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post-reply.md) to that post in that thread.</span></span>

<span data-ttu-id="0fa33-109">Observação: Você também pode [Iniciar uma nova conversa criando primeiro um thread](group-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="0fa33-109">Note: You can also [start a new conversation by first creating a thread](group-post-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0fa33-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="0fa33-110">Permissions</span></span>
<span data-ttu-id="0fa33-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fa33-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fa33-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fa33-113">Permission type</span></span>      | <span data-ttu-id="0fa33-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0fa33-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fa33-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fa33-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0fa33-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fa33-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0fa33-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fa33-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fa33-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fa33-118">Not supported.</span></span>    |
|<span data-ttu-id="0fa33-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fa33-119">Application</span></span> | <span data-ttu-id="0fa33-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fa33-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fa33-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fa33-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="0fa33-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa33-122">Request headers</span></span>
| <span data-ttu-id="0fa33-123">Nome</span><span class="sxs-lookup"><span data-stu-id="0fa33-123">Name</span></span>       | <span data-ttu-id="0fa33-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="0fa33-124">Type</span></span> | <span data-ttu-id="0fa33-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fa33-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0fa33-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fa33-126">Authorization</span></span>  | <span data-ttu-id="0fa33-127">string</span><span class="sxs-lookup"><span data-stu-id="0fa33-127">string</span></span>  | <span data-ttu-id="0fa33-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fa33-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fa33-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa33-130">Request body</span></span>
<span data-ttu-id="0fa33-131">No corpo da solicitação, forneça uma representação JSON do objeto [ConversationThread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="0fa33-131">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0fa33-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fa33-132">Response</span></span>

<span data-ttu-id="0fa33-133">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [ConversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fa33-133">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fa33-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fa33-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0fa33-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fa33-135">Request</span></span>
<span data-ttu-id="0fa33-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fa33-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0fa33-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fa33-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0fa33-138">C#</span><span class="sxs-lookup"><span data-stu-id="0fa33-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationthread-from-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fa33-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fa33-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationthread-from-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fa33-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fa33-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationthread-from-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0fa33-141">No corpo da solicitação, forneça uma representação JSON do objeto [ConversationThread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="0fa33-141">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0fa33-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fa33-142">Response</span></span>

<span data-ttu-id="0fa33-p104">Se for bem-sucedido, este método retornará um código de resposta `201 Created` e o `id` do novo thread no corpo da resposta. Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fa33-p104">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span>
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


