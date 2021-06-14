---
title: Excluir educationSubmissionResource
description: Exclui um recurso do envio. Isso só pode ser feito pelo aluno. Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada após a exclusão da cópia atual.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 45b165ab8f2a9c07d657ea56b3118f5e14ba5e4b
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912127"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="69fc7-105">Excluir educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="69fc7-105">Delete educationSubmissionResource</span></span>

<span data-ttu-id="69fc7-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69fc7-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69fc7-107">Exclui um recurso do envio.</span><span class="sxs-lookup"><span data-stu-id="69fc7-107">Deletes a resource from the submission.</span></span> <span data-ttu-id="69fc7-108">Isso só pode ser feito pelo aluno.</span><span class="sxs-lookup"><span data-stu-id="69fc7-108">This can only be done by the student.</span></span> <span data-ttu-id="69fc7-109">Se o recurso foi copiado da atribuição, uma nova cópia do recurso será criada após a exclusão da cópia atual.</span><span class="sxs-lookup"><span data-stu-id="69fc7-109">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="69fc7-110">Isso permite que você "redefina" o recurso para seu estado original.</span><span class="sxs-lookup"><span data-stu-id="69fc7-110">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="69fc7-111">Se o recurso não foi copiado da atribuição, mas foi adicionado do aluno, o recurso será simplesmente excluído.</span><span class="sxs-lookup"><span data-stu-id="69fc7-111">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="69fc7-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="69fc7-112">Permissions</span></span>
<span data-ttu-id="69fc7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69fc7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69fc7-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69fc7-115">Permission type</span></span>      | <span data-ttu-id="69fc7-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="69fc7-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69fc7-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69fc7-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="69fc7-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69fc7-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="69fc7-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69fc7-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="69fc7-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69fc7-120">Not supported.</span></span>  |
|<span data-ttu-id="69fc7-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69fc7-121">Application</span></span> | <span data-ttu-id="69fc7-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69fc7-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="69fc7-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69fc7-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/resources/8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c
```

## <a name="request-headers"></a><span data-ttu-id="69fc7-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69fc7-124">Request headers</span></span>
| <span data-ttu-id="69fc7-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="69fc7-125">Header</span></span>       | <span data-ttu-id="69fc7-126">Valor</span><span class="sxs-lookup"><span data-stu-id="69fc7-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="69fc7-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="69fc7-127">Authorization</span></span>  | <span data-ttu-id="69fc7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69fc7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="69fc7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69fc7-130">Request body</span></span>
<span data-ttu-id="69fc7-131">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="69fc7-131">Don't supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="69fc7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="69fc7-132">Response</span></span>
<span data-ttu-id="69fc7-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69fc7-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69fc7-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69fc7-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="69fc7-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69fc7-136">Request</span></span>
<span data-ttu-id="69fc7-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="69fc7-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```

### <a name="response"></a><span data-ttu-id="69fc7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="69fc7-138">Response</span></span>
<span data-ttu-id="69fc7-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="69fc7-139">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


