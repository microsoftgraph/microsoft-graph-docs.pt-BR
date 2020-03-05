---
title: Excluir educationSubmissionResource
description: Exclui um recurso do envio. Isso só pode ser feito pelo aluno. Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada após a cópia atual ser excluída.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ffba53cee0cd3038db3e97fab2ff3a27c881bed3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424726"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="d4d41-105">Excluir educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="d4d41-105">Delete educationSubmissionResource</span></span>

<span data-ttu-id="d4d41-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d4d41-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4d41-107">Exclui um recurso do envio.</span><span class="sxs-lookup"><span data-stu-id="d4d41-107">Deletes a resource from the submission.</span></span> <span data-ttu-id="d4d41-108">Isso só pode ser feito pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="d4d41-108">This can only be done by the student.</span></span> <span data-ttu-id="d4d41-109">Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada após a cópia atual ser excluída.</span><span class="sxs-lookup"><span data-stu-id="d4d41-109">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="d4d41-110">Isso permite que você "Redefina" o recurso para seu estado original.</span><span class="sxs-lookup"><span data-stu-id="d4d41-110">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="d4d41-111">Se o recurso não foi copiado da atribuição, mas foi adicionado do aluno, o recurso será simplesmente excluído.</span><span class="sxs-lookup"><span data-stu-id="d4d41-111">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4d41-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4d41-112">Permissions</span></span>
<span data-ttu-id="d4d41-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4d41-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4d41-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4d41-115">Permission type</span></span>      | <span data-ttu-id="d4d41-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4d41-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4d41-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4d41-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="d4d41-118">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4d41-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d4d41-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4d41-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d4d41-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4d41-120">Not supported.</span></span>  |
|<span data-ttu-id="d4d41-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4d41-121">Application</span></span> | <span data-ttu-id="d4d41-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4d41-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d4d41-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4d41-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="d4d41-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4d41-124">Request headers</span></span>
| <span data-ttu-id="d4d41-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4d41-125">Header</span></span>       | <span data-ttu-id="d4d41-126">Valor</span><span class="sxs-lookup"><span data-stu-id="d4d41-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d4d41-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4d41-127">Authorization</span></span>  | <span data-ttu-id="d4d41-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4d41-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d4d41-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4d41-130">Request body</span></span>
<span data-ttu-id="d4d41-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4d41-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d4d41-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4d41-132">Response</span></span>
<span data-ttu-id="d4d41-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4d41-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4d41-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4d41-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4d41-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4d41-136">Request</span></span>
<span data-ttu-id="d4d41-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4d41-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d4d41-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4d41-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
# <a name="c"></a>[<span data-ttu-id="d4d41-139">C#</span><span class="sxs-lookup"><span data-stu-id="d4d41-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationsubmissionresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4d41-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4d41-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationsubmissionresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4d41-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4d41-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationsubmissionresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d4d41-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4d41-142">Response</span></span>
<span data-ttu-id="d4d41-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d4d41-143">The following is an example of the response.</span></span> 

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
