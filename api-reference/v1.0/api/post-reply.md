---
title: 'post: reply'
description: 'Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo. Você pode especificar '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0df8c2c586d4522a2287cbdedb909df5b3e4f24e
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622548"
---
# <a name="post-reply"></a><span data-ttu-id="796c0-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="796c0-104">post: reply</span></span>

<span data-ttu-id="796c0-105">Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="796c0-105">Reply to a post and add a new post to the specified thread in a group conversation.</span></span> 

<span data-ttu-id="796c0-106">Você pode especificar a conversa pai e o thread na solicitação ou pode especificar apenas o thread pai, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="796c0-106">You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="796c0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="796c0-107">Permissions</span></span>
<span data-ttu-id="796c0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="796c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="796c0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="796c0-110">Permission type</span></span>      | <span data-ttu-id="796c0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="796c0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="796c0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="796c0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="796c0-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="796c0-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="796c0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="796c0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="796c0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="796c0-115">Not supported.</span></span>    |
|<span data-ttu-id="796c0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="796c0-116">Application</span></span> | <span data-ttu-id="796c0-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="796c0-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="796c0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="796c0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="796c0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="796c0-119">Request headers</span></span>
| <span data-ttu-id="796c0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="796c0-120">Header</span></span>       | <span data-ttu-id="796c0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="796c0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="796c0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="796c0-122">Authorization</span></span>  | <span data-ttu-id="796c0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="796c0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="796c0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="796c0-125">Request body</span></span>
<span data-ttu-id="796c0-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="796c0-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="796c0-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="796c0-127">Parameter</span></span>    | <span data-ttu-id="796c0-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="796c0-128">Type</span></span>   |<span data-ttu-id="796c0-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="796c0-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="796c0-130">post</span><span class="sxs-lookup"><span data-stu-id="796c0-130">post</span></span>|[<span data-ttu-id="796c0-131">post</span><span class="sxs-lookup"><span data-stu-id="796c0-131">post</span></span>](../resources/post.md)|<span data-ttu-id="796c0-132">A nova postagem que está sendo respondida.</span><span class="sxs-lookup"><span data-stu-id="796c0-132">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="796c0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="796c0-133">Response</span></span>

<span data-ttu-id="796c0-p104">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="796c0-p104">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="796c0-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="796c0-136">Example</span></span>
<span data-ttu-id="796c0-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="796c0-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="796c0-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="796c0-138">Request</span></span>
<span data-ttu-id="796c0-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="796c0-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="796c0-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="796c0-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="796c0-141">C#</span><span class="sxs-lookup"><span data-stu-id="796c0-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="796c0-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="796c0-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="796c0-143">Java</span><span class="sxs-lookup"><span data-stu-id="796c0-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="796c0-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="796c0-144">Response</span></span>
<span data-ttu-id="796c0-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="796c0-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
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
