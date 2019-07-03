---
title: Excluir educationAssignmentResource
description: .
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d4a38b2f8b8d4f0ff278ad0984681c2e970257ed
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436107"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="61a04-103">Excluir educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="61a04-103">Delete educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61a04-104">Excluir um recurso de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="61a04-104">Delete a resource from an assignment.</span></span> <span data-ttu-id="61a04-105">Somente os professores da turma podem remover um recurso.</span><span class="sxs-lookup"><span data-stu-id="61a04-105">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="61a04-106">Após uma atribuição ter sido publicada para estudantes, os professores não poderão remover recursos marcados como "distributeToStudents".</span><span class="sxs-lookup"><span data-stu-id="61a04-106">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="61a04-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="61a04-107">Permissions</span></span>
<span data-ttu-id="61a04-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61a04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61a04-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61a04-110">Permission type</span></span>      | <span data-ttu-id="61a04-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61a04-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61a04-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61a04-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="61a04-113">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61a04-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="61a04-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61a04-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="61a04-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61a04-115">Not supported.</span></span>  |
|<span data-ttu-id="61a04-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61a04-116">Application</span></span> | <span data-ttu-id="61a04-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61a04-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="61a04-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61a04-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="61a04-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61a04-119">Request headers</span></span>
| <span data-ttu-id="61a04-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61a04-120">Header</span></span>       | <span data-ttu-id="61a04-121">Valor</span><span class="sxs-lookup"><span data-stu-id="61a04-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="61a04-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="61a04-122">Authorization</span></span>  | <span data-ttu-id="61a04-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61a04-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="61a04-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61a04-125">Request body</span></span>
<span data-ttu-id="61a04-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61a04-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="61a04-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="61a04-127">Response</span></span>
<span data-ttu-id="61a04-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61a04-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61a04-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61a04-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61a04-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61a04-131">Request</span></span>
<span data-ttu-id="61a04-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="61a04-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="61a04-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="61a04-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="61a04-134">C#</span><span class="sxs-lookup"><span data-stu-id="61a04-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="61a04-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="61a04-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="61a04-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="61a04-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="61a04-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="61a04-137">Response</span></span>
<span data-ttu-id="61a04-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="61a04-138">The following is an example of the response.</span></span> 


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
