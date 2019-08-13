---
title: Criar thread
description: Crie um novo thread na conversa especificada.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b989e4dbf368324bc43ffd2259118dc8db155dfb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319731"
---
# <a name="create-thread"></a><span data-ttu-id="2dbc1-103">Criar thread</span><span class="sxs-lookup"><span data-stu-id="2dbc1-103">Create thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dbc1-104">Crie um novo thread na conversa especificada.</span><span class="sxs-lookup"><span data-stu-id="2dbc1-104">Create a new thread in the specified conversation.</span></span>

<span data-ttu-id="2dbc1-p101">Um thread e uma postagem são criados conforme especificado. Use [responder ao thread](conversationthread-reply.md) para incluir postagens adicionais no thread. Ou, se receber a ID de postagem, você também poderá [responder](post-reply.md) a essa postagem no thread.</span><span class="sxs-lookup"><span data-stu-id="2dbc1-p101">A thread and post are created as specified. Use [reply thread](conversationthread-reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post-reply.md) to that post in that thread.</span></span>

<span data-ttu-id="2dbc1-108">Observação: Você também pode [Iniciar uma nova conversa criando primeiro um thread](group-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="2dbc1-108">Note: You can also [start a new conversation by first creating a thread](group-post-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2dbc1-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="2dbc1-109">Permissions</span></span>
<span data-ttu-id="2dbc1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2dbc1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dbc1-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2dbc1-112">Permission type</span></span>      | <span data-ttu-id="2dbc1-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2dbc1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2dbc1-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2dbc1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2dbc1-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dbc1-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2dbc1-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2dbc1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2dbc1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2dbc1-117">Not supported.</span></span>    |
|<span data-ttu-id="2dbc1-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2dbc1-118">Application</span></span> | <span data-ttu-id="2dbc1-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2dbc1-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2dbc1-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2dbc1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="2dbc1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2dbc1-121">Request headers</span></span>
| <span data-ttu-id="2dbc1-122">Nome</span><span class="sxs-lookup"><span data-stu-id="2dbc1-122">Name</span></span>       | <span data-ttu-id="2dbc1-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="2dbc1-123">Type</span></span> | <span data-ttu-id="2dbc1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dbc1-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2dbc1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2dbc1-125">Authorization</span></span>  | <span data-ttu-id="2dbc1-126">string</span><span class="sxs-lookup"><span data-stu-id="2dbc1-126">string</span></span>  | <span data-ttu-id="2dbc1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2dbc1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2dbc1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2dbc1-129">Request body</span></span>
<span data-ttu-id="2dbc1-130">No corpo da solicitação, forneça uma representação JSON do objeto [ConversationThread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="2dbc1-130">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2dbc1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2dbc1-131">Response</span></span>

<span data-ttu-id="2dbc1-132">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [ConversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2dbc1-132">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2dbc1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2dbc1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2dbc1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2dbc1-134">Request</span></span>
<span data-ttu-id="2dbc1-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2dbc1-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2dbc1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2dbc1-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2dbc1-137">C#</span><span class="sxs-lookup"><span data-stu-id="2dbc1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationthread-from-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2dbc1-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2dbc1-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationthread-from-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2dbc1-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2dbc1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationthread-from-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2dbc1-140">Java</span><span class="sxs-lookup"><span data-stu-id="2dbc1-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversationthread-from-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2dbc1-141">No corpo da solicitação, forneça uma representação JSON do objeto [ConversationThread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="2dbc1-141">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2dbc1-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2dbc1-142">Response</span></span>

<span data-ttu-id="2dbc1-p104">Se for bem-sucedido, este método retornará um código de resposta `201 Created` e o `id` do novo thread no corpo da resposta. Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2dbc1-p104">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span>
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
