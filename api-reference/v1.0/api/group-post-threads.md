---
title: Criar thread de conversas
description: 'Inicie uma nova conversa em grupo criando primeiro um thread. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c8d5c4d4025f8928acd5a8a40e0b8c6ca7a3fb18
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516960"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="89488-103">Criar thread de conversas</span><span class="sxs-lookup"><span data-stu-id="89488-103">Create conversation thread</span></span>

<span data-ttu-id="89488-104">Namespace: Microsoft. Graph inicie uma nova conversa de grupo criando primeiro um thread.</span><span class="sxs-lookup"><span data-stu-id="89488-104">Namespace: microsoft.graph Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="89488-p101">Uma nova conversa, thread de conversas e posts são criados no grupo. Use [reply thread](conversationthread-reply.md) ou [reply post](post-reply.md) para postar mais naquele thread.</span><span class="sxs-lookup"><span data-stu-id="89488-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="89488-107">Observação: também é possível [iniciar um novo thread em uma conversa existente](conversation-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="89488-107">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="89488-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="89488-108">Permissions</span></span>
<span data-ttu-id="89488-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89488-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89488-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89488-111">Permission type</span></span>      | <span data-ttu-id="89488-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89488-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89488-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89488-113">Delegated (work or school account)</span></span> | <span data-ttu-id="89488-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89488-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="89488-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89488-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89488-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89488-116">Not supported.</span></span>    |
|<span data-ttu-id="89488-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89488-117">Application</span></span> | <span data-ttu-id="89488-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89488-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89488-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89488-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="89488-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89488-120">Request headers</span></span>
| <span data-ttu-id="89488-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89488-121">Header</span></span>       | <span data-ttu-id="89488-122">Valor</span><span class="sxs-lookup"><span data-stu-id="89488-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="89488-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="89488-123">Authorization</span></span>  | <span data-ttu-id="89488-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89488-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="89488-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89488-126">Content-Type</span></span>  | <span data-ttu-id="89488-127">application/json</span><span class="sxs-lookup"><span data-stu-id="89488-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="89488-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89488-128">Request body</span></span>
<span data-ttu-id="89488-129">No corpo da solicitação, forneça uma representação JSON do objeto [conversationThread](../resources/conversationthread.md) que contém um [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="89488-129">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="89488-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="89488-130">Response</span></span>
<span data-ttu-id="89488-131">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89488-131">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89488-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89488-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="89488-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89488-133">Request</span></span>
<span data-ttu-id="89488-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="89488-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="89488-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="89488-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads
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
# <a name="c"></a>[<span data-ttu-id="89488-136">C#</span><span class="sxs-lookup"><span data-stu-id="89488-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationthread-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89488-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89488-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationthread-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89488-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89488-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationthread-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89488-139">Java</span><span class="sxs-lookup"><span data-stu-id="89488-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversationthread-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="89488-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="89488-140">Response</span></span>
<span data-ttu-id="89488-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="89488-141">The following is an example of the response.</span></span>
><span data-ttu-id="89488-142">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="89488-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="89488-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89488-143">All the properties will be returned from an actual call.</span></span>
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
  "lastDeliveredDateTime": "datetime-value",
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
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
