---
title: 'educationSubmission: retornar'
description: Esta ação faz com que a classificação e os comentários associados a esse envio estejam disponíveis para o aluno.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f785fab77f6da9c8d9c8dff1f20eb568191ca3db
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416083"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="a8551-103">educationSubmission: retornar</span><span class="sxs-lookup"><span data-stu-id="a8551-103">educationSubmission: return</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8551-104">Esta ação faz com que a classificação e os comentários associados a esse envio estejam disponíveis para o aluno.</span><span class="sxs-lookup"><span data-stu-id="a8551-104">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="a8551-105">Isso alterará o status do envio de "enviado" para "retornado" e indica que o feedback é fornecido ou a gradação é feita.</span><span class="sxs-lookup"><span data-stu-id="a8551-105">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="a8551-106">Esta ação só pode ser feita pelo professor.</span><span class="sxs-lookup"><span data-stu-id="a8551-106">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8551-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8551-107">Permissions</span></span>
<span data-ttu-id="a8551-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8551-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8551-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8551-110">Permission type</span></span>      | <span data-ttu-id="a8551-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8551-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8551-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8551-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="a8551-113">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8551-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="a8551-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8551-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a8551-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8551-115">Not supported.</span></span>  |
|<span data-ttu-id="a8551-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8551-116">Application</span></span> | <span data-ttu-id="a8551-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8551-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a8551-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8551-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="a8551-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8551-119">Request headers</span></span>
| <span data-ttu-id="a8551-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8551-120">Header</span></span>       | <span data-ttu-id="a8551-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a8551-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a8551-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8551-122">Authorization</span></span>  | <span data-ttu-id="a8551-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8551-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a8551-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8551-125">Request body</span></span>
<span data-ttu-id="a8551-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8551-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8551-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8551-127">Response</span></span>
<span data-ttu-id="a8551-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8551-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8551-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8551-130">Example</span></span>
<span data-ttu-id="a8551-131">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a8551-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a8551-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8551-132">Request</span></span>
<span data-ttu-id="a8551-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8551-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a8551-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8551-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a8551-135">C#</span><span class="sxs-lookup"><span data-stu-id="a8551-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-return-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8551-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8551-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-return-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a8551-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a8551-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-return-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a8551-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8551-138">Response</span></span>
<span data-ttu-id="a8551-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a8551-139">The following is an example of the response.</span></span>

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
