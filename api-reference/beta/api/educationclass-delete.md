---
title: Excluir educationClass
description: Exclua uma aula. Como uma aula também é um grupo universal, excluir uma aula exclui o grupo.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: b918b97dfc45af79f0df9708889f4fc763816023
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587391"
---
# <a name="delete-educationclass"></a><span data-ttu-id="fc2c2-104">Excluir educationClass</span><span class="sxs-lookup"><span data-stu-id="fc2c2-104">Delete educationClass</span></span>

<span data-ttu-id="fc2c2-105">Exclua uma aula.</span><span class="sxs-lookup"><span data-stu-id="fc2c2-105">Delete a class.</span></span> <span data-ttu-id="fc2c2-106">Como uma aula também é um grupo universal, excluir uma aula exclui o grupo.</span><span class="sxs-lookup"><span data-stu-id="fc2c2-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc2c2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc2c2-107">Permissions</span></span>
<span data-ttu-id="fc2c2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc2c2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc2c2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc2c2-110">Permission type</span></span>      | <span data-ttu-id="fc2c2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc2c2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc2c2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc2c2-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="fc2c2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc2c2-113">Not supported.</span></span>  |
|<span data-ttu-id="fc2c2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc2c2-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fc2c2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc2c2-115">Not supported.</span></span>  |
|<span data-ttu-id="fc2c2-116">Application</span><span class="sxs-lookup"><span data-stu-id="fc2c2-116">Application</span></span> | <span data-ttu-id="fc2c2-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc2c2-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fc2c2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc2c2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="fc2c2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc2c2-119">Request headers</span></span>
| <span data-ttu-id="fc2c2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc2c2-120">Header</span></span>       | <span data-ttu-id="fc2c2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fc2c2-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fc2c2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc2c2-122">Authorization</span></span>  | <span data-ttu-id="fc2c2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc2c2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fc2c2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc2c2-125">Request body</span></span>
<span data-ttu-id="fc2c2-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc2c2-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="fc2c2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc2c2-127">Response</span></span>
<span data-ttu-id="fc2c2-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc2c2-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc2c2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc2c2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc2c2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc2c2-131">Request</span></span>
<span data-ttu-id="fc2c2-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc2c2-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
##### <a name="response"></a><span data-ttu-id="fc2c2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc2c2-133">Response</span></span>
<span data-ttu-id="fc2c2-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fc2c2-134">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fc2c2-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="fc2c2-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fc2c2-136">Basic</span><span class="sxs-lookup"><span data-stu-id="fc2c2-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationclass-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc2c2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc2c2-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationclass-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationclass-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationclass-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
