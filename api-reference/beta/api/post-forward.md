---
title: 'post: forward'
description: 'Encaminhe uma postagem para um destinatário. Você pode especificar a conversa primária e o thread na solicitação, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: ac4f4f193d4b647fd97292f1aaa5d5b3bb88e1a1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33595252"
---
# <a name="post-forward"></a><span data-ttu-id="cf962-104">post: forward</span><span class="sxs-lookup"><span data-stu-id="cf962-104">post: forward</span></span>

<span data-ttu-id="cf962-p102">Encaminhe uma postagem para um destinatário. Você pode especificar a conversa pai e o thread na solicitação ou pode especificar apenas o thread pai, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="cf962-p102">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="cf962-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="cf962-107">Permissions</span></span>
<span data-ttu-id="cf962-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf962-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf962-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf962-110">Permission type</span></span>      | <span data-ttu-id="cf962-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf962-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf962-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf962-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cf962-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf962-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf962-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf962-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf962-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf962-115">Not supported.</span></span>    |
|<span data-ttu-id="cf962-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf962-116">Application</span></span> | <span data-ttu-id="cf962-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf962-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf962-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf962-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="cf962-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf962-119">Request headers</span></span>
| <span data-ttu-id="cf962-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf962-120">Header</span></span>       | <span data-ttu-id="cf962-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cf962-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cf962-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf962-122">Authorization</span></span>  | <span data-ttu-id="cf962-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf962-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf962-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf962-125">Request body</span></span>
<span data-ttu-id="cf962-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf962-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cf962-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cf962-127">Parameter</span></span>    | <span data-ttu-id="cf962-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf962-128">Type</span></span>   |<span data-ttu-id="cf962-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf962-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf962-130">comment</span><span class="sxs-lookup"><span data-stu-id="cf962-130">comment</span></span>|<span data-ttu-id="cf962-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf962-131">String</span></span>|<span data-ttu-id="cf962-132">Comentário opcional que é encaminhado com a postagem.</span><span class="sxs-lookup"><span data-stu-id="cf962-132">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="cf962-133">toRecipients</span><span class="sxs-lookup"><span data-stu-id="cf962-133">toRecipients</span></span>|<span data-ttu-id="cf962-134">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="cf962-134">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="cf962-135">Os destinatários aos quais os threads são encaminhados.</span><span class="sxs-lookup"><span data-stu-id="cf962-135">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="cf962-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf962-136">Response</span></span>

<span data-ttu-id="cf962-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf962-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf962-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf962-139">Example</span></span>
<span data-ttu-id="cf962-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="cf962-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cf962-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf962-141">Request</span></span>
<span data-ttu-id="cf962-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf962-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/forward
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

##### <a name="response"></a><span data-ttu-id="cf962-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf962-143">Response</span></span>
<span data-ttu-id="cf962-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf962-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cf962-145">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="cf962-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cf962-146">Basic</span><span class="sxs-lookup"><span data-stu-id="cf962-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_forward-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cf962-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf962-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_forward-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/post-forward.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/post-forward.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
