---
title: Criar rejectedSender
description: Adiciona um novo usuário ou grupo à lista rejectedSender.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: dc1b701a80a145ce0c8e119910f1d239e37ee1fc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953518"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="ae834-103">Criar rejectedSender</span><span class="sxs-lookup"><span data-stu-id="ae834-103">Create rejectedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae834-104">Adiciona um novo usuário ou grupo à lista rejectedSender.</span><span class="sxs-lookup"><span data-stu-id="ae834-104">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="ae834-p101">Especifique o usuário ou grupo em `@odata.id` no corpo da solicitação. Os usuários na lista de remetentes rejeitados não podem postar em conversas do grupo (identificado na URL da solicitação POST). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="ae834-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae834-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ae834-108">Permissions</span></span>
<span data-ttu-id="ae834-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae834-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae834-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae834-111">Permission type</span></span>      | <span data-ttu-id="ae834-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae834-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae834-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae834-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ae834-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae834-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ae834-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae834-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae834-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae834-116">Not supported.</span></span>    |
|<span data-ttu-id="ae834-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae834-117">Application</span></span> | <span data-ttu-id="ae834-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae834-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae834-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae834-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ae834-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae834-120">Request headers</span></span>
| <span data-ttu-id="ae834-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae834-121">Header</span></span>       | <span data-ttu-id="ae834-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ae834-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ae834-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae834-123">Authorization</span></span>  | <span data-ttu-id="ae834-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae834-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ae834-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae834-126">Request body</span></span>
<span data-ttu-id="ae834-127">No corpo da solicitação, forneça a id de um objeto de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="ae834-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="ae834-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae834-128">Response</span></span>
<span data-ttu-id="ae834-129">Este método retorna o código de resposta `204 No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae834-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae834-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae834-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ae834-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae834-131">Request</span></span>
<span data-ttu-id="ae834-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae834-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ae834-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae834-133">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ae834-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="ae834-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-rejectedsender-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ae834-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ae834-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-rejectedsender-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="ae834-136">C#</span><span class="sxs-lookup"><span data-stu-id="ae834-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-rejectedsender-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ae834-137">Java</span><span class="sxs-lookup"><span data-stu-id="ae834-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-rejectedsender-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ae834-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae834-138">Response</span></span>
<span data-ttu-id="ae834-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae834-139">The following is an example of the response.</span></span>
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
