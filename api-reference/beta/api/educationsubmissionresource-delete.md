---
title: Excluir educationSubmissionResource
description: Exclui um recurso do envio. Isso só pode ser feito pelo aluno. Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada após a cópia atual ser excluída.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 056f09adb9bb36a38d613edaf8d0c1220d69bcb3
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587771"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="fe81f-105">Excluir educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="fe81f-105">Delete educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe81f-106">Exclui um recurso do envio.</span><span class="sxs-lookup"><span data-stu-id="fe81f-106">Deletes a resource from the submission.</span></span> <span data-ttu-id="fe81f-107">Isso só pode ser feito pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="fe81f-107">This can only be done by the student.</span></span> <span data-ttu-id="fe81f-108">Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada após a cópia atual ser excluída.</span><span class="sxs-lookup"><span data-stu-id="fe81f-108">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="fe81f-109">Isso permite que você "Redefina" o recurso para seu estado original.</span><span class="sxs-lookup"><span data-stu-id="fe81f-109">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="fe81f-110">Se o recurso não foi copiado da atribuição, mas foi adicionado do aluno, o recurso será simplesmente excluído.</span><span class="sxs-lookup"><span data-stu-id="fe81f-110">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe81f-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe81f-111">Permissions</span></span>
<span data-ttu-id="fe81f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe81f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe81f-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe81f-114">Permission type</span></span>      | <span data-ttu-id="fe81f-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe81f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe81f-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe81f-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="fe81f-117">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe81f-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="fe81f-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe81f-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fe81f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe81f-119">Not supported.</span></span>  |
|<span data-ttu-id="fe81f-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe81f-120">Application</span></span> | <span data-ttu-id="fe81f-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe81f-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fe81f-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe81f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="fe81f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe81f-123">Request headers</span></span>
| <span data-ttu-id="fe81f-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe81f-124">Header</span></span>       | <span data-ttu-id="fe81f-125">Valor</span><span class="sxs-lookup"><span data-stu-id="fe81f-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fe81f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe81f-126">Authorization</span></span>  | <span data-ttu-id="fe81f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe81f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fe81f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe81f-129">Request body</span></span>
<span data-ttu-id="fe81f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe81f-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="fe81f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe81f-131">Response</span></span>
<span data-ttu-id="fe81f-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe81f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe81f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe81f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe81f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe81f-135">Request</span></span>
<span data-ttu-id="fe81f-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe81f-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="fe81f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe81f-137">Response</span></span>
<span data-ttu-id="fe81f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fe81f-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fe81f-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="fe81f-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fe81f-140">Basic</span><span class="sxs-lookup"><span data-stu-id="fe81f-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationsubmissionresource-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe81f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe81f-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationsubmissionresource-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/educationsubmissionresource-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsubmissionresource-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
