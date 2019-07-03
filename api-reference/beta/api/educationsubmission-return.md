---
title: 'educationSubmission: retornar'
description: Esta ação faz com que a classificação e os comentários associados a esse envio estejam disponíveis para o aluno.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 203fcc9efa06b9f34e5c1d9fbb0bc806cc1e6e10
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441398"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="c501b-103">educationSubmission: retornar</span><span class="sxs-lookup"><span data-stu-id="c501b-103">educationSubmission: return</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c501b-104">Esta ação faz com que a classificação e os comentários associados a esse envio estejam disponíveis para o aluno.</span><span class="sxs-lookup"><span data-stu-id="c501b-104">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="c501b-105">Isso alterará o status do envio de "enviado" para "retornado" e indica que o feedback é fornecido ou a gradação é feita.</span><span class="sxs-lookup"><span data-stu-id="c501b-105">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="c501b-106">Esta ação só pode ser feita pelo professor.</span><span class="sxs-lookup"><span data-stu-id="c501b-106">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="c501b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c501b-107">Permissions</span></span>
<span data-ttu-id="c501b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c501b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c501b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c501b-110">Permission type</span></span>      | <span data-ttu-id="c501b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c501b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c501b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c501b-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="c501b-113">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c501b-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="c501b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c501b-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c501b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c501b-115">Not supported.</span></span>  |
|<span data-ttu-id="c501b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c501b-116">Application</span></span> | <span data-ttu-id="c501b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c501b-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c501b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c501b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="c501b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c501b-119">Request headers</span></span>
| <span data-ttu-id="c501b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c501b-120">Header</span></span>       | <span data-ttu-id="c501b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c501b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c501b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c501b-122">Authorization</span></span>  | <span data-ttu-id="c501b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c501b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c501b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c501b-125">Request body</span></span>
<span data-ttu-id="c501b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c501b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c501b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c501b-127">Response</span></span>
<span data-ttu-id="c501b-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c501b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c501b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c501b-130">Example</span></span>
<span data-ttu-id="c501b-131">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="c501b-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c501b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c501b-132">Request</span></span>
<span data-ttu-id="c501b-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c501b-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c501b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c501b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c501b-135">C#</span><span class="sxs-lookup"><span data-stu-id="c501b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-return-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c501b-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="c501b-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-return-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c501b-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c501b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-return-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c501b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c501b-138">Response</span></span>
<span data-ttu-id="c501b-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c501b-139">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
