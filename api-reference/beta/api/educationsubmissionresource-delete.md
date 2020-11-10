---
title: Excluir educationSubmissionResource
description: Exclui um recurso do envio. Isso só pode ser feito pelo aluno. Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada após a cópia atual ser excluída.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4dc8b2970bf6cf241c93934593d0424d538fc01a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955397"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="412d7-105">Excluir educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="412d7-105">Delete educationSubmissionResource</span></span>

<span data-ttu-id="412d7-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="412d7-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="412d7-107">Exclui um recurso do envio.</span><span class="sxs-lookup"><span data-stu-id="412d7-107">Deletes a resource from the submission.</span></span> <span data-ttu-id="412d7-108">Isso só pode ser feito pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="412d7-108">This can only be done by the student.</span></span> <span data-ttu-id="412d7-109">Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada após a cópia atual ser excluída.</span><span class="sxs-lookup"><span data-stu-id="412d7-109">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="412d7-110">Isso permite que você "Redefina" o recurso para seu estado original.</span><span class="sxs-lookup"><span data-stu-id="412d7-110">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="412d7-111">Se o recurso não foi copiado da atribuição, mas foi adicionado do aluno, o recurso será simplesmente excluído.</span><span class="sxs-lookup"><span data-stu-id="412d7-111">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="412d7-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="412d7-112">Permissions</span></span>
<span data-ttu-id="412d7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="412d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="412d7-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="412d7-115">Permission type</span></span>      | <span data-ttu-id="412d7-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="412d7-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="412d7-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="412d7-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="412d7-118">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="412d7-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="412d7-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="412d7-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="412d7-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="412d7-120">Not supported.</span></span>  |
|<span data-ttu-id="412d7-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="412d7-121">Application</span></span> | <span data-ttu-id="412d7-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="412d7-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="412d7-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="412d7-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="412d7-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="412d7-124">Request headers</span></span>
| <span data-ttu-id="412d7-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="412d7-125">Header</span></span>       | <span data-ttu-id="412d7-126">Valor</span><span class="sxs-lookup"><span data-stu-id="412d7-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="412d7-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="412d7-127">Authorization</span></span>  | <span data-ttu-id="412d7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="412d7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="412d7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="412d7-130">Request body</span></span>
<span data-ttu-id="412d7-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="412d7-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="412d7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="412d7-132">Response</span></span>
<span data-ttu-id="412d7-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="412d7-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="412d7-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="412d7-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="412d7-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="412d7-136">Request</span></span>
<span data-ttu-id="412d7-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="412d7-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="412d7-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="412d7-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
# <a name="c"></a>[<span data-ttu-id="412d7-139">C#</span><span class="sxs-lookup"><span data-stu-id="412d7-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationsubmissionresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="412d7-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="412d7-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationsubmissionresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="412d7-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="412d7-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationsubmissionresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="412d7-142">Java</span><span class="sxs-lookup"><span data-stu-id="412d7-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationsubmissionresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="412d7-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="412d7-143">Response</span></span>
<span data-ttu-id="412d7-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="412d7-144">The following is an example of the response.</span></span> 

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


