---
title: 'post: reply'
description: 'Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo. Você pode especificar '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ecc13135fee90d0fc8175669551578fe9e22d128
ms.sourcegitcommit: 7dc8ca82a8b2c25c5084e6b3121688766c9c14a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/02/2021
ms.locfileid: "50072359"
---
# <a name="post-reply"></a><span data-ttu-id="deaa9-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="deaa9-104">post: reply</span></span>

<span data-ttu-id="deaa9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deaa9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="deaa9-106">Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="deaa9-106">Reply to a post and add a new post to the specified thread in a group conversation.</span></span> 

<span data-ttu-id="deaa9-107">Você pode especificar a conversa pai e o thread na solicitação ou pode especificar apenas o thread pai, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="deaa9-107">You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="deaa9-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="deaa9-108">Permissions</span></span>
<span data-ttu-id="deaa9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="deaa9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="deaa9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="deaa9-111">Permission type</span></span>      | <span data-ttu-id="deaa9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="deaa9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="deaa9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="deaa9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="deaa9-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deaa9-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="deaa9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="deaa9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="deaa9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="deaa9-116">Not supported.</span></span>    |
|<span data-ttu-id="deaa9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="deaa9-117">Application</span></span> | <span data-ttu-id="deaa9-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deaa9-118">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="deaa9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="deaa9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="deaa9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="deaa9-120">Request headers</span></span>
| <span data-ttu-id="deaa9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="deaa9-121">Header</span></span>       | <span data-ttu-id="deaa9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="deaa9-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="deaa9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="deaa9-123">Authorization</span></span>  | <span data-ttu-id="deaa9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="deaa9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="deaa9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="deaa9-126">Request body</span></span>
<span data-ttu-id="deaa9-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="deaa9-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="deaa9-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="deaa9-128">Parameter</span></span>    | <span data-ttu-id="deaa9-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="deaa9-129">Type</span></span>   |<span data-ttu-id="deaa9-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="deaa9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="deaa9-131">post</span><span class="sxs-lookup"><span data-stu-id="deaa9-131">post</span></span>|[<span data-ttu-id="deaa9-132">post</span><span class="sxs-lookup"><span data-stu-id="deaa9-132">post</span></span>](../resources/post.md)|<span data-ttu-id="deaa9-133">A nova postagem que está sendo respondida.</span><span class="sxs-lookup"><span data-stu-id="deaa9-133">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="deaa9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="deaa9-134">Response</span></span>

<span data-ttu-id="deaa9-p104">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="deaa9-p104">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="deaa9-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="deaa9-137">Example</span></span>
<span data-ttu-id="deaa9-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="deaa9-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="deaa9-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="deaa9-139">Request</span></span>
<span data-ttu-id="deaa9-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="deaa9-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="deaa9-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="deaa9-141">HTTP</span></span>](#tab/http)
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
        "@odata.type": "#microsoft.graph.fileAttachment",
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
# <a name="c"></a>[<span data-ttu-id="deaa9-142">C#</span><span class="sxs-lookup"><span data-stu-id="deaa9-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="deaa9-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="deaa9-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="deaa9-144">Java</span><span class="sxs-lookup"><span data-stu-id="deaa9-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="deaa9-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="deaa9-145">Response</span></span>
<span data-ttu-id="deaa9-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="deaa9-146">Here is an example of the response.</span></span>
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

