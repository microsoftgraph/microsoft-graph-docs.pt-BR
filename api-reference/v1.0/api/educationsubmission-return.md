---
title: 'educationSubmission: return'
description: Disponibilizar a nota e os comentários associados a esse envio para o aluno.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8ef40b6ffe95a6e815ede6c44d4d0639be1c2524
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993366"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="0cd7b-103">educationSubmission: return</span><span class="sxs-lookup"><span data-stu-id="0cd7b-103">educationSubmission: return</span></span>

<span data-ttu-id="0cd7b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cd7b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0cd7b-105">Disponibilizar a nota e os comentários associados a esse envio para o aluno.</span><span class="sxs-lookup"><span data-stu-id="0cd7b-105">Make the grade and feedback associated with this submission available to the student.</span></span> 

<span data-ttu-id="0cd7b-106">Essa ação altera o status do envio de "enviado" para "retornado" e indica que os comentários são fornecidos ou a classificação é feita.</span><span class="sxs-lookup"><span data-stu-id="0cd7b-106">This action changes the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="0cd7b-107">Essa ação só pode ser feita pelo professor.</span><span class="sxs-lookup"><span data-stu-id="0cd7b-107">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cd7b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0cd7b-108">Permissions</span></span>
<span data-ttu-id="0cd7b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cd7b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cd7b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cd7b-111">Permission type</span></span>      | <span data-ttu-id="0cd7b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0cd7b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cd7b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cd7b-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="0cd7b-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0cd7b-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="0cd7b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cd7b-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0cd7b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cd7b-116">Not supported.</span></span>  |
|<span data-ttu-id="0cd7b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cd7b-117">Application</span></span> | <span data-ttu-id="0cd7b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cd7b-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0cd7b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cd7b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/return
```
## <a name="request-headers"></a><span data-ttu-id="0cd7b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cd7b-120">Request headers</span></span>
| <span data-ttu-id="0cd7b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0cd7b-121">Header</span></span>       | <span data-ttu-id="0cd7b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0cd7b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0cd7b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cd7b-123">Authorization</span></span>  | <span data-ttu-id="0cd7b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0cd7b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0cd7b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cd7b-126">Request body</span></span>
<span data-ttu-id="0cd7b-127">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="0cd7b-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cd7b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cd7b-128">Response</span></span>
<span data-ttu-id="0cd7b-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cd7b-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cd7b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cd7b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cd7b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cd7b-132">Request</span></span>
<span data-ttu-id="0cd7b-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cd7b-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0cd7b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cd7b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/return
```
# <a name="c"></a>[<span data-ttu-id="0cd7b-135">C#</span><span class="sxs-lookup"><span data-stu-id="0cd7b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-return-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cd7b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cd7b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-return-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cd7b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cd7b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-return-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cd7b-138">Java</span><span class="sxs-lookup"><span data-stu-id="0cd7b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-return-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0cd7b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cd7b-139">Response</span></span>
<span data-ttu-id="0cd7b-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0cd7b-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->

```http
HTTP/1.1 204 No Content

{
}
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


