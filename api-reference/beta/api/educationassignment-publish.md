---
title: 'educationAssignment: publish'
description: Esta ação altera o estado de uma atribuição do status original do rascunho para o status publicado. Apenas um professor na turma pode fazer essa chamada. Quando uma atribuição está no status de rascunho, os alunos não verão a atribuição nem haverá nenhum objeto de envio. Ao chamar essa API, os objetos de envio são criados e a atribuição aparece na lista do aluno.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a425562009c66c1a406129361a8bc1b2230cf47e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320900"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="98b6f-106">educationAssignment: publish</span><span class="sxs-lookup"><span data-stu-id="98b6f-106">educationAssignment: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98b6f-107">Esta ação altera o estado de uma atribuição do status original do rascunho para o status publicado.</span><span class="sxs-lookup"><span data-stu-id="98b6f-107">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="98b6f-108">Apenas um professor na turma pode fazer essa chamada.</span><span class="sxs-lookup"><span data-stu-id="98b6f-108">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="98b6f-109">Quando uma atribuição está no status de rascunho, os alunos não verão a atribuição nem haverá nenhum objeto de envio.</span><span class="sxs-lookup"><span data-stu-id="98b6f-109">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="98b6f-110">Ao chamar essa API, os objetos de envio são criados e a atribuição aparece na lista do aluno.</span><span class="sxs-lookup"><span data-stu-id="98b6f-110">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="98b6f-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="98b6f-111">Permissions</span></span>
<span data-ttu-id="98b6f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98b6f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98b6f-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98b6f-114">Permission type</span></span>      | <span data-ttu-id="98b6f-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98b6f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98b6f-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98b6f-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="98b6f-117">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98b6f-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="98b6f-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98b6f-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="98b6f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98b6f-119">Not supported.</span></span>  |
|<span data-ttu-id="98b6f-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98b6f-120">Application</span></span> | <span data-ttu-id="98b6f-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98b6f-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="98b6f-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98b6f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="98b6f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98b6f-123">Request headers</span></span>
| <span data-ttu-id="98b6f-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98b6f-124">Header</span></span>       | <span data-ttu-id="98b6f-125">Valor</span><span class="sxs-lookup"><span data-stu-id="98b6f-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="98b6f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="98b6f-126">Authorization</span></span>  | <span data-ttu-id="98b6f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98b6f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="98b6f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98b6f-129">Request body</span></span>
<span data-ttu-id="98b6f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="98b6f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98b6f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="98b6f-131">Response</span></span>
<span data-ttu-id="98b6f-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98b6f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98b6f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98b6f-134">Example</span></span>
<span data-ttu-id="98b6f-135">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="98b6f-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="98b6f-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98b6f-136">Request</span></span>
<span data-ttu-id="98b6f-137">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="98b6f-137">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="98b6f-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="98b6f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="98b6f-139">C#</span><span class="sxs-lookup"><span data-stu-id="98b6f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98b6f-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98b6f-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="98b6f-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="98b6f-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="98b6f-142">Java</span><span class="sxs-lookup"><span data-stu-id="98b6f-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="98b6f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="98b6f-143">Response</span></span>
<span data-ttu-id="98b6f-144">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="98b6f-144">The following is an example of a response.</span></span> 

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
