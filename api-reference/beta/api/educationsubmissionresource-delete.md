---
title: Excluir educationSubmissionResource
description: Exclui um recurso do envio. Isso só pode ser feito pelo aluno. Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada após a exclusão da cópia atual.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f989c1854ee952b53bfd5df123e425bd25a0d2ca
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664752"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="a5e0e-105">Excluir educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="a5e0e-105">Delete educationSubmissionResource</span></span>

<span data-ttu-id="a5e0e-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5e0e-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5e0e-107">Exclui um recurso do envio.</span><span class="sxs-lookup"><span data-stu-id="a5e0e-107">Deletes a resource from the submission.</span></span> <span data-ttu-id="a5e0e-108">Isso só pode ser feito pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="a5e0e-108">This can only be done by the student.</span></span> <span data-ttu-id="a5e0e-109">Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada após a exclusão da cópia atual.</span><span class="sxs-lookup"><span data-stu-id="a5e0e-109">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="a5e0e-110">Isso permite que você "redefina" o recurso para seu estado original.</span><span class="sxs-lookup"><span data-stu-id="a5e0e-110">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="a5e0e-111">Se o recurso não foi copiado da atribuição, mas foi adicionado do aluno, o recurso será simplesmente excluído.</span><span class="sxs-lookup"><span data-stu-id="a5e0e-111">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5e0e-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5e0e-112">Permissions</span></span>
<span data-ttu-id="a5e0e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5e0e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5e0e-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5e0e-115">Permission type</span></span>      | <span data-ttu-id="a5e0e-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5e0e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5e0e-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5e0e-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="a5e0e-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5e0e-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="a5e0e-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5e0e-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a5e0e-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5e0e-120">Not supported.</span></span>  |
|<span data-ttu-id="a5e0e-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5e0e-121">Application</span></span> | <span data-ttu-id="a5e0e-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5e0e-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a5e0e-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5e0e-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a5e0e-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e0e-124">Request headers</span></span>
| <span data-ttu-id="a5e0e-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5e0e-125">Header</span></span>       | <span data-ttu-id="a5e0e-126">Valor</span><span class="sxs-lookup"><span data-stu-id="a5e0e-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a5e0e-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5e0e-127">Authorization</span></span>  | <span data-ttu-id="a5e0e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5e0e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5e0e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e0e-130">Request body</span></span>
<span data-ttu-id="a5e0e-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5e0e-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a5e0e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5e0e-132">Response</span></span>
<span data-ttu-id="a5e0e-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5e0e-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5e0e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5e0e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5e0e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e0e-136">Request</span></span>
<span data-ttu-id="a5e0e-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5e0e-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5e0e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5e0e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
# <a name="c"></a>[<span data-ttu-id="a5e0e-139">C#</span><span class="sxs-lookup"><span data-stu-id="a5e0e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationsubmissionresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5e0e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5e0e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationsubmissionresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5e0e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5e0e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationsubmissionresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5e0e-142">Java</span><span class="sxs-lookup"><span data-stu-id="a5e0e-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationsubmissionresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a5e0e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5e0e-143">Response</span></span>
<span data-ttu-id="a5e0e-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a5e0e-144">The following is an example of the response.</span></span> 

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


