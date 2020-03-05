---
title: 'educationSubmission: retornar'
description: Esta ação faz com que a classificação e os comentários associados a esse envio estejam disponíveis para o aluno.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d04c954f239ba1999f2ca838d14e52b7920f4bc0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424824"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="6094a-103">educationSubmission: retornar</span><span class="sxs-lookup"><span data-stu-id="6094a-103">educationSubmission: return</span></span>

<span data-ttu-id="6094a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6094a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6094a-105">Esta ação faz com que a classificação e os comentários associados a esse envio estejam disponíveis para o aluno.</span><span class="sxs-lookup"><span data-stu-id="6094a-105">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="6094a-106">Isso alterará o status do envio de "enviado" para "retornado" e indica que o feedback é fornecido ou a gradação é feita.</span><span class="sxs-lookup"><span data-stu-id="6094a-106">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="6094a-107">Esta ação só pode ser feita pelo professor.</span><span class="sxs-lookup"><span data-stu-id="6094a-107">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="6094a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6094a-108">Permissions</span></span>
<span data-ttu-id="6094a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6094a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6094a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6094a-111">Permission type</span></span>      | <span data-ttu-id="6094a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6094a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6094a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6094a-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="6094a-114">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6094a-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="6094a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6094a-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6094a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6094a-116">Not supported.</span></span>  |
|<span data-ttu-id="6094a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6094a-117">Application</span></span> | <span data-ttu-id="6094a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6094a-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6094a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6094a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="6094a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6094a-120">Request headers</span></span>
| <span data-ttu-id="6094a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6094a-121">Header</span></span>       | <span data-ttu-id="6094a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6094a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6094a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6094a-123">Authorization</span></span>  | <span data-ttu-id="6094a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6094a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6094a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6094a-126">Request body</span></span>
<span data-ttu-id="6094a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6094a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6094a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6094a-128">Response</span></span>
<span data-ttu-id="6094a-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6094a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6094a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6094a-131">Example</span></span>
<span data-ttu-id="6094a-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="6094a-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6094a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6094a-133">Request</span></span>
<span data-ttu-id="6094a-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6094a-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6094a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6094a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```
# <a name="c"></a>[<span data-ttu-id="6094a-136">C#</span><span class="sxs-lookup"><span data-stu-id="6094a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-return-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6094a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6094a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-return-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6094a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6094a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-return-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6094a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6094a-139">Response</span></span>
<span data-ttu-id="6094a-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6094a-140">The following is an example of the response.</span></span>

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
