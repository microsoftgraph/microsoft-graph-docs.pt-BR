---
title: Criar acceptedSender
description: Adicione um novo usuário ou grupo à lista acceptedSender.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 56b874861469cdc5a47fa29b0a4af6ad4605e3e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418936"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="cdbde-103">Criar acceptedSender</span><span class="sxs-lookup"><span data-stu-id="cdbde-103">Create acceptedSender</span></span>

<span data-ttu-id="cdbde-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cdbde-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdbde-105">Adicione um novo usuário ou grupo à lista acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="cdbde-105">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="cdbde-p101">Especifique o usuário ou grupo em `@odata.id` no corpo da solicitação. Os usuários na lista de remetentes aceitos podem postar em conversas do grupo. Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="cdbde-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdbde-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="cdbde-109">Permissions</span></span>
<span data-ttu-id="cdbde-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdbde-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdbde-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdbde-112">Permission type</span></span>      | <span data-ttu-id="cdbde-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cdbde-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdbde-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdbde-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cdbde-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdbde-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cdbde-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdbde-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdbde-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdbde-117">Not supported.</span></span>    |
|<span data-ttu-id="cdbde-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdbde-118">Application</span></span> | <span data-ttu-id="cdbde-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdbde-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdbde-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdbde-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="cdbde-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdbde-121">Request headers</span></span>
| <span data-ttu-id="cdbde-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cdbde-122">Header</span></span>       | <span data-ttu-id="cdbde-123">Valor</span><span class="sxs-lookup"><span data-stu-id="cdbde-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cdbde-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdbde-124">Authorization</span></span>  | <span data-ttu-id="cdbde-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdbde-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cdbde-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdbde-127">Request body</span></span>
<span data-ttu-id="cdbde-128">No corpo da solicitação, forneça a id de um objeto de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="cdbde-128">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="cdbde-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdbde-129">Response</span></span>
<span data-ttu-id="cdbde-130">Este método retorna o código de resposta `204 No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cdbde-130">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdbde-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdbde-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cdbde-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdbde-132">Request</span></span>
<span data-ttu-id="cdbde-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdbde-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cdbde-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdbde-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_acceptedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```
# <a name="javascript"></a>[<span data-ttu-id="cdbde-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdbde-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-acceptedsender-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdbde-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdbde-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-acceptedsender-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="cdbde-137">C#</span><span class="sxs-lookup"><span data-stu-id="cdbde-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-acceptedsender-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cdbde-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdbde-138">Response</span></span>
<span data-ttu-id="cdbde-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cdbde-139">The following is an example of the response.</span></span>
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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
