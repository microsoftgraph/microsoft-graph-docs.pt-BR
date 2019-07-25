---
title: Criar thread de conversas
description: 'Inicie uma nova conversa em grupo criando primeiro um thread. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: ffa0124f658e474588262d868fd5d2a66e3fc7c9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857931"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="c4352-103">Criar thread de conversas</span><span class="sxs-lookup"><span data-stu-id="c4352-103">Create conversation thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4352-104">Inicie uma nova conversa em grupo criando primeiro um thread.</span><span class="sxs-lookup"><span data-stu-id="c4352-104">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="c4352-p101">Uma nova conversa, thread de conversas e posts são criados no grupo. Use [reply thread](conversationthread-reply.md) ou [reply post](post-reply.md) para postar mais naquele thread.</span><span class="sxs-lookup"><span data-stu-id="c4352-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="c4352-107">Observação: também é possível [iniciar um novo thread em uma conversa existente](conversation-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="c4352-107">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="c4352-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4352-108">Permissions</span></span>
<span data-ttu-id="c4352-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4352-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4352-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4352-111">Permission type</span></span>      | <span data-ttu-id="c4352-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4352-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4352-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4352-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c4352-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4352-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c4352-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4352-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4352-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4352-116">Not supported.</span></span>    |
|<span data-ttu-id="c4352-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4352-117">Application</span></span> | <span data-ttu-id="c4352-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4352-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4352-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4352-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="c4352-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4352-120">Request headers</span></span>
| <span data-ttu-id="c4352-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4352-121">Header</span></span>       | <span data-ttu-id="c4352-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c4352-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c4352-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4352-123">Authorization</span></span>  | <span data-ttu-id="c4352-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4352-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c4352-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4352-126">Content-Type</span></span>  | <span data-ttu-id="c4352-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c4352-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c4352-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4352-128">Request body</span></span>
<span data-ttu-id="c4352-129">No corpo da solicitação, forneça uma representação JSON do objeto [conversationThread](../resources/conversationthread.md) que contém um [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="c4352-129">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="c4352-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4352-130">Response</span></span>
<span data-ttu-id="c4352-131">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4352-131">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4352-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4352-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c4352-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4352-133">Request</span></span>
<span data-ttu-id="c4352-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4352-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c4352-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4352-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads
Content-type: application/json

{
  "topic": "New Conversation Thread Topic",
  "posts": [{
    "body": {
      "contentType": "html",
      "content": "this is body content"
    },
    "newParticipants": [{
      "emailAddress": {
        "name": "Alex Darrow",
        "address": "alexd@contoso.com"
      }
    }]
  }]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4352-136">C#</span><span class="sxs-lookup"><span data-stu-id="c4352-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationthread-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4352-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="c4352-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationthread-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4352-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c4352-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationthread-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c4352-139">Java</span><span class="sxs-lookup"><span data-stu-id="c4352-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversationthread-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c4352-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4352-140">Response</span></span>
<span data-ttu-id="c4352-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c4352-141">The following is an example of the response.</span></span>
><span data-ttu-id="c4352-142">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c4352-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c4352-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4352-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
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
