---
title: Excluir educationUser
description: Exclua um usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bc1946d9155227df0bd1d6c7489161faf9c5c4b6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459451"
---
# <a name="delete-educationuser"></a><span data-ttu-id="47171-103">Excluir educationUser</span><span class="sxs-lookup"><span data-stu-id="47171-103">Delete educationUser</span></span>

<span data-ttu-id="47171-104">Exclua um usuário.</span><span class="sxs-lookup"><span data-stu-id="47171-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="47171-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="47171-105">Permissions</span></span>
<span data-ttu-id="47171-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47171-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47171-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47171-108">Permission type</span></span>      | <span data-ttu-id="47171-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47171-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47171-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47171-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="47171-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47171-111">Not supported.</span></span>  |
|<span data-ttu-id="47171-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47171-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="47171-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47171-113">Not supported.</span></span>  |
|<span data-ttu-id="47171-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47171-114">Application</span></span> | <span data-ttu-id="47171-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47171-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47171-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47171-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="47171-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47171-117">Request headers</span></span>
| <span data-ttu-id="47171-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47171-118">Header</span></span>       | <span data-ttu-id="47171-119">Valor</span><span class="sxs-lookup"><span data-stu-id="47171-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="47171-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="47171-120">Authorization</span></span>  | <span data-ttu-id="47171-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47171-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47171-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47171-123">Request body</span></span>
<span data-ttu-id="47171-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47171-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="47171-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="47171-125">Response</span></span>
<span data-ttu-id="47171-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47171-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47171-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47171-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47171-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47171-129">Request</span></span>
<span data-ttu-id="47171-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47171-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="47171-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="47171-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/users/{user-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="47171-132">C#</span><span class="sxs-lookup"><span data-stu-id="47171-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="47171-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="47171-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="47171-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="47171-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="47171-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="47171-135">Response</span></span>
<span data-ttu-id="47171-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="47171-136">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
