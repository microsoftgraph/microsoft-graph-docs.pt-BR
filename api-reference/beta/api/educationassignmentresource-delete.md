---
title: Excluir educationAssignmentResource
description: .
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 330f00c46bc9bff8796655f6f1eff8e6a3039164
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587673"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="8604d-103">Excluir educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="8604d-103">Delete educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8604d-104">Excluir um recurso de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="8604d-104">Delete a resource from an assignment.</span></span> <span data-ttu-id="8604d-105">Somente os professores da turma podem remover um recurso.</span><span class="sxs-lookup"><span data-stu-id="8604d-105">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="8604d-106">Após uma atribuição ter sido publicada para estudantes, os professores não poderão remover recursos marcados como "distributeToStudents".</span><span class="sxs-lookup"><span data-stu-id="8604d-106">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="8604d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8604d-107">Permissions</span></span>
<span data-ttu-id="8604d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8604d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8604d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8604d-110">Permission type</span></span>      | <span data-ttu-id="8604d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8604d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8604d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8604d-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="8604d-113">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8604d-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="8604d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8604d-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8604d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8604d-115">Not supported.</span></span>  |
|<span data-ttu-id="8604d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8604d-116">Application</span></span> | <span data-ttu-id="8604d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8604d-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8604d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8604d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="8604d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8604d-119">Request headers</span></span>
| <span data-ttu-id="8604d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8604d-120">Header</span></span>       | <span data-ttu-id="8604d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8604d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8604d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8604d-122">Authorization</span></span>  | <span data-ttu-id="8604d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8604d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8604d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8604d-125">Request body</span></span>
<span data-ttu-id="8604d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8604d-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8604d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8604d-127">Response</span></span>
<span data-ttu-id="8604d-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8604d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8604d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8604d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8604d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8604d-131">Request</span></span>
<span data-ttu-id="8604d-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8604d-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="8604d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8604d-133">Response</span></span>
<span data-ttu-id="8604d-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8604d-134">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8604d-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8604d-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8604d-136">Basic</span><span class="sxs-lookup"><span data-stu-id="8604d-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationassignmentresource-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8604d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8604d-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationassignmentresource-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/educationassignmentresource-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationassignmentresource-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
