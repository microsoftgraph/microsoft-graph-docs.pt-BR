---
title: Remover o educationRubric do educationAssignment
description: Remover um educationRubric de um educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 119fe854c1bc04f850e89fcaf9dd8460b87ac95d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966597"
---
# <a name="remove-educationrubric-from-educationassignment"></a><span data-ttu-id="99dca-103">Remover o educationRubric do educationAssignment</span><span class="sxs-lookup"><span data-stu-id="99dca-103">Remove educationRubric from educationAssignment</span></span>

<span data-ttu-id="99dca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99dca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99dca-105">Remover um [educationRubric](../resources/educationrubric.md) de um [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="99dca-105">Remove an [educationRubric](../resources/educationrubric.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>  <span data-ttu-id="99dca-106">Isso não exclui o próprio amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="99dca-106">This does not delete the rubric itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="99dca-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="99dca-107">Permissions</span></span>

<span data-ttu-id="99dca-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99dca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="99dca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99dca-110">Permission type</span></span>                        | <span data-ttu-id="99dca-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="99dca-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="99dca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99dca-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="99dca-113">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99dca-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="99dca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99dca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99dca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99dca-115">Not supported.</span></span> |
| <span data-ttu-id="99dca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99dca-116">Application</span></span>                            | <span data-ttu-id="99dca-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99dca-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99dca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99dca-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="99dca-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99dca-119">Request headers</span></span>

| <span data-ttu-id="99dca-120">Nome</span><span class="sxs-lookup"><span data-stu-id="99dca-120">Name</span></span>          | <span data-ttu-id="99dca-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="99dca-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="99dca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="99dca-122">Authorization</span></span> | <span data-ttu-id="99dca-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="99dca-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="99dca-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99dca-124">Request body</span></span>

<span data-ttu-id="99dca-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99dca-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99dca-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="99dca-126">Response</span></span>

<span data-ttu-id="99dca-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99dca-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="99dca-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="99dca-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="99dca-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99dca-130">Request</span></span>

<span data-ttu-id="99dca-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="99dca-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99dca-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="99dca-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric_from_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric/$ref
```
# <a name="c"></a>[<span data-ttu-id="99dca-133">C#</span><span class="sxs-lookup"><span data-stu-id="99dca-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99dca-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99dca-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99dca-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99dca-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99dca-136">Java</span><span class="sxs-lookup"><span data-stu-id="99dca-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationrubric-from-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="99dca-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="99dca-137">Response</span></span>

<span data-ttu-id="99dca-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="99dca-138">The following is an example of the response.</span></span>

> <span data-ttu-id="99dca-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99dca-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


