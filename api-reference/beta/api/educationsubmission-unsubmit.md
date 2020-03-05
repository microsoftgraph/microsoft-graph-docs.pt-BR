---
title: 'educationSubmission: não enviar'
description: 'Uma ação que indica que um aluno deseja trabalhar no envio da atribuição depois que ela foi ativada. Esta ação só pode ser realizada pelo aluno. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 17be34a014e83b43bf7494758933ecaa10f4068f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424733"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="b763f-104">educationSubmission: não enviar</span><span class="sxs-lookup"><span data-stu-id="b763f-104">educationSubmission: unsubmit</span></span>

<span data-ttu-id="b763f-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b763f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b763f-106">Uma ação que indica que um aluno deseja trabalhar no envio da atribuição depois que ela foi ativada.</span><span class="sxs-lookup"><span data-stu-id="b763f-106">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="b763f-107">Esta ação só pode ser realizada pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="b763f-107">This action can only be taken by the student.</span></span> <span data-ttu-id="b763f-108">Isso alterará o status do envio de "enviado" para "trabalho".</span><span class="sxs-lookup"><span data-stu-id="b763f-108">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="b763f-109">Durante o processo de envio, todos os recursos serão copiados do submittedResources para o Bucket do workingResources.</span><span class="sxs-lookup"><span data-stu-id="b763f-109">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="b763f-110">O professor examinará a lista de recursos de trabalho para fins de gradação.</span><span class="sxs-lookup"><span data-stu-id="b763f-110">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="b763f-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="b763f-111">Permissions</span></span>
<span data-ttu-id="b763f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b763f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b763f-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b763f-114">Permission type</span></span>      | <span data-ttu-id="b763f-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b763f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b763f-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b763f-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="b763f-117">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b763f-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="b763f-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b763f-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b763f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b763f-119">Not supported.</span></span>  |
|<span data-ttu-id="b763f-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b763f-120">Application</span></span> | <span data-ttu-id="b763f-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b763f-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b763f-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b763f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="b763f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b763f-123">Request headers</span></span>
| <span data-ttu-id="b763f-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b763f-124">Header</span></span>       | <span data-ttu-id="b763f-125">Valor</span><span class="sxs-lookup"><span data-stu-id="b763f-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b763f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b763f-126">Authorization</span></span>  | <span data-ttu-id="b763f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b763f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b763f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b763f-129">Request body</span></span>
<span data-ttu-id="b763f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b763f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b763f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b763f-131">Response</span></span>
<span data-ttu-id="b763f-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b763f-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b763f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b763f-134">Example</span></span>
<span data-ttu-id="b763f-135">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b763f-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b763f-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b763f-136">Request</span></span>
<span data-ttu-id="b763f-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b763f-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b763f-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="b763f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```
# <a name="c"></a>[<span data-ttu-id="b763f-139">C#</span><span class="sxs-lookup"><span data-stu-id="b763f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-unsubmit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b763f-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b763f-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-unsubmit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b763f-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b763f-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-unsubmit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b763f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b763f-142">Response</span></span>
<span data-ttu-id="b763f-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b763f-143">The following is an example of the response.</span></span>

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
