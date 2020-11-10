---
title: 'educationAssignment: publish'
description: Esta ação altera o estado de uma atribuição do status original do rascunho para o status publicado. Apenas um professor na turma pode fazer essa chamada. Quando uma atribuição está no status de rascunho, os alunos não verão a atribuição nem haverá nenhum objeto de envio. Ao chamar essa API, os objetos de envio são criados e a atribuição aparece na lista do aluno.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 40e32d07e89d870a12143b4b970f8a8520b508c0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966521"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="d0217-106">educationAssignment: publish</span><span class="sxs-lookup"><span data-stu-id="d0217-106">educationAssignment: publish</span></span>

<span data-ttu-id="d0217-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0217-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0217-108">Esta ação altera o estado de uma atribuição do status original do rascunho para o status publicado.</span><span class="sxs-lookup"><span data-stu-id="d0217-108">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="d0217-109">Apenas um professor na turma pode fazer essa chamada.</span><span class="sxs-lookup"><span data-stu-id="d0217-109">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="d0217-110">Quando uma atribuição está no status de rascunho, os alunos não verão a atribuição nem haverá nenhum objeto de envio.</span><span class="sxs-lookup"><span data-stu-id="d0217-110">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="d0217-111">Ao chamar essa API, os objetos de envio são criados e a atribuição aparece na lista do aluno.</span><span class="sxs-lookup"><span data-stu-id="d0217-111">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0217-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0217-112">Permissions</span></span>
<span data-ttu-id="d0217-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0217-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0217-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0217-115">Permission type</span></span>      | <span data-ttu-id="d0217-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0217-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0217-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0217-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="d0217-118">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0217-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d0217-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0217-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d0217-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0217-120">Not supported.</span></span>  |
|<span data-ttu-id="d0217-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0217-121">Application</span></span> | <span data-ttu-id="d0217-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0217-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d0217-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0217-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="d0217-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0217-124">Request headers</span></span>
| <span data-ttu-id="d0217-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0217-125">Header</span></span>       | <span data-ttu-id="d0217-126">Valor</span><span class="sxs-lookup"><span data-stu-id="d0217-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d0217-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0217-127">Authorization</span></span>  | <span data-ttu-id="d0217-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0217-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d0217-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0217-130">Request body</span></span>
<span data-ttu-id="d0217-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0217-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0217-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0217-132">Response</span></span>
<span data-ttu-id="d0217-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0217-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0217-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0217-135">Example</span></span>
<span data-ttu-id="d0217-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d0217-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d0217-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0217-137">Request</span></span>
<span data-ttu-id="d0217-138">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0217-138">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d0217-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0217-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```
# <a name="c"></a>[<span data-ttu-id="d0217-140">C#</span><span class="sxs-lookup"><span data-stu-id="d0217-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0217-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0217-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0217-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0217-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0217-143">Java</span><span class="sxs-lookup"><span data-stu-id="d0217-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d0217-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0217-144">Response</span></span>
<span data-ttu-id="d0217-145">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="d0217-145">The following is an example of a response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


