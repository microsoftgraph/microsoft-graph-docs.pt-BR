---
title: Publicar uma atribuição de educação
description: Esta ação publica uma atribuição de educação.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0ef7011e283e9c9c1139516a0261b52e4cfdfff5
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993207"
---
# <a name="publish-an-education-assignment"></a><span data-ttu-id="3cfae-103">Publicar uma atribuição de educação</span><span class="sxs-lookup"><span data-stu-id="3cfae-103">Publish an education assignment</span></span>

<span data-ttu-id="3cfae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cfae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3cfae-105">Esta ação publica uma atribuição de educação.</span><span class="sxs-lookup"><span data-stu-id="3cfae-105">This action publishes an education assignment.</span></span>

 <span data-ttu-id="3cfae-106">Somente um professor da classe pode fazer essa chamada.</span><span class="sxs-lookup"><span data-stu-id="3cfae-106">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="3cfae-107">Quando uma atribuição estiver no status de rascunho, os alunos não verão a atribuição, nem haverá objetos de envio.</span><span class="sxs-lookup"><span data-stu-id="3cfae-107">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="3cfae-108">Chamar essa API [cria objetos educationSubmission](../resources/educationsubmission.md) e exibe a atribuição na lista de cada aluno.</span><span class="sxs-lookup"><span data-stu-id="3cfae-108">Calling this API creates [educationSubmission](../resources/educationsubmission.md) objects and displays the assignment in each student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cfae-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cfae-109">Permissions</span></span>
<span data-ttu-id="3cfae-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cfae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cfae-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cfae-112">Permission type</span></span>      | <span data-ttu-id="3cfae-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cfae-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cfae-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cfae-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="3cfae-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cfae-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="3cfae-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cfae-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3cfae-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cfae-117">Not supported.</span></span>  |
|<span data-ttu-id="3cfae-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cfae-118">Application</span></span> | <span data-ttu-id="3cfae-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cfae-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3cfae-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cfae-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="3cfae-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cfae-121">Request headers</span></span>
| <span data-ttu-id="3cfae-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3cfae-122">Header</span></span>       | <span data-ttu-id="3cfae-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3cfae-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3cfae-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cfae-124">Authorization</span></span>  | <span data-ttu-id="3cfae-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cfae-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3cfae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cfae-127">Request body</span></span>
<span data-ttu-id="3cfae-128">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="3cfae-128">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cfae-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cfae-129">Response</span></span>
<span data-ttu-id="3cfae-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cfae-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cfae-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cfae-132">Example</span></span>
<span data-ttu-id="3cfae-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="3cfae-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="3cfae-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cfae-134">Request</span></span>
<span data-ttu-id="3cfae-135">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cfae-135">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3cfae-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cfae-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "educationassignment_publish_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/publish
```
# <a name="c"></a>[<span data-ttu-id="3cfae-137">C#</span><span class="sxs-lookup"><span data-stu-id="3cfae-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cfae-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cfae-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cfae-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cfae-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cfae-140">Java</span><span class="sxs-lookup"><span data-stu-id="3cfae-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3cfae-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cfae-141">Response</span></span>
<span data-ttu-id="3cfae-142">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="3cfae-142">The following is an example of a response.</span></span> 

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
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


