---
title: Excluir educationAssignmentResource
description: Exclua um recurso específico anexado a uma atribuição.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7e853534998978f89e44cbd8f657a56250c599a0
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911901"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="f377d-103">Excluir educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="f377d-103">Delete educationAssignmentResource</span></span>

<span data-ttu-id="f377d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f377d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f377d-105">Exclua um recurso específico anexado a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="f377d-105">Delete a specific resource attached to an assignment.</span></span> <span data-ttu-id="f377d-106">Somente os professores da classe podem remover um recurso.</span><span class="sxs-lookup"><span data-stu-id="f377d-106">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="f377d-107">Depois que uma atribuição é publicada para os alunos, os professores não podem remover recursos marcados como "distributeToStudents".</span><span class="sxs-lookup"><span data-stu-id="f377d-107">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="f377d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f377d-108">Permissions</span></span>
<span data-ttu-id="f377d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f377d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f377d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f377d-111">Permission type</span></span>      | <span data-ttu-id="f377d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f377d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f377d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f377d-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="f377d-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f377d-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f377d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f377d-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f377d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f377d-116">Not supported.</span></span>  |
|<span data-ttu-id="f377d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f377d-117">Application</span></span> | <span data-ttu-id="f377d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f377d-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f377d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f377d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="f377d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f377d-120">Request headers</span></span>
| <span data-ttu-id="f377d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f377d-121">Header</span></span>       | <span data-ttu-id="f377d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f377d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f377d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f377d-123">Authorization</span></span>  | <span data-ttu-id="f377d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f377d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f377d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f377d-126">Request body</span></span>
<span data-ttu-id="f377d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f377d-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f377d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f377d-128">Response</span></span>
<span data-ttu-id="f377d-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f377d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f377d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f377d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f377d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f377d-132">Request</span></span>
<span data-ttu-id="f377d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f377d-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f377d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f377d-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="c"></a>[<span data-ttu-id="f377d-135">C#</span><span class="sxs-lookup"><span data-stu-id="f377d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f377d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f377d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f377d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f377d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f377d-138">Java</span><span class="sxs-lookup"><span data-stu-id="f377d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f377d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f377d-139">Response</span></span>
<span data-ttu-id="f377d-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f377d-140">The following is an example of the response.</span></span> 


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


