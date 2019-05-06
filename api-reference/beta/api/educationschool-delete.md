---
title: Excluir educationSchool
description: Exclua uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c84bde3d7309af8b4d6ef901d43d323b08ac5155
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33588023"
---
# <a name="delete-educationschool"></a><span data-ttu-id="b8c5d-103">Excluir educationSchool</span><span class="sxs-lookup"><span data-stu-id="b8c5d-103">Delete educationSchool</span></span>

<span data-ttu-id="b8c5d-104">Exclua uma escola.</span><span class="sxs-lookup"><span data-stu-id="b8c5d-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8c5d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8c5d-105">Permissions</span></span>
<span data-ttu-id="b8c5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8c5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8c5d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8c5d-108">Permission type</span></span>      | <span data-ttu-id="b8c5d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8c5d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8c5d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8c5d-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="b8c5d-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8c5d-111">Not supported.</span></span>  |
|<span data-ttu-id="b8c5d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8c5d-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b8c5d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8c5d-113">Not supported.</span></span>  |
|<span data-ttu-id="b8c5d-114">Application</span><span class="sxs-lookup"><span data-stu-id="b8c5d-114">Application</span></span> | <span data-ttu-id="b8c5d-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8c5d-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b8c5d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8c5d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b8c5d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8c5d-117">Request headers</span></span>
| <span data-ttu-id="b8c5d-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8c5d-118">Header</span></span>       | <span data-ttu-id="b8c5d-119">Valor</span><span class="sxs-lookup"><span data-stu-id="b8c5d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8c5d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8c5d-120">Authorization</span></span>  | <span data-ttu-id="b8c5d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8c5d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8c5d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8c5d-123">Request body</span></span>
<span data-ttu-id="b8c5d-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8c5d-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b8c5d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8c5d-125">Response</span></span>
<span data-ttu-id="b8c5d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8c5d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8c5d-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8c5d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8c5d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8c5d-129">Request</span></span>
<span data-ttu-id="b8c5d-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8c5d-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
##### <a name="response"></a><span data-ttu-id="b8c5d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8c5d-131">Response</span></span>
<span data-ttu-id="b8c5d-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8c5d-132">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b8c5d-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b8c5d-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b8c5d-134">Basic</span><span class="sxs-lookup"><span data-stu-id="b8c5d-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationschool-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8c5d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8c5d-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationschool-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationschool-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationschool-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
