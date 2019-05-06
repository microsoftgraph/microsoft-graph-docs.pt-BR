---
title: Excluir educationCategory
description: Excluir uma categoria existente.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7e7f9d0682c1a279d448e82addb1434f93f2e0ec
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587396"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="969dc-103">Excluir educationCategory</span><span class="sxs-lookup"><span data-stu-id="969dc-103">Delete educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="969dc-104">Excluir uma categoria existente.</span><span class="sxs-lookup"><span data-stu-id="969dc-104">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="969dc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="969dc-105">Permissions</span></span>
<span data-ttu-id="969dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="969dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="969dc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="969dc-108">Permission type</span></span>      | <span data-ttu-id="969dc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="969dc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="969dc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="969dc-110">Delegated (work or school account)</span></span>| <span data-ttu-id="969dc-111">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="969dc-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="969dc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="969dc-112">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="969dc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="969dc-113">Not Supported.</span></span> |
|<span data-ttu-id="969dc-114">Application</span><span class="sxs-lookup"><span data-stu-id="969dc-114">Application</span></span> | <span data-ttu-id="969dc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="969dc-115">Not Supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="969dc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="969dc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/<id>/assignmentCategories/<id>
```
## <a name="request-headers"></a><span data-ttu-id="969dc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="969dc-117">Request headers</span></span>
| <span data-ttu-id="969dc-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="969dc-118">Header</span></span>       | <span data-ttu-id="969dc-119">Valor</span><span class="sxs-lookup"><span data-stu-id="969dc-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="969dc-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="969dc-120">Authorization</span></span>  | <span data-ttu-id="969dc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="969dc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="969dc-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="969dc-123">Request body</span></span>
<span data-ttu-id="969dc-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="969dc-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="969dc-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="969dc-125">Response</span></span>
<span data-ttu-id="969dc-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="969dc-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="969dc-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="969dc-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="969dc-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="969dc-129">Request</span></span>
<span data-ttu-id="969dc-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="969dc-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
### <a name="response"></a><span data-ttu-id="969dc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="969dc-131">Response</span></span>
<span data-ttu-id="969dc-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="969dc-132">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="969dc-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="969dc-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="969dc-134">Basic</span><span class="sxs-lookup"><span data-stu-id="969dc-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationassignment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="969dc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="969dc-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationassignment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationcategory-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationcategory-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
