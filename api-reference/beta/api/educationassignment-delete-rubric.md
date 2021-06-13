---
title: Excluir educationRubric de educationAssignment
description: Remover um educationRubric de um educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 619938b8550647acfe10f648a20460fe9c7554aa
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911942"
---
# <a name="remove-educationrubric-from-educationassignment"></a><span data-ttu-id="798c7-103">Remover educationRubric do educationAssignment</span><span class="sxs-lookup"><span data-stu-id="798c7-103">Remove educationRubric from educationAssignment</span></span>

<span data-ttu-id="798c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="798c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="798c7-105">Excluir um [educationRubric](../resources/educationrubric.md) de [um educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="798c7-105">Delete an [educationRubric](../resources/educationrubric.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>
<span data-ttu-id="798c7-106">Este método não exclui a rubrica em si.</span><span class="sxs-lookup"><span data-stu-id="798c7-106">This method does not delete the rubric itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="798c7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="798c7-107">Permissions</span></span>

<span data-ttu-id="798c7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="798c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="798c7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="798c7-110">Permission type</span></span>                        | <span data-ttu-id="798c7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="798c7-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="798c7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="798c7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="798c7-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="798c7-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="798c7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="798c7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="798c7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="798c7-115">Not supported.</span></span> |
| <span data-ttu-id="798c7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="798c7-116">Application</span></span>                            | <span data-ttu-id="798c7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="798c7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="798c7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="798c7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="798c7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="798c7-119">Request headers</span></span>

| <span data-ttu-id="798c7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="798c7-120">Name</span></span>          | <span data-ttu-id="798c7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="798c7-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="798c7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="798c7-122">Authorization</span></span> | <span data-ttu-id="798c7-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="798c7-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="798c7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="798c7-124">Request body</span></span>

<span data-ttu-id="798c7-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="798c7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="798c7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="798c7-126">Response</span></span>

<span data-ttu-id="798c7-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="798c7-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="798c7-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="798c7-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="798c7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="798c7-130">Request</span></span>

<span data-ttu-id="798c7-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="798c7-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="798c7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="798c7-132">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "delete_educationrubric_from_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/rubric/$ref
```
# <a name="c"></a>[<span data-ttu-id="798c7-133">C#</span><span class="sxs-lookup"><span data-stu-id="798c7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="798c7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="798c7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="798c7-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="798c7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="798c7-136">Java</span><span class="sxs-lookup"><span data-stu-id="798c7-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationrubric-from-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="798c7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="798c7-137">Response</span></span>

<span data-ttu-id="798c7-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="798c7-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


