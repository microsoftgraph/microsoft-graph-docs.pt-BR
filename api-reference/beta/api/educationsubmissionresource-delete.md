---
title: Excluir educationSubmissionResource
description: Exclui um recurso do envio. Isso só pode ser feito pelo aluno. Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada após a cópia atual ser excluída.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ece6960764051401f08889a0d21bb88c39835701
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441356"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="42ad6-105">Excluir educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="42ad6-105">Delete educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42ad6-106">Exclui um recurso do envio.</span><span class="sxs-lookup"><span data-stu-id="42ad6-106">Deletes a resource from the submission.</span></span> <span data-ttu-id="42ad6-107">Isso só pode ser feito pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="42ad6-107">This can only be done by the student.</span></span> <span data-ttu-id="42ad6-108">Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada após a cópia atual ser excluída.</span><span class="sxs-lookup"><span data-stu-id="42ad6-108">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="42ad6-109">Isso permite que você "Redefina" o recurso para seu estado original.</span><span class="sxs-lookup"><span data-stu-id="42ad6-109">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="42ad6-110">Se o recurso não foi copiado da atribuição, mas foi adicionado do aluno, o recurso será simplesmente excluído.</span><span class="sxs-lookup"><span data-stu-id="42ad6-110">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="42ad6-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="42ad6-111">Permissions</span></span>
<span data-ttu-id="42ad6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42ad6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42ad6-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42ad6-114">Permission type</span></span>      | <span data-ttu-id="42ad6-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42ad6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42ad6-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42ad6-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="42ad6-117">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42ad6-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="42ad6-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42ad6-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="42ad6-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42ad6-119">Not supported.</span></span>  |
|<span data-ttu-id="42ad6-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42ad6-120">Application</span></span> | <span data-ttu-id="42ad6-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42ad6-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="42ad6-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42ad6-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="42ad6-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42ad6-123">Request headers</span></span>
| <span data-ttu-id="42ad6-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42ad6-124">Header</span></span>       | <span data-ttu-id="42ad6-125">Valor</span><span class="sxs-lookup"><span data-stu-id="42ad6-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="42ad6-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="42ad6-126">Authorization</span></span>  | <span data-ttu-id="42ad6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42ad6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="42ad6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42ad6-129">Request body</span></span>
<span data-ttu-id="42ad6-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42ad6-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="42ad6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="42ad6-131">Response</span></span>
<span data-ttu-id="42ad6-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42ad6-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42ad6-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42ad6-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42ad6-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42ad6-135">Request</span></span>
<span data-ttu-id="42ad6-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="42ad6-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="42ad6-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="42ad6-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="42ad6-138">C#</span><span class="sxs-lookup"><span data-stu-id="42ad6-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationsubmissionresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="42ad6-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="42ad6-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationsubmissionresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="42ad6-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="42ad6-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationsubmissionresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="42ad6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="42ad6-141">Response</span></span>
<span data-ttu-id="42ad6-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="42ad6-142">The following is an example of the response.</span></span> 

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
  "description": "Delete educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
