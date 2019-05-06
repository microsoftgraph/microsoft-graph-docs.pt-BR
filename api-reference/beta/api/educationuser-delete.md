---
title: Excluir educationUser
description: Exclua um usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 703ecc41cead8039ea3609de7afec558d6ae5b87
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587098"
---
# <a name="delete-educationuser"></a><span data-ttu-id="0c01c-103">Excluir educationUser</span><span class="sxs-lookup"><span data-stu-id="0c01c-103">Delete educationUser</span></span>

<span data-ttu-id="0c01c-104">Exclua um usuário.</span><span class="sxs-lookup"><span data-stu-id="0c01c-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="0c01c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c01c-105">Permissions</span></span>
<span data-ttu-id="0c01c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c01c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c01c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c01c-108">Permission type</span></span>      | <span data-ttu-id="0c01c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c01c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c01c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c01c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="0c01c-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c01c-111">Not supported.</span></span>  |
|<span data-ttu-id="0c01c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c01c-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0c01c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c01c-113">Not supported.</span></span>  |
|<span data-ttu-id="0c01c-114">Application</span><span class="sxs-lookup"><span data-stu-id="0c01c-114">Application</span></span> | <span data-ttu-id="0c01c-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c01c-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c01c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c01c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0c01c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c01c-117">Request headers</span></span>
| <span data-ttu-id="0c01c-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c01c-118">Header</span></span>       | <span data-ttu-id="0c01c-119">Valor</span><span class="sxs-lookup"><span data-stu-id="0c01c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0c01c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c01c-120">Authorization</span></span>  | <span data-ttu-id="0c01c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c01c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0c01c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c01c-123">Request body</span></span>
<span data-ttu-id="0c01c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0c01c-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0c01c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c01c-125">Response</span></span>
<span data-ttu-id="0c01c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c01c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c01c-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c01c-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c01c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c01c-129">Request</span></span>
<span data-ttu-id="0c01c-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c01c-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="0c01c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c01c-131">Response</span></span>
<span data-ttu-id="0c01c-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0c01c-132">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0c01c-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="0c01c-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0c01c-134">Basic</span><span class="sxs-lookup"><span data-stu-id="0c01c-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c01c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c01c-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationuser-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationuser-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationuser-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
