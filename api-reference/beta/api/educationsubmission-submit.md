---
title: 'educationSubmission: submit'
description: Uma ação que indica que um aluno é feito com o trabalho e está pronto para entregar a atribuição. Essa ação só pode ser tomada pelo aluno.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2f33bea764c76ccc3a320bd610249cedf372071f
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787279"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="8e727-104">educationSubmission: submit</span><span class="sxs-lookup"><span data-stu-id="8e727-104">educationSubmission: submit</span></span>

<span data-ttu-id="8e727-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e727-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e727-106">Uma ação que indica que um aluno é feito com o trabalho e está pronto para entregar a atribuição.</span><span class="sxs-lookup"><span data-stu-id="8e727-106">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="8e727-107">Essa ação só pode ser tomada pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="8e727-107">This action can only be taken by the student.</span></span> <span data-ttu-id="8e727-108">Isso alterará o status do envio de "working" para "submitted".</span><span class="sxs-lookup"><span data-stu-id="8e727-108">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="8e727-109">Durante o processo de envio, todos os recursos serão copiados para o **bucket submittedResources.**</span><span class="sxs-lookup"><span data-stu-id="8e727-109">During the submit process, all the resources will be copied to the **submittedResources** bucket.</span></span> <span data-ttu-id="8e727-110">O professor estará olhando para a lista de recursos enviados para classificação.</span><span class="sxs-lookup"><span data-stu-id="8e727-110">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e727-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="8e727-111">Permissions</span></span>
<span data-ttu-id="8e727-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e727-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e727-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e727-114">Permission type</span></span>      | <span data-ttu-id="8e727-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e727-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e727-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e727-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="8e727-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e727-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="8e727-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e727-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8e727-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e727-119">Not supported.</span></span>  |
|<span data-ttu-id="8e727-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e727-120">Application</span></span> | <span data-ttu-id="8e727-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e727-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8e727-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e727-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit
```

## <a name="request-headers"></a><span data-ttu-id="8e727-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e727-123">Request headers</span></span>
| <span data-ttu-id="8e727-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e727-124">Header</span></span>       | <span data-ttu-id="8e727-125">Valor</span><span class="sxs-lookup"><span data-stu-id="8e727-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8e727-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e727-126">Authorization</span></span>  | <span data-ttu-id="8e727-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e727-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e727-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e727-129">Request body</span></span>
<span data-ttu-id="8e727-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e727-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e727-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e727-131">Response</span></span>
<span data-ttu-id="8e727-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e727-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e727-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e727-134">Example</span></span>
<span data-ttu-id="8e727-135">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8e727-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8e727-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e727-136">Request</span></span>
<span data-ttu-id="8e727-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e727-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e727-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e727-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```
# <a name="c"></a>[<span data-ttu-id="8e727-139">C#</span><span class="sxs-lookup"><span data-stu-id="8e727-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-submit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e727-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e727-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-submit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e727-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e727-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-submit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e727-142">Java</span><span class="sxs-lookup"><span data-stu-id="8e727-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-submit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8e727-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e727-143">Response</span></span>
<span data-ttu-id="8e727-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e727-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


