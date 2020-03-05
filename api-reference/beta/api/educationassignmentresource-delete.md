---
title: Excluir educationAssignmentResource
description: .
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2e2d1c887d2c25f5d385c734a6e85912929704d5
ms.sourcegitcommit: fc818699566f03493937be95447eb9f656a1f950
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534417"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="459be-103">Excluir educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="459be-103">Delete educationAssignmentResource</span></span>

<span data-ttu-id="459be-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="459be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="459be-105">Excluir um recurso de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="459be-105">Delete a resource from an assignment.</span></span> <span data-ttu-id="459be-106">Somente os professores da turma podem remover um recurso.</span><span class="sxs-lookup"><span data-stu-id="459be-106">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="459be-107">Após uma atribuição ter sido publicada para estudantes, os professores não poderão remover recursos marcados como "distributeToStudents".</span><span class="sxs-lookup"><span data-stu-id="459be-107">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="459be-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="459be-108">Permissions</span></span>
<span data-ttu-id="459be-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="459be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="459be-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="459be-111">Permission type</span></span>      | <span data-ttu-id="459be-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="459be-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="459be-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="459be-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="459be-114">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="459be-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="459be-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="459be-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="459be-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="459be-116">Not supported.</span></span>  |
|<span data-ttu-id="459be-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="459be-117">Application</span></span> | <span data-ttu-id="459be-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="459be-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="459be-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="459be-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="459be-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="459be-120">Request headers</span></span>
| <span data-ttu-id="459be-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="459be-121">Header</span></span>       | <span data-ttu-id="459be-122">Valor</span><span class="sxs-lookup"><span data-stu-id="459be-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="459be-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="459be-123">Authorization</span></span>  | <span data-ttu-id="459be-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="459be-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="459be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="459be-126">Request body</span></span>
<span data-ttu-id="459be-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="459be-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="459be-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="459be-128">Response</span></span>
<span data-ttu-id="459be-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="459be-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="459be-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="459be-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="459be-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="459be-132">Request</span></span>
<span data-ttu-id="459be-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="459be-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="459be-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="459be-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="c"></a>[<span data-ttu-id="459be-135">C#</span><span class="sxs-lookup"><span data-stu-id="459be-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="459be-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="459be-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="459be-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="459be-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="459be-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="459be-138">Response</span></span>
<span data-ttu-id="459be-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="459be-139">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
