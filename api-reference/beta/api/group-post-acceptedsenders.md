---
title: Criar acceptedSender
description: Adicione um novo usuário ou grupo à lista acceptedSender.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 31a4dd44eb0f16b78dfe3b2cebe068ba825e6835
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681414"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="684eb-103">Criar acceptedSender</span><span class="sxs-lookup"><span data-stu-id="684eb-103">Create acceptedSender</span></span>

<span data-ttu-id="684eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="684eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="684eb-105">Adicione um novo usuário ou grupo à lista acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="684eb-105">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="684eb-p101">Especifique o usuário ou grupo em `@odata.id` no corpo da solicitação. Os usuários na lista de remetentes aceitos podem postar em conversas do grupo. Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="684eb-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="684eb-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="684eb-109">Permissions</span></span>
<span data-ttu-id="684eb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="684eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="684eb-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="684eb-112">Permission type</span></span>      | <span data-ttu-id="684eb-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="684eb-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="684eb-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="684eb-114">Delegated (work or school account)</span></span> | <span data-ttu-id="684eb-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="684eb-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="684eb-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="684eb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="684eb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="684eb-117">Not supported.</span></span>    |
|<span data-ttu-id="684eb-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="684eb-118">Application</span></span> | <span data-ttu-id="684eb-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="684eb-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="684eb-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="684eb-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="684eb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="684eb-121">Request headers</span></span>
| <span data-ttu-id="684eb-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="684eb-122">Header</span></span>       | <span data-ttu-id="684eb-123">Valor</span><span class="sxs-lookup"><span data-stu-id="684eb-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="684eb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="684eb-124">Authorization</span></span>  | <span data-ttu-id="684eb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="684eb-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="684eb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="684eb-127">Request body</span></span>
<span data-ttu-id="684eb-128">No corpo da solicitação, forneça a id de um objeto de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="684eb-128">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="684eb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="684eb-129">Response</span></span>
<span data-ttu-id="684eb-130">Este método retorna o código de resposta `204 No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="684eb-130">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="684eb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="684eb-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="684eb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="684eb-132">Request</span></span>
<span data-ttu-id="684eb-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="684eb-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="684eb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="684eb-134">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="684eb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="684eb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-acceptedsender-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="684eb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="684eb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-acceptedsender-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="684eb-137">C#</span><span class="sxs-lookup"><span data-stu-id="684eb-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-acceptedsender-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="684eb-138">Java</span><span class="sxs-lookup"><span data-stu-id="684eb-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-acceptedsender-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="684eb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="684eb-139">Response</span></span>
<span data-ttu-id="684eb-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="684eb-140">The following is an example of the response.</span></span>
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


