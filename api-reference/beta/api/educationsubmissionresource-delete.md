---
title: Excluir educationSubmissionResource
description: Exclui um recurso do envio. Isso só pode ser feito pelo aluno. Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada após a cópia atual ser excluída.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 86cff1730950c8d587d516a24b458f636e6e873e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259462"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="3b34e-105">Excluir educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="3b34e-105">Delete educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b34e-106">Exclui um recurso do envio.</span><span class="sxs-lookup"><span data-stu-id="3b34e-106">Deletes a resource from the submission.</span></span> <span data-ttu-id="3b34e-107">Isso só pode ser feito pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="3b34e-107">This can only be done by the student.</span></span> <span data-ttu-id="3b34e-108">Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada após a cópia atual ser excluída.</span><span class="sxs-lookup"><span data-stu-id="3b34e-108">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="3b34e-109">Isso permite que você "Redefina" o recurso para seu estado original.</span><span class="sxs-lookup"><span data-stu-id="3b34e-109">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="3b34e-110">Se o recurso não foi copiado da atribuição, mas foi adicionado do aluno, o recurso será simplesmente excluído.</span><span class="sxs-lookup"><span data-stu-id="3b34e-110">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b34e-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b34e-111">Permissions</span></span>
<span data-ttu-id="3b34e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b34e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b34e-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b34e-114">Permission type</span></span>      | <span data-ttu-id="3b34e-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b34e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b34e-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b34e-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="3b34e-117">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b34e-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="3b34e-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b34e-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3b34e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b34e-119">Not supported.</span></span>  |
|<span data-ttu-id="3b34e-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b34e-120">Application</span></span> | <span data-ttu-id="3b34e-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b34e-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3b34e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b34e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="3b34e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b34e-123">Request headers</span></span>
| <span data-ttu-id="3b34e-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b34e-124">Header</span></span>       | <span data-ttu-id="3b34e-125">Valor</span><span class="sxs-lookup"><span data-stu-id="3b34e-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3b34e-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b34e-126">Authorization</span></span>  | <span data-ttu-id="3b34e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b34e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3b34e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b34e-129">Request body</span></span>
<span data-ttu-id="3b34e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b34e-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3b34e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b34e-131">Response</span></span>
<span data-ttu-id="3b34e-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b34e-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b34e-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b34e-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b34e-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b34e-135">Request</span></span>
<span data-ttu-id="3b34e-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b34e-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="3b34e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b34e-137">Response</span></span>
<span data-ttu-id="3b34e-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b34e-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3b34e-139">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="3b34e-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3b34e-140">C#</span><span class="sxs-lookup"><span data-stu-id="3b34e-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationsubmissionresource-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3b34e-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="3b34e-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationsubmissionresource-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3b34e-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3b34e-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_educationsubmissionresource-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmissionresource-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationsubmissionresource-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsubmissionresource-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
