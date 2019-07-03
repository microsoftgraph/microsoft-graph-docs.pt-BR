---
title: Criar acceptedSender
description: Adicione um novo usuário ou grupo à lista acceptedSender.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: bfa5e6f67475fadde7d5a1c815ba231cf534cbe5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440285"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="8bf9d-103">Criar acceptedSender</span><span class="sxs-lookup"><span data-stu-id="8bf9d-103">Create acceptedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bf9d-104">Adicione um novo usuário ou grupo à lista acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="8bf9d-104">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="8bf9d-p101">Especifique o usuário ou grupo em `@odata.id` no corpo da solicitação. Os usuários na lista de remetentes aceitos podem postar em conversas do grupo. Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="8bf9d-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bf9d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8bf9d-108">Permissions</span></span>
<span data-ttu-id="8bf9d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bf9d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bf9d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bf9d-111">Permission type</span></span>      | <span data-ttu-id="8bf9d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8bf9d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bf9d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bf9d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8bf9d-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bf9d-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8bf9d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bf9d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bf9d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bf9d-116">Not supported.</span></span>    |
|<span data-ttu-id="8bf9d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bf9d-117">Application</span></span> | <span data-ttu-id="8bf9d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bf9d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bf9d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bf9d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="8bf9d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bf9d-120">Request headers</span></span>
| <span data-ttu-id="8bf9d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8bf9d-121">Header</span></span>       | <span data-ttu-id="8bf9d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8bf9d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8bf9d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bf9d-123">Authorization</span></span>  | <span data-ttu-id="8bf9d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bf9d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8bf9d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bf9d-126">Request body</span></span>
<span data-ttu-id="8bf9d-127">No corpo da solicitação, forneça a id de um objeto de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="8bf9d-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="8bf9d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bf9d-128">Response</span></span>
<span data-ttu-id="8bf9d-129">Este método retorna o código de resposta `204 No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8bf9d-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bf9d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8bf9d-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8bf9d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bf9d-131">Request</span></span>
<span data-ttu-id="8bf9d-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8bf9d-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8bf9d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bf9d-133">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8bf9d-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="8bf9d-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-acceptedsender-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8bf9d-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8bf9d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-acceptedsender-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8bf9d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bf9d-136">Response</span></span>
<span data-ttu-id="8bf9d-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8bf9d-137">The following is an example of the response.</span></span>
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
