---
title: 'educationSubmission: não enviar'
description: 'Uma ação que indica que um aluno deseja trabalhar no envio da atribuição depois que ela foi ativada. Esta ação só pode ser realizada pelo aluno. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 702d0d1e5dc18838c87ffa37ab5628e0f924e378
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323795"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="d681f-104">educationSubmission: não enviar</span><span class="sxs-lookup"><span data-stu-id="d681f-104">educationSubmission: unsubmit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d681f-105">Uma ação que indica que um aluno deseja trabalhar no envio da atribuição depois que ela foi ativada.</span><span class="sxs-lookup"><span data-stu-id="d681f-105">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="d681f-106">Esta ação só pode ser realizada pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="d681f-106">This action can only be taken by the student.</span></span> <span data-ttu-id="d681f-107">Isso alterará o status do envio de "enviado" para "trabalho".</span><span class="sxs-lookup"><span data-stu-id="d681f-107">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="d681f-108">Durante o processo de envio, todos os recursos serão copiados do submittedResources para o Bucket do workingResources.</span><span class="sxs-lookup"><span data-stu-id="d681f-108">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="d681f-109">O professor examinará a lista de recursos de trabalho para fins de gradação.</span><span class="sxs-lookup"><span data-stu-id="d681f-109">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="d681f-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d681f-110">Permissions</span></span>
<span data-ttu-id="d681f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d681f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d681f-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d681f-113">Permission type</span></span>      | <span data-ttu-id="d681f-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d681f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d681f-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d681f-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="d681f-116">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d681f-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d681f-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d681f-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d681f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d681f-118">Not supported.</span></span>  |
|<span data-ttu-id="d681f-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d681f-119">Application</span></span> | <span data-ttu-id="d681f-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d681f-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d681f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d681f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="d681f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d681f-122">Request headers</span></span>
| <span data-ttu-id="d681f-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d681f-123">Header</span></span>       | <span data-ttu-id="d681f-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d681f-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d681f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d681f-125">Authorization</span></span>  | <span data-ttu-id="d681f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d681f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d681f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d681f-128">Request body</span></span>
<span data-ttu-id="d681f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d681f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d681f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d681f-130">Response</span></span>
<span data-ttu-id="d681f-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d681f-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d681f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d681f-133">Example</span></span>
<span data-ttu-id="d681f-134">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d681f-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d681f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d681f-135">Request</span></span>
<span data-ttu-id="d681f-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d681f-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d681f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d681f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d681f-138">C#</span><span class="sxs-lookup"><span data-stu-id="d681f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-unsubmit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d681f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d681f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-unsubmit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d681f-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d681f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-unsubmit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d681f-141">Java</span><span class="sxs-lookup"><span data-stu-id="d681f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-unsubmit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d681f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d681f-142">Response</span></span>
<span data-ttu-id="d681f-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d681f-143">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: unsubmit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
