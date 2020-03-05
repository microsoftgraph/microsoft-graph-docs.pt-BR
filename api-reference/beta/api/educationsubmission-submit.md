---
title: 'educationSubmission: enviar'
description: Uma ação que indica que um aluno foi feito com o trabalho e está pronto para ser entregue na atribuição. Esta ação só pode ser realizada pelo aluno.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 58ddcd99c1e93696fbca037cea89ed51bd633283
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424740"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="74ddf-104">educationSubmission: enviar</span><span class="sxs-lookup"><span data-stu-id="74ddf-104">educationSubmission: submit</span></span>

<span data-ttu-id="74ddf-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="74ddf-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74ddf-106">Uma ação que indica que um aluno foi feito com o trabalho e está pronto para ser entregue na atribuição.</span><span class="sxs-lookup"><span data-stu-id="74ddf-106">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="74ddf-107">Esta ação só pode ser realizada pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="74ddf-107">This action can only be taken by the student.</span></span> <span data-ttu-id="74ddf-108">Isso alterará o status do envio de "trabalho" para "enviado".</span><span class="sxs-lookup"><span data-stu-id="74ddf-108">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="74ddf-109">Durante o processo de envio, todos os recursos serão copiados para o Bucket submittedResources.</span><span class="sxs-lookup"><span data-stu-id="74ddf-109">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="74ddf-110">O professor examinará a lista de recursos enviados para fins de gradação.</span><span class="sxs-lookup"><span data-stu-id="74ddf-110">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="74ddf-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="74ddf-111">Permissions</span></span>
<span data-ttu-id="74ddf-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74ddf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74ddf-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74ddf-114">Permission type</span></span>      | <span data-ttu-id="74ddf-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74ddf-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74ddf-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74ddf-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="74ddf-117">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74ddf-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="74ddf-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74ddf-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="74ddf-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74ddf-119">Not supported.</span></span>  |
|<span data-ttu-id="74ddf-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74ddf-120">Application</span></span> | <span data-ttu-id="74ddf-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74ddf-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="74ddf-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74ddf-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="74ddf-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74ddf-123">Request headers</span></span>
| <span data-ttu-id="74ddf-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74ddf-124">Header</span></span>       | <span data-ttu-id="74ddf-125">Valor</span><span class="sxs-lookup"><span data-stu-id="74ddf-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="74ddf-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="74ddf-126">Authorization</span></span>  | <span data-ttu-id="74ddf-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74ddf-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="74ddf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74ddf-129">Request body</span></span>
<span data-ttu-id="74ddf-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74ddf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74ddf-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="74ddf-131">Response</span></span>
<span data-ttu-id="74ddf-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74ddf-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74ddf-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74ddf-134">Example</span></span>
<span data-ttu-id="74ddf-135">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="74ddf-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="74ddf-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74ddf-136">Request</span></span>
<span data-ttu-id="74ddf-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="74ddf-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="74ddf-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="74ddf-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```
# <a name="c"></a>[<span data-ttu-id="74ddf-139">C#</span><span class="sxs-lookup"><span data-stu-id="74ddf-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-submit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74ddf-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74ddf-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-submit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74ddf-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74ddf-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-submit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="74ddf-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="74ddf-142">Response</span></span>
<span data-ttu-id="74ddf-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="74ddf-143">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
