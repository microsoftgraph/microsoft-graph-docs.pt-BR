---
title: 'post: forward'
description: 'Encaminhe uma postagem para um destinatário. Você pode especificar a conversa primária e o thread na solicitação, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 50090aa86676b544e93818d5b0058517c58b85fe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445160"
---
# <a name="post-forward"></a><span data-ttu-id="0be54-104">post: forward</span><span class="sxs-lookup"><span data-stu-id="0be54-104">post: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0be54-p102">Encaminhe uma postagem para um destinatário. Você pode especificar a conversa pai e o thread na solicitação ou pode especificar apenas o thread pai, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="0be54-p102">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0be54-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0be54-107">Permissions</span></span>
<span data-ttu-id="0be54-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0be54-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0be54-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0be54-110">Permission type</span></span>      | <span data-ttu-id="0be54-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0be54-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0be54-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0be54-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0be54-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be54-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0be54-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0be54-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0be54-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0be54-115">Not supported.</span></span>    |
|<span data-ttu-id="0be54-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0be54-116">Application</span></span> | <span data-ttu-id="0be54-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be54-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0be54-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0be54-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="0be54-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0be54-119">Request headers</span></span>
| <span data-ttu-id="0be54-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0be54-120">Header</span></span>       | <span data-ttu-id="0be54-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0be54-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0be54-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0be54-122">Authorization</span></span>  | <span data-ttu-id="0be54-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0be54-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0be54-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0be54-125">Request body</span></span>
<span data-ttu-id="0be54-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0be54-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0be54-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0be54-127">Parameter</span></span>    | <span data-ttu-id="0be54-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="0be54-128">Type</span></span>   |<span data-ttu-id="0be54-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="0be54-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0be54-130">comment</span><span class="sxs-lookup"><span data-stu-id="0be54-130">comment</span></span>|<span data-ttu-id="0be54-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0be54-131">String</span></span>|<span data-ttu-id="0be54-132">Comentário opcional que é encaminhado com a postagem.</span><span class="sxs-lookup"><span data-stu-id="0be54-132">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="0be54-133">toRecipients</span><span class="sxs-lookup"><span data-stu-id="0be54-133">toRecipients</span></span>|<span data-ttu-id="0be54-134">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="0be54-134">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="0be54-135">Os destinatários aos quais os threads são encaminhados.</span><span class="sxs-lookup"><span data-stu-id="0be54-135">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="0be54-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0be54-136">Response</span></span>

<span data-ttu-id="0be54-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0be54-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0be54-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0be54-139">Example</span></span>
<span data-ttu-id="0be54-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0be54-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0be54-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0be54-141">Request</span></span>
<span data-ttu-id="0be54-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0be54-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0be54-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="0be54-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0be54-144">C#</span><span class="sxs-lookup"><span data-stu-id="0be54-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0be54-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="0be54-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0be54-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0be54-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0be54-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0be54-147">Response</span></span>
<span data-ttu-id="0be54-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0be54-148">Here is an example of the response.</span></span>
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
