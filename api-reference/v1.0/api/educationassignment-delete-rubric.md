---
title: Excluir educationRubric de educationAssignment
description: Excluir um educationRubric de um educationAssignment
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b35e71df638a6285eff614f89a2a728c115011a1
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991110"
---
# <a name="delete-educationrubric-from-educationassignment"></a><span data-ttu-id="a0b6d-103">Excluir educationRubric de educationAssignment</span><span class="sxs-lookup"><span data-stu-id="a0b6d-103">Delete educationRubric from educationAssignment</span></span>

<span data-ttu-id="a0b6d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0b6d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a0b6d-105">Remover um [educationRubric](../resources/educationrubric.md) de [um educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a0b6d-105">Remove an [educationRubric](../resources/educationrubric.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>
<span data-ttu-id="a0b6d-106">Este método não exclui a rubrica em si.</span><span class="sxs-lookup"><span data-stu-id="a0b6d-106">This method does not delete the rubric itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0b6d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0b6d-107">Permissions</span></span>

<span data-ttu-id="a0b6d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0b6d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0b6d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0b6d-110">Permission type</span></span>                        | <span data-ttu-id="a0b6d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0b6d-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a0b6d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0b6d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0b6d-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0b6d-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="a0b6d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0b6d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0b6d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0b6d-115">Not supported.</span></span> |
| <span data-ttu-id="a0b6d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0b6d-116">Application</span></span>                            | <span data-ttu-id="a0b6d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0b6d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0b6d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0b6d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a0b6d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0b6d-119">Request headers</span></span>

| <span data-ttu-id="a0b6d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a0b6d-120">Name</span></span>          | <span data-ttu-id="a0b6d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0b6d-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a0b6d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0b6d-122">Authorization</span></span> | <span data-ttu-id="a0b6d-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="a0b6d-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0b6d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0b6d-124">Request body</span></span>

<span data-ttu-id="a0b6d-125">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="a0b6d-125">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0b6d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0b6d-126">Response</span></span>

<span data-ttu-id="a0b6d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0b6d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0b6d-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a0b6d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a0b6d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0b6d-130">Request</span></span>

<span data-ttu-id="a0b6d-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0b6d-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a0b6d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0b6d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric_from_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/rubric/$ref
```
# <a name="c"></a>[<span data-ttu-id="a0b6d-133">C#</span><span class="sxs-lookup"><span data-stu-id="a0b6d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0b6d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0b6d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0b6d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0b6d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0b6d-136">Java</span><span class="sxs-lookup"><span data-stu-id="a0b6d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationrubric-from-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a0b6d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0b6d-137">Response</span></span>

<span data-ttu-id="a0b6d-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a0b6d-138">The following is an example of the response.</span></span>

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


