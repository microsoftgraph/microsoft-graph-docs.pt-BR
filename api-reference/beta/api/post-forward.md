---
title: 'post: forward'
description: 'Encaminhe uma postagem para um destinatário. Você pode especificar a conversa primária e o thread na solicitação, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2095e5a22ed15ff5444f424da475cda314925e37
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980429"
---
# <a name="post-forward"></a><span data-ttu-id="643c7-104">post: forward</span><span class="sxs-lookup"><span data-stu-id="643c7-104">post: forward</span></span>

<span data-ttu-id="643c7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="643c7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="643c7-p102">Encaminhe uma postagem para um destinatário. Você pode especificar a conversa pai e o thread na solicitação ou pode especificar apenas o thread pai, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="643c7-p102">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="643c7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="643c7-108">Permissions</span></span>
<span data-ttu-id="643c7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="643c7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="643c7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="643c7-111">Permission type</span></span>      | <span data-ttu-id="643c7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="643c7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="643c7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="643c7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="643c7-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="643c7-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="643c7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="643c7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="643c7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="643c7-116">Not supported.</span></span>    |
|<span data-ttu-id="643c7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="643c7-117">Application</span></span> | <span data-ttu-id="643c7-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="643c7-118">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="643c7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="643c7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="643c7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="643c7-120">Request headers</span></span>
| <span data-ttu-id="643c7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="643c7-121">Header</span></span>       | <span data-ttu-id="643c7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="643c7-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="643c7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="643c7-123">Authorization</span></span>  | <span data-ttu-id="643c7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="643c7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="643c7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="643c7-126">Request body</span></span>
<span data-ttu-id="643c7-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="643c7-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="643c7-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="643c7-128">Parameter</span></span>    | <span data-ttu-id="643c7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="643c7-129">Type</span></span>   |<span data-ttu-id="643c7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="643c7-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="643c7-131">comment</span><span class="sxs-lookup"><span data-stu-id="643c7-131">comment</span></span>|<span data-ttu-id="643c7-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="643c7-132">String</span></span>|<span data-ttu-id="643c7-133">Comentário opcional que é encaminhado com a postagem.</span><span class="sxs-lookup"><span data-stu-id="643c7-133">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="643c7-134">toRecipients</span><span class="sxs-lookup"><span data-stu-id="643c7-134">toRecipients</span></span>|<span data-ttu-id="643c7-135">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="643c7-135">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="643c7-136">Os destinatários aos quais os threads são encaminhados.</span><span class="sxs-lookup"><span data-stu-id="643c7-136">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="643c7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="643c7-137">Response</span></span>

<span data-ttu-id="643c7-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="643c7-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="643c7-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="643c7-140">Example</span></span>
<span data-ttu-id="643c7-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="643c7-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="643c7-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="643c7-142">Request</span></span>
<span data-ttu-id="643c7-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="643c7-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="643c7-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="643c7-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="643c7-145">C#</span><span class="sxs-lookup"><span data-stu-id="643c7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="643c7-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="643c7-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="643c7-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="643c7-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="643c7-148">Java</span><span class="sxs-lookup"><span data-stu-id="643c7-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="643c7-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="643c7-149">Response</span></span>
<span data-ttu-id="643c7-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="643c7-150">Here is an example of the response.</span></span>
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
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


