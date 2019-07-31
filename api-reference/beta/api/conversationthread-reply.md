---
title: 'conversationThread: reply'
description: 'Responde a um thread em uma conversa de grupo e adicione uma nova postagem a ele. Você pode especificar a conversa pai '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b4743de1b825a3aeb5915c0e984b807fe198e3be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943040"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="df62c-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="df62c-104">conversationThread: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df62c-p102">Responde a um thread em uma conversa de grupo e adicione uma nova postagem a ele. Você pode especificar a conversa pai na solicitação ou apenas o thread, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="df62c-p102">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="df62c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="df62c-107">Permissions</span></span>
<span data-ttu-id="df62c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df62c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df62c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df62c-110">Permission type</span></span>      | <span data-ttu-id="df62c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df62c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df62c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df62c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="df62c-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df62c-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="df62c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df62c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df62c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df62c-115">Not supported.</span></span>    |
|<span data-ttu-id="df62c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df62c-116">Application</span></span> | <span data-ttu-id="df62c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df62c-117">Not supported.</span></span>    |

## <a name="http-request"></a><span data-ttu-id="df62c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df62c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="df62c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df62c-119">Request headers</span></span>
| <span data-ttu-id="df62c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df62c-120">Header</span></span>       | <span data-ttu-id="df62c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="df62c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="df62c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="df62c-122">Authorization</span></span>  | <span data-ttu-id="df62c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df62c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="df62c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="df62c-125">Content-Type</span></span>  | <span data-ttu-id="df62c-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df62c-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df62c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df62c-128">Request body</span></span>
<span data-ttu-id="df62c-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df62c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="df62c-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="df62c-130">Parameter</span></span>    | <span data-ttu-id="df62c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="df62c-131">Type</span></span>   |<span data-ttu-id="df62c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="df62c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df62c-133">post</span><span class="sxs-lookup"><span data-stu-id="df62c-133">post</span></span>|[<span data-ttu-id="df62c-134">post</span><span class="sxs-lookup"><span data-stu-id="df62c-134">post</span></span>](../resources/post.md)|<span data-ttu-id="df62c-135">A nova postagem que está sendo respondida.</span><span class="sxs-lookup"><span data-stu-id="df62c-135">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="df62c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="df62c-136">Response</span></span>

<span data-ttu-id="df62c-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df62c-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df62c-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df62c-139">Example</span></span>
<span data-ttu-id="df62c-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="df62c-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="df62c-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df62c-141">Request</span></span>
<span data-ttu-id="df62c-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df62c-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="df62c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="df62c-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="df62c-144">C#</span><span class="sxs-lookup"><span data-stu-id="df62c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/conversationthread-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="df62c-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="df62c-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/conversationthread-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="df62c-146">Java</span><span class="sxs-lookup"><span data-stu-id="df62c-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/conversationthread-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="df62c-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="df62c-147">Response</span></span>
<span data-ttu-id="df62c-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df62c-148">Here is an example of the response.</span></span>
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
