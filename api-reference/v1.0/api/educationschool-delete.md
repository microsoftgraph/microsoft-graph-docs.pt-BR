---
title: Excluir educationSchool
description: Exclua uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b7c3bfe0d2a99fe7fe72e6d6303e66d81191650a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445195"
---
# <a name="delete-educationschool"></a><span data-ttu-id="13d5c-103">Excluir educationSchool</span><span class="sxs-lookup"><span data-stu-id="13d5c-103">Delete educationSchool</span></span>

<span data-ttu-id="13d5c-104">Exclua uma escola.</span><span class="sxs-lookup"><span data-stu-id="13d5c-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="13d5c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="13d5c-105">Permissions</span></span>
<span data-ttu-id="13d5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13d5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13d5c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13d5c-108">Permission type</span></span>      | <span data-ttu-id="13d5c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13d5c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13d5c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13d5c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="13d5c-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13d5c-111">Not supported.</span></span>  |
|<span data-ttu-id="13d5c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13d5c-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="13d5c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13d5c-113">Not supported.</span></span>  |
|<span data-ttu-id="13d5c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13d5c-114">Application</span></span> | <span data-ttu-id="13d5c-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13d5c-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="13d5c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13d5c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="13d5c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13d5c-117">Request headers</span></span>
| <span data-ttu-id="13d5c-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="13d5c-118">Header</span></span>       | <span data-ttu-id="13d5c-119">Valor</span><span class="sxs-lookup"><span data-stu-id="13d5c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="13d5c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="13d5c-120">Authorization</span></span>  | <span data-ttu-id="13d5c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13d5c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="13d5c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13d5c-123">Request body</span></span>
<span data-ttu-id="13d5c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13d5c-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="13d5c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="13d5c-125">Response</span></span>
<span data-ttu-id="13d5c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13d5c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13d5c-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13d5c-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13d5c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13d5c-129">Request</span></span>
<span data-ttu-id="13d5c-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="13d5c-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="13d5c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="13d5c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="13d5c-132">C#</span><span class="sxs-lookup"><span data-stu-id="13d5c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="13d5c-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="13d5c-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="13d5c-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="13d5c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="13d5c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="13d5c-135">Response</span></span>
<span data-ttu-id="13d5c-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="13d5c-136">The following is an example of the response.</span></span> 

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
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
