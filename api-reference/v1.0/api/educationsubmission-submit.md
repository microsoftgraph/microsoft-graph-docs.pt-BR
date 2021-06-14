---
title: 'educationSubmission: submit'
description: Uma ação que indica que um aluno é feito com o trabalho e está pronto para entregar a atribuição. Essa ação só pode ser tomada pelo aluno.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1c455b022fef11b82935471a3eb90fd2b253bbd7
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912216"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="6dfc1-104">educationSubmission: submit</span><span class="sxs-lookup"><span data-stu-id="6dfc1-104">educationSubmission: submit</span></span>

<span data-ttu-id="6dfc1-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dfc1-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6dfc1-106">Indica que um aluno terminou com o trabalho e está pronto para entregar a atribuição.</span><span class="sxs-lookup"><span data-stu-id="6dfc1-106">Indicate that a student is done with the work and is ready to hand in the assignment.</span></span> 

<span data-ttu-id="6dfc1-107">Essa ação só pode ser tomada pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="6dfc1-107">This action can only be taken by the student.</span></span> <span data-ttu-id="6dfc1-108">Isso alterará o status do envio de "working" para "submitted".</span><span class="sxs-lookup"><span data-stu-id="6dfc1-108">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="6dfc1-109">Durante o processo de envio, todos os recursos serão copiados para o **bucket submittedResources.**</span><span class="sxs-lookup"><span data-stu-id="6dfc1-109">During the submit process, all the resources will be copied to the **submittedResources** bucket.</span></span> <span data-ttu-id="6dfc1-110">O professor estará olhando para a lista de recursos enviados para classificação.</span><span class="sxs-lookup"><span data-stu-id="6dfc1-110">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dfc1-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="6dfc1-111">Permissions</span></span>
<span data-ttu-id="6dfc1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dfc1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dfc1-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6dfc1-114">Permission type</span></span>      | <span data-ttu-id="6dfc1-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6dfc1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dfc1-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6dfc1-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="6dfc1-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6dfc1-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="6dfc1-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6dfc1-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6dfc1-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6dfc1-119">Not supported.</span></span>  |
|<span data-ttu-id="6dfc1-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6dfc1-120">Application</span></span> | <span data-ttu-id="6dfc1-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6dfc1-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6dfc1-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6dfc1-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/submit
```

## <a name="request-headers"></a><span data-ttu-id="6dfc1-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6dfc1-123">Request headers</span></span>
| <span data-ttu-id="6dfc1-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6dfc1-124">Header</span></span>       | <span data-ttu-id="6dfc1-125">Valor</span><span class="sxs-lookup"><span data-stu-id="6dfc1-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6dfc1-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="6dfc1-126">Authorization</span></span>  | <span data-ttu-id="6dfc1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6dfc1-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6dfc1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6dfc1-129">Request body</span></span>
<span data-ttu-id="6dfc1-130">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="6dfc1-130">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dfc1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dfc1-131">Response</span></span>
<span data-ttu-id="6dfc1-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6dfc1-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dfc1-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6dfc1-134">Example</span></span>
<span data-ttu-id="6dfc1-135">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="6dfc1-135">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6dfc1-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6dfc1-136">Request</span></span>
<span data-ttu-id="6dfc1-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6dfc1-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/submit
```

### <a name="response"></a><span data-ttu-id="6dfc1-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dfc1-138">Response</span></span>
<span data-ttu-id="6dfc1-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6dfc1-139">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


