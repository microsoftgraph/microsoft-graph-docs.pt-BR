---
title: 'post: reply'
description: 'Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo. Você pode especificar '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6059240cfd0dfe8fd3155338233fee9d2384d80f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978815"
---
# <a name="post-reply"></a><span data-ttu-id="bbe70-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="bbe70-104">post: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbe70-p102">Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo. Você pode especificar a conversa pai e o thread na solicitação ou pode especificar apenas o thread pai, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="bbe70-p102">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbe70-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbe70-107">Permissions</span></span>
<span data-ttu-id="bbe70-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbe70-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbe70-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbe70-110">Permission type</span></span>      | <span data-ttu-id="bbe70-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbe70-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbe70-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbe70-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bbe70-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbe70-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bbe70-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbe70-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbe70-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbe70-115">Not supported.</span></span>    |
|<span data-ttu-id="bbe70-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbe70-116">Application</span></span> | <span data-ttu-id="bbe70-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbe70-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbe70-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbe70-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="bbe70-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbe70-119">Request headers</span></span>
| <span data-ttu-id="bbe70-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bbe70-120">Header</span></span>       | <span data-ttu-id="bbe70-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bbe70-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bbe70-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbe70-122">Authorization</span></span>  | <span data-ttu-id="bbe70-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbe70-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bbe70-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbe70-125">Request body</span></span>
<span data-ttu-id="bbe70-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbe70-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bbe70-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bbe70-127">Parameter</span></span>    | <span data-ttu-id="bbe70-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbe70-128">Type</span></span>   |<span data-ttu-id="bbe70-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbe70-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbe70-130">post</span><span class="sxs-lookup"><span data-stu-id="bbe70-130">post</span></span>|[<span data-ttu-id="bbe70-131">post</span><span class="sxs-lookup"><span data-stu-id="bbe70-131">post</span></span>](../resources/post.md)|<span data-ttu-id="bbe70-132">A nova postagem que está sendo respondida.</span><span class="sxs-lookup"><span data-stu-id="bbe70-132">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="bbe70-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbe70-133">Response</span></span>

<span data-ttu-id="bbe70-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbe70-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbe70-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbe70-136">Example</span></span>
<span data-ttu-id="bbe70-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="bbe70-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bbe70-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbe70-138">Request</span></span>
<span data-ttu-id="bbe70-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbe70-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bbe70-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbe70-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "2016-10-19T10:37:00Z",
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
    "createdDateTime": "2016-10-19T10:37:00Z",
    "lastModifiedDateTime": "2016-10-19T10:37:00Z",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "lastModifiedDateTime": "2016-10-19T10:37:00Z",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="bbe70-141">C#</span><span class="sxs-lookup"><span data-stu-id="bbe70-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bbe70-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="bbe70-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bbe70-143">Java</span><span class="sxs-lookup"><span data-stu-id="bbe70-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bbe70-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbe70-144">Response</span></span>
##### <a name="response"></a><span data-ttu-id="bbe70-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbe70-145">Response</span></span>
<span data-ttu-id="bbe70-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbe70-146">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
