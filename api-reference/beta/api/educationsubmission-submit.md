---
title: 'educationSubmission: enviar'
description: Uma ação que indica que um aluno foi feito com o trabalho e está pronto para ser entregue na atribuição. Esta ação só pode ser realizada pelo aluno.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 58ddf90e574e146ebdbd9134ec41ae2ac76637bb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441405"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="f5f79-104">educationSubmission: enviar</span><span class="sxs-lookup"><span data-stu-id="f5f79-104">educationSubmission: submit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5f79-105">Uma ação que indica que um aluno foi feito com o trabalho e está pronto para ser entregue na atribuição.</span><span class="sxs-lookup"><span data-stu-id="f5f79-105">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="f5f79-106">Esta ação só pode ser realizada pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="f5f79-106">This action can only be taken by the student.</span></span> <span data-ttu-id="f5f79-107">Isso alterará o status do envio de "trabalho" para "enviado".</span><span class="sxs-lookup"><span data-stu-id="f5f79-107">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="f5f79-108">Durante o processo de envio, todos os recursos serão copiados para o Bucket submittedResources.</span><span class="sxs-lookup"><span data-stu-id="f5f79-108">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="f5f79-109">O professor examinará a lista de recursos enviados para fins de gradação.</span><span class="sxs-lookup"><span data-stu-id="f5f79-109">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5f79-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5f79-110">Permissions</span></span>
<span data-ttu-id="f5f79-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5f79-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5f79-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5f79-113">Permission type</span></span>      | <span data-ttu-id="f5f79-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5f79-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5f79-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5f79-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="f5f79-116">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5f79-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f5f79-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5f79-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f5f79-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5f79-118">Not supported.</span></span>  |
|<span data-ttu-id="f5f79-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5f79-119">Application</span></span> | <span data-ttu-id="f5f79-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5f79-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f5f79-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5f79-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="f5f79-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f79-122">Request headers</span></span>
| <span data-ttu-id="f5f79-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5f79-123">Header</span></span>       | <span data-ttu-id="f5f79-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f5f79-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f5f79-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5f79-125">Authorization</span></span>  | <span data-ttu-id="f5f79-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5f79-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f5f79-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f79-128">Request body</span></span>
<span data-ttu-id="f5f79-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5f79-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5f79-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f79-130">Response</span></span>
<span data-ttu-id="f5f79-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5f79-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5f79-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5f79-133">Example</span></span>
<span data-ttu-id="f5f79-134">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f5f79-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f5f79-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5f79-135">Request</span></span>
<span data-ttu-id="f5f79-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5f79-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f5f79-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5f79-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f5f79-138">C#</span><span class="sxs-lookup"><span data-stu-id="f5f79-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-submit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f5f79-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="f5f79-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-submit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f5f79-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f5f79-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-submit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f5f79-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5f79-141">Response</span></span>
<span data-ttu-id="f5f79-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f5f79-142">The following is an example of the response.</span></span>

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
