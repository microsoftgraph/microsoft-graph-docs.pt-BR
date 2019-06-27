---
title: 'educationSubmission: retornar'
description: Esta ação faz com que a classificação e os comentários associados a esse envio estejam disponíveis para o aluno.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 60d470dbfe80620e477a2b60cd47a875ca7ad043
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259490"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="76a98-103">educationSubmission: retornar</span><span class="sxs-lookup"><span data-stu-id="76a98-103">educationSubmission: return</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76a98-104">Esta ação faz com que a classificação e os comentários associados a esse envio estejam disponíveis para o aluno.</span><span class="sxs-lookup"><span data-stu-id="76a98-104">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="76a98-105">Isso alterará o status do envio de "enviado" para "retornado" e indica que o feedback é fornecido ou a gradação é feita.</span><span class="sxs-lookup"><span data-stu-id="76a98-105">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="76a98-106">Esta ação só pode ser feita pelo professor.</span><span class="sxs-lookup"><span data-stu-id="76a98-106">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="76a98-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="76a98-107">Permissions</span></span>
<span data-ttu-id="76a98-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76a98-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76a98-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76a98-110">Permission type</span></span>      | <span data-ttu-id="76a98-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76a98-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76a98-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76a98-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="76a98-113">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76a98-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="76a98-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76a98-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="76a98-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76a98-115">Not supported.</span></span>  |
|<span data-ttu-id="76a98-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76a98-116">Application</span></span> | <span data-ttu-id="76a98-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76a98-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="76a98-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76a98-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="76a98-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76a98-119">Request headers</span></span>
| <span data-ttu-id="76a98-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76a98-120">Header</span></span>       | <span data-ttu-id="76a98-121">Valor</span><span class="sxs-lookup"><span data-stu-id="76a98-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="76a98-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="76a98-122">Authorization</span></span>  | <span data-ttu-id="76a98-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76a98-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="76a98-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76a98-125">Request body</span></span>
<span data-ttu-id="76a98-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="76a98-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76a98-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="76a98-127">Response</span></span>
<span data-ttu-id="76a98-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76a98-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76a98-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76a98-130">Example</span></span>
<span data-ttu-id="76a98-131">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="76a98-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="76a98-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76a98-132">Request</span></span>
<span data-ttu-id="76a98-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="76a98-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="76a98-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="76a98-134">Response</span></span>
<span data-ttu-id="76a98-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="76a98-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="76a98-136">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="76a98-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="76a98-137">C#</span><span class="sxs-lookup"><span data-stu-id="76a98-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/educationsubmission_return-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="76a98-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="76a98-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/educationsubmission_return-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="76a98-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="76a98-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/educationsubmission_return-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-return.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationsubmission-return.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsubmission-return.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
