---
title: Excluir educationSubmissionResource
description: Exclui um recurso do envio. Isso só pode ser feito pelo aluno. Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada após a cópia atual ser excluída.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 72905ef2dabe7b9b08703dab9f313f44923e6b8d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991310"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="0cd9c-105">Excluir educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="0cd9c-105">Delete educationSubmissionResource</span></span>

<span data-ttu-id="0cd9c-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cd9c-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cd9c-107">Exclui um recurso do envio.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-107">Deletes a resource from the submission.</span></span> <span data-ttu-id="0cd9c-108">Isso só pode ser feito pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-108">This can only be done by the student.</span></span> <span data-ttu-id="0cd9c-109">Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada após a cópia atual ser excluída.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-109">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="0cd9c-110">Isso permite que você "Redefina" o recurso para seu estado original.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-110">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="0cd9c-111">Se o recurso não foi copiado da atribuição, mas foi adicionado do aluno, o recurso será simplesmente excluído.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-111">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cd9c-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="0cd9c-112">Permissions</span></span>
<span data-ttu-id="0cd9c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cd9c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cd9c-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cd9c-115">Permission type</span></span>      | <span data-ttu-id="0cd9c-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0cd9c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cd9c-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cd9c-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="0cd9c-118">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0cd9c-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="0cd9c-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cd9c-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0cd9c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-120">Not supported.</span></span>  |
|<span data-ttu-id="0cd9c-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cd9c-121">Application</span></span> | <span data-ttu-id="0cd9c-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0cd9c-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cd9c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="0cd9c-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cd9c-124">Request headers</span></span>
| <span data-ttu-id="0cd9c-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0cd9c-125">Header</span></span>       | <span data-ttu-id="0cd9c-126">Valor</span><span class="sxs-lookup"><span data-stu-id="0cd9c-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0cd9c-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cd9c-127">Authorization</span></span>  | <span data-ttu-id="0cd9c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0cd9c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cd9c-130">Request body</span></span>
<span data-ttu-id="0cd9c-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0cd9c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cd9c-132">Response</span></span>
<span data-ttu-id="0cd9c-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cd9c-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cd9c-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0cd9c-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cd9c-136">Request</span></span>
<span data-ttu-id="0cd9c-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0cd9c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cd9c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
# <a name="c"></a>[<span data-ttu-id="0cd9c-139">C#</span><span class="sxs-lookup"><span data-stu-id="0cd9c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationsubmissionresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cd9c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cd9c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationsubmissionresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cd9c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cd9c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationsubmissionresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0cd9c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cd9c-142">Response</span></span>
<span data-ttu-id="0cd9c-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0cd9c-143">The following is an example of the response.</span></span> 

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


