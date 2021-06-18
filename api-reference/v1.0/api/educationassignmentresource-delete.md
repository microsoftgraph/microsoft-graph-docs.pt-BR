---
title: Excluir educationAssignmentResource
description: Exclua um recurso específico anexado a uma atribuição.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 16cb969fc4f1980c7ec5b37f5dfb8c1c384c6e7f
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993000"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="951b7-103">Excluir educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="951b7-103">Delete educationAssignmentResource</span></span>

<span data-ttu-id="951b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="951b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="951b7-105">Exclua um recurso específico anexado a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="951b7-105">Delete a specific resource attached to an assignment.</span></span>

<span data-ttu-id="951b7-106">Em geral, somente os professores da classe podem remover um recurso.</span><span class="sxs-lookup"><span data-stu-id="951b7-106">In general, only teachers in the class can remove a resource.</span></span> <span data-ttu-id="951b7-107">No entanto, os professores não podem remover recursos marcados como "distributeToStudents", depois que a atribuição tiver sido publicada para os alunos.</span><span class="sxs-lookup"><span data-stu-id="951b7-107">However, teachers cannot remove resources marked as "distributeToStudents", after the assignment has been published to students.</span></span>

## <a name="permissions"></a><span data-ttu-id="951b7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="951b7-108">Permissions</span></span>
<span data-ttu-id="951b7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="951b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="951b7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="951b7-111">Permission type</span></span>      | <span data-ttu-id="951b7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="951b7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="951b7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="951b7-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="951b7-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="951b7-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="951b7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="951b7-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="951b7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="951b7-116">Not supported.</span></span>  |
|<span data-ttu-id="951b7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="951b7-117">Application</span></span> | <span data-ttu-id="951b7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="951b7-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="951b7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="951b7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/resources/8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c

```
## <a name="request-headers"></a><span data-ttu-id="951b7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="951b7-120">Request headers</span></span>
| <span data-ttu-id="951b7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="951b7-121">Header</span></span>       | <span data-ttu-id="951b7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="951b7-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="951b7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="951b7-123">Authorization</span></span>  | <span data-ttu-id="951b7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="951b7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="951b7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="951b7-126">Request body</span></span>
<span data-ttu-id="951b7-127">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="951b7-127">Don't supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="951b7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="951b7-128">Response</span></span>
<span data-ttu-id="951b7-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="951b7-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="951b7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="951b7-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="951b7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="951b7-132">Request</span></span>
<span data-ttu-id="951b7-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="951b7-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="951b7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="951b7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/resources/22002
```
# <a name="c"></a>[<span data-ttu-id="951b7-135">C#</span><span class="sxs-lookup"><span data-stu-id="951b7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="951b7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="951b7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="951b7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="951b7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="951b7-138">Java</span><span class="sxs-lookup"><span data-stu-id="951b7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="951b7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="951b7-139">Response</span></span>
<span data-ttu-id="951b7-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="951b7-140">The following is an example of the response.</span></span> 


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


