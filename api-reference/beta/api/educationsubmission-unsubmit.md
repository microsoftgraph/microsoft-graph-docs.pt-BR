---
title: 'educationSubmission: não enviar'
description: 'Uma ação que indica que um aluno deseja trabalhar no envio da atribuição depois que ela foi ativada. Esta ação só pode ser realizada pelo aluno. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 84b3b99b6ef04585f6380c297a98a08d909ff6ac
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259476"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="1d053-104">educationSubmission: não enviar</span><span class="sxs-lookup"><span data-stu-id="1d053-104">educationSubmission: unsubmit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d053-105">Uma ação que indica que um aluno deseja trabalhar no envio da atribuição depois que ela foi ativada.</span><span class="sxs-lookup"><span data-stu-id="1d053-105">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="1d053-106">Esta ação só pode ser realizada pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="1d053-106">This action can only be taken by the student.</span></span> <span data-ttu-id="1d053-107">Isso alterará o status do envio de "enviado" para "trabalho".</span><span class="sxs-lookup"><span data-stu-id="1d053-107">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="1d053-108">Durante o processo de envio, todos os recursos serão copiados do submittedResources para o Bucket do workingResources.</span><span class="sxs-lookup"><span data-stu-id="1d053-108">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="1d053-109">O professor examinará a lista de recursos de trabalho para fins de gradação.</span><span class="sxs-lookup"><span data-stu-id="1d053-109">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d053-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d053-110">Permissions</span></span>
<span data-ttu-id="1d053-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d053-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d053-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d053-113">Permission type</span></span>      | <span data-ttu-id="1d053-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d053-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d053-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d053-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="1d053-116">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d053-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="1d053-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d053-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1d053-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d053-118">Not supported.</span></span>  |
|<span data-ttu-id="1d053-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d053-119">Application</span></span> | <span data-ttu-id="1d053-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d053-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1d053-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d053-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="1d053-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d053-122">Request headers</span></span>
| <span data-ttu-id="1d053-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d053-123">Header</span></span>       | <span data-ttu-id="1d053-124">Valor</span><span class="sxs-lookup"><span data-stu-id="1d053-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1d053-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d053-125">Authorization</span></span>  | <span data-ttu-id="1d053-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d053-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1d053-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d053-128">Request body</span></span>
<span data-ttu-id="1d053-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1d053-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d053-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d053-130">Response</span></span>
<span data-ttu-id="1d053-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d053-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d053-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d053-133">Example</span></span>
<span data-ttu-id="1d053-134">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="1d053-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1d053-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d053-135">Request</span></span>
<span data-ttu-id="1d053-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d053-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```

##### <a name="response"></a><span data-ttu-id="1d053-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d053-137">Response</span></span>
<span data-ttu-id="1d053-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1d053-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1d053-139">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="1d053-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1d053-140">C#</span><span class="sxs-lookup"><span data-stu-id="1d053-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/educationsubmission_unsubmit-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1d053-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="1d053-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/educationsubmission_unsubmit-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1d053-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1d053-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/educationsubmission_unsubmit-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/educationsubmission-unsubmit.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationsubmission-unsubmit.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsubmission-unsubmit.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
