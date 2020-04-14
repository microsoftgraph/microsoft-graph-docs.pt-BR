---
title: Criar rejectedSender
description: Adiciona um novo usuário ou grupo à lista rejectedSender.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1ac6c8f6a75ff900630bbd27047d547566335318
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43396421"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="fc64f-103">Criar rejectedSender</span><span class="sxs-lookup"><span data-stu-id="fc64f-103">Create rejectedSender</span></span>

<span data-ttu-id="fc64f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc64f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc64f-105">Adiciona um novo usuário ou grupo à lista rejectedSender.</span><span class="sxs-lookup"><span data-stu-id="fc64f-105">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="fc64f-p101">Especifique o usuário ou grupo em `@odata.id` no corpo da solicitação. Os usuários na lista de remetentes rejeitados não podem postar em conversas do grupo (identificado na URL da solicitação POST). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="fc64f-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc64f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc64f-109">Permissions</span></span>
<span data-ttu-id="fc64f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc64f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc64f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc64f-112">Permission type</span></span>      | <span data-ttu-id="fc64f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc64f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc64f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc64f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fc64f-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc64f-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fc64f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc64f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc64f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc64f-117">Not supported.</span></span>    |
|<span data-ttu-id="fc64f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc64f-118">Application</span></span> | <span data-ttu-id="fc64f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc64f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc64f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc64f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="fc64f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc64f-121">Request headers</span></span>
| <span data-ttu-id="fc64f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc64f-122">Header</span></span>       | <span data-ttu-id="fc64f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="fc64f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fc64f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc64f-124">Authorization</span></span>  | <span data-ttu-id="fc64f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc64f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fc64f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc64f-127">Request body</span></span>
<span data-ttu-id="fc64f-128">No corpo da solicitação, forneça a id de um objeto de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="fc64f-128">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="fc64f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc64f-129">Response</span></span>
<span data-ttu-id="fc64f-130">Este método retorna o código de resposta `204 No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fc64f-130">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc64f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc64f-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fc64f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc64f-132">Request</span></span>
<span data-ttu-id="fc64f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc64f-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc64f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc64f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_rejectedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```
# <a name="javascript"></a>[<span data-ttu-id="fc64f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc64f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-rejectedsender-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc64f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc64f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-rejectedsender-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="fc64f-137">C#</span><span class="sxs-lookup"><span data-stu-id="fc64f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-rejectedsender-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fc64f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc64f-138">Response</span></span>
<span data-ttu-id="fc64f-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fc64f-139">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
