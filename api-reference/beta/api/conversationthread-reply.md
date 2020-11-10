---
title: 'conversationThread: reply'
description: 'Responde a um thread em uma conversa de grupo e adicione uma nova postagem a ele. Você pode especificar a conversa pai '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 076f3d3eddb6ca0c33eabe706e7b58fd22cfd54b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956622"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="d9e59-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="d9e59-104">conversationThread: reply</span></span>

<span data-ttu-id="d9e59-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9e59-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9e59-p102">Responde a um thread em uma conversa de grupo e adicione uma nova postagem a ele. Você pode especificar a conversa pai na solicitação ou apenas o thread, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="d9e59-p102">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9e59-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9e59-108">Permissions</span></span>
<span data-ttu-id="d9e59-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9e59-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9e59-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9e59-111">Permission type</span></span>      | <span data-ttu-id="d9e59-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9e59-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9e59-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9e59-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d9e59-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9e59-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d9e59-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9e59-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9e59-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9e59-116">Not supported.</span></span>    |
|<span data-ttu-id="d9e59-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9e59-117">Application</span></span> | <span data-ttu-id="d9e59-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9e59-118">Not supported.</span></span>    |

## <a name="http-request"></a><span data-ttu-id="d9e59-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9e59-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="d9e59-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9e59-120">Request headers</span></span>
| <span data-ttu-id="d9e59-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9e59-121">Header</span></span>       | <span data-ttu-id="d9e59-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d9e59-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d9e59-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9e59-123">Authorization</span></span>  | <span data-ttu-id="d9e59-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9e59-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d9e59-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9e59-126">Content-Type</span></span>  | <span data-ttu-id="d9e59-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9e59-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d9e59-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9e59-129">Request body</span></span>
<span data-ttu-id="d9e59-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9e59-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d9e59-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d9e59-131">Parameter</span></span>    | <span data-ttu-id="d9e59-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9e59-132">Type</span></span>   |<span data-ttu-id="d9e59-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9e59-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9e59-134">post</span><span class="sxs-lookup"><span data-stu-id="d9e59-134">post</span></span>|[<span data-ttu-id="d9e59-135">post</span><span class="sxs-lookup"><span data-stu-id="d9e59-135">post</span></span>](../resources/post.md)|<span data-ttu-id="d9e59-136">A nova postagem que está sendo respondida.</span><span class="sxs-lookup"><span data-stu-id="d9e59-136">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="d9e59-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9e59-137">Response</span></span>

<span data-ttu-id="d9e59-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9e59-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9e59-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9e59-140">Example</span></span>
<span data-ttu-id="d9e59-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d9e59-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d9e59-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9e59-142">Request</span></span>
<span data-ttu-id="d9e59-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9e59-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9e59-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9e59-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```
# <a name="c"></a>[<span data-ttu-id="d9e59-145">C#</span><span class="sxs-lookup"><span data-stu-id="d9e59-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/conversationthread-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9e59-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9e59-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/conversationthread-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9e59-147">Java</span><span class="sxs-lookup"><span data-stu-id="d9e59-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/conversationthread-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d9e59-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9e59-148">Response</span></span>
<span data-ttu-id="d9e59-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9e59-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


