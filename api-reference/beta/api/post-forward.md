---
title: 'post: forward'
description: 'Encaminhe uma postagem para um destinatário. Você pode especificar a conversa primária e o thread na solicitação, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ff8bbab2bf23622deeefd3aaa8cd163186f834d8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455472"
---
# <a name="post-forward"></a><span data-ttu-id="a080c-104">post: forward</span><span class="sxs-lookup"><span data-stu-id="a080c-104">post: forward</span></span>

<span data-ttu-id="a080c-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a080c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a080c-p102">Encaminhe uma postagem para um destinatário. Você pode especificar a conversa pai e o thread na solicitação ou pode especificar apenas o thread pai, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="a080c-p102">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a080c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a080c-108">Permissions</span></span>
<span data-ttu-id="a080c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a080c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a080c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a080c-111">Permission type</span></span>      | <span data-ttu-id="a080c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a080c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a080c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a080c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a080c-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a080c-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a080c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a080c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a080c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a080c-116">Not supported.</span></span>    |
|<span data-ttu-id="a080c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a080c-117">Application</span></span> | <span data-ttu-id="a080c-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a080c-118">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a080c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a080c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="a080c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a080c-120">Request headers</span></span>
| <span data-ttu-id="a080c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a080c-121">Header</span></span>       | <span data-ttu-id="a080c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a080c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a080c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a080c-123">Authorization</span></span>  | <span data-ttu-id="a080c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a080c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a080c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a080c-126">Request body</span></span>
<span data-ttu-id="a080c-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a080c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a080c-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a080c-128">Parameter</span></span>    | <span data-ttu-id="a080c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a080c-129">Type</span></span>   |<span data-ttu-id="a080c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a080c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a080c-131">comment</span><span class="sxs-lookup"><span data-stu-id="a080c-131">comment</span></span>|<span data-ttu-id="a080c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a080c-132">String</span></span>|<span data-ttu-id="a080c-133">Comentário opcional que é encaminhado com a postagem.</span><span class="sxs-lookup"><span data-stu-id="a080c-133">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="a080c-134">toRecipients</span><span class="sxs-lookup"><span data-stu-id="a080c-134">toRecipients</span></span>|<span data-ttu-id="a080c-135">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="a080c-135">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="a080c-136">Os destinatários aos quais os threads são encaminhados.</span><span class="sxs-lookup"><span data-stu-id="a080c-136">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="a080c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a080c-137">Response</span></span>

<span data-ttu-id="a080c-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a080c-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a080c-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a080c-140">Example</span></span>
<span data-ttu-id="a080c-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a080c-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a080c-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a080c-142">Request</span></span>
<span data-ttu-id="a080c-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a080c-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a080c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="a080c-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a080c-145">C#</span><span class="sxs-lookup"><span data-stu-id="a080c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a080c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a080c-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a080c-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a080c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a080c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a080c-148">Response</span></span>
<span data-ttu-id="a080c-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a080c-149">Here is an example of the response.</span></span>
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
