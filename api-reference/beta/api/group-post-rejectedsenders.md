---
title: Criar rejectedSender
description: Adiciona um novo usuário ou grupo à lista rejectedSender.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 78574fbf0d739075da252e1794c0c1c5f63df295
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681347"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="1b03a-103">Criar rejectedSender</span><span class="sxs-lookup"><span data-stu-id="1b03a-103">Create rejectedSender</span></span>

<span data-ttu-id="1b03a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b03a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b03a-105">Adiciona um novo usuário ou grupo à lista rejectedSender.</span><span class="sxs-lookup"><span data-stu-id="1b03a-105">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="1b03a-p101">Especifique o usuário ou grupo em `@odata.id` no corpo da solicitação. Os usuários na lista de remetentes rejeitados não podem postar em conversas do grupo (identificado na URL da solicitação POST). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="1b03a-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b03a-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b03a-109">Permissions</span></span>
<span data-ttu-id="1b03a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b03a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b03a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b03a-112">Permission type</span></span>      | <span data-ttu-id="1b03a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b03a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b03a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b03a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1b03a-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b03a-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1b03a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b03a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b03a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b03a-117">Not supported.</span></span>    |
|<span data-ttu-id="1b03a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b03a-118">Application</span></span> | <span data-ttu-id="1b03a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b03a-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b03a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b03a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="1b03a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b03a-121">Request headers</span></span>
| <span data-ttu-id="1b03a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b03a-122">Header</span></span>       | <span data-ttu-id="1b03a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1b03a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1b03a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b03a-124">Authorization</span></span>  | <span data-ttu-id="1b03a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b03a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1b03a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b03a-127">Request body</span></span>
<span data-ttu-id="1b03a-128">No corpo da solicitação, forneça a id de um objeto de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="1b03a-128">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="1b03a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b03a-129">Response</span></span>
<span data-ttu-id="1b03a-130">Este método retorna o código de resposta `204 No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1b03a-130">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b03a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b03a-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1b03a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b03a-132">Request</span></span>
<span data-ttu-id="1b03a-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b03a-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b03a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b03a-134">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="1b03a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b03a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-rejectedsender-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b03a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b03a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-rejectedsender-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="1b03a-137">C#</span><span class="sxs-lookup"><span data-stu-id="1b03a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-rejectedsender-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b03a-138">Java</span><span class="sxs-lookup"><span data-stu-id="1b03a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-rejectedsender-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1b03a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b03a-139">Response</span></span>
<span data-ttu-id="1b03a-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1b03a-140">The following is an example of the response.</span></span>
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


