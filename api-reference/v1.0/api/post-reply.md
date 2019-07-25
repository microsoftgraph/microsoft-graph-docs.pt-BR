---
title: 'post: reply'
description: 'Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo. Você pode especificar '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: be33bf35eb840daebabafb316c210f1f728ffef1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888654"
---
# <a name="post-reply"></a><span data-ttu-id="b6cb7-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="b6cb7-104">post: reply</span></span>

<span data-ttu-id="b6cb7-p102">Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo. Você pode especificar a conversa pai e o thread na solicitação ou pode especificar apenas o thread pai, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="b6cb7-p102">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6cb7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6cb7-107">Permissions</span></span>
<span data-ttu-id="b6cb7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6cb7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6cb7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6cb7-110">Permission type</span></span>      | <span data-ttu-id="b6cb7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6cb7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6cb7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6cb7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b6cb7-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6cb7-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b6cb7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6cb7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6cb7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6cb7-115">Not supported.</span></span>    |
|<span data-ttu-id="b6cb7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6cb7-116">Application</span></span> | <span data-ttu-id="b6cb7-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6cb7-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6cb7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6cb7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="b6cb7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6cb7-119">Request headers</span></span>
| <span data-ttu-id="b6cb7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6cb7-120">Header</span></span>       | <span data-ttu-id="b6cb7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b6cb7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b6cb7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6cb7-122">Authorization</span></span>  | <span data-ttu-id="b6cb7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6cb7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b6cb7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6cb7-125">Request body</span></span>
<span data-ttu-id="b6cb7-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6cb7-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b6cb7-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b6cb7-127">Parameter</span></span>    | <span data-ttu-id="b6cb7-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6cb7-128">Type</span></span>   |<span data-ttu-id="b6cb7-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6cb7-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6cb7-130">post</span><span class="sxs-lookup"><span data-stu-id="b6cb7-130">post</span></span>|[<span data-ttu-id="b6cb7-131">post</span><span class="sxs-lookup"><span data-stu-id="b6cb7-131">post</span></span>](../resources/post.md)|<span data-ttu-id="b6cb7-132">A nova postagem que está sendo respondida.</span><span class="sxs-lookup"><span data-stu-id="b6cb7-132">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="b6cb7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6cb7-133">Response</span></span>

<span data-ttu-id="b6cb7-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6cb7-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6cb7-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6cb7-136">Example</span></span>
<span data-ttu-id="b6cb7-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b6cb7-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b6cb7-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6cb7-138">Request</span></span>
<span data-ttu-id="b6cb7-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6cb7-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b6cb7-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6cb7-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "datetime-value",
    "hasAttachments": true,
    "from": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "sender": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "conversationThreadId": "conversationThreadId-value",
    "newParticipants": [
      {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      }
    ],
    "conversationId": "conversationId-value",
    "createdDateTime": "datetime-value",
    "lastModifiedDateTime": "datetime-value",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "lastModifiedDateTime": "datetime-value",
        "name": "name-value",
        "contentType": "contentType-value",
        "size": 99,
        "isInline": true,
        "id": "id-value"
      }
    ]
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b6cb7-141">C#</span><span class="sxs-lookup"><span data-stu-id="b6cb7-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b6cb7-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="b6cb7-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b6cb7-143">Java</span><span class="sxs-lookup"><span data-stu-id="b6cb7-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b6cb7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6cb7-144">Response</span></span>
<span data-ttu-id="b6cb7-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6cb7-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
