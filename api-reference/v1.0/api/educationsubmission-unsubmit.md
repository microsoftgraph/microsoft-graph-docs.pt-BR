---
title: 'educationSubmission: unsubmit'
description: Indica que um aluno deseja trabalhar no envio da atribuição depois que ela foi entregue.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4ddad6241c4e6c7820db143e93064b4570d68e49
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993264"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="6fd72-103">educationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="6fd72-103">educationSubmission: unsubmit</span></span>

<span data-ttu-id="6fd72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fd72-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6fd72-105">Indica que um aluno deseja trabalhar no envio da atribuição depois que ela foi entregue.</span><span class="sxs-lookup"><span data-stu-id="6fd72-105">Indicate that a student wants to work on the submission of the assignment after it was turned in.</span></span> 

<span data-ttu-id="6fd72-106">Essa ação só pode ser tomada pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="6fd72-106">This action can only be taken by the student.</span></span> <span data-ttu-id="6fd72-107">Isso alterará o status do envio de "enviado" para "working".</span><span class="sxs-lookup"><span data-stu-id="6fd72-107">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="6fd72-108">Durante o processo de envio, todos os recursos serão copiados de submittedResources para o bucket workingResources.</span><span class="sxs-lookup"><span data-stu-id="6fd72-108">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="6fd72-109">O professor estará olhando para a lista de recursos de trabalho para classificação.</span><span class="sxs-lookup"><span data-stu-id="6fd72-109">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fd72-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="6fd72-110">Permissions</span></span>
<span data-ttu-id="6fd72-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fd72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fd72-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fd72-113">Permission type</span></span>      | <span data-ttu-id="6fd72-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6fd72-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fd72-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fd72-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="6fd72-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6fd72-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="6fd72-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fd72-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6fd72-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fd72-118">Not supported.</span></span>  |
|<span data-ttu-id="6fd72-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fd72-119">Application</span></span> | <span data-ttu-id="6fd72-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fd72-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6fd72-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fd72-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="6fd72-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fd72-122">Request headers</span></span>
| <span data-ttu-id="6fd72-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6fd72-123">Header</span></span>       | <span data-ttu-id="6fd72-124">Valor</span><span class="sxs-lookup"><span data-stu-id="6fd72-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6fd72-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fd72-125">Authorization</span></span>  | <span data-ttu-id="6fd72-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fd72-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6fd72-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fd72-128">Request body</span></span>
<span data-ttu-id="6fd72-129">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="6fd72-129">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fd72-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fd72-130">Response</span></span>
<span data-ttu-id="6fd72-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fd72-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fd72-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fd72-133">Example</span></span>
<span data-ttu-id="6fd72-134">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="6fd72-134">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="6fd72-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fd72-135">Request</span></span>
<span data-ttu-id="6fd72-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fd72-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6fd72-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fd72-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/unsubmit
```
# <a name="c"></a>[<span data-ttu-id="6fd72-138">C#</span><span class="sxs-lookup"><span data-stu-id="6fd72-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-unsubmit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fd72-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fd72-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-unsubmit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fd72-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fd72-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-unsubmit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6fd72-141">Java</span><span class="sxs-lookup"><span data-stu-id="6fd72-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-unsubmit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6fd72-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fd72-142">Response</span></span>
<span data-ttu-id="6fd72-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6fd72-143">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: unsubmit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


