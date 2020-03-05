---
title: Remover o educationRubric do educationAssignment
description: Remover um educationRubric de um educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8fb3bb1c18a3373c17ecc8c19533c5db32a8e632
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427799"
---
# <a name="remove-educationrubric-from-educationassignment"></a><span data-ttu-id="2a40f-103">Remover o educationRubric do educationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a40f-103">Remove educationRubric from educationAssignment</span></span>

<span data-ttu-id="2a40f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2a40f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a40f-105">Remover um [educationRubric](../resources/educationrubric.md) de um [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2a40f-105">Remove an [educationRubric](../resources/educationrubric.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>  <span data-ttu-id="2a40f-106">Isso não exclui o próprio amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="2a40f-106">This does not delete the rubric itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a40f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a40f-107">Permissions</span></span>

<span data-ttu-id="2a40f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a40f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a40f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a40f-110">Permission type</span></span>                        | <span data-ttu-id="2a40f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a40f-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2a40f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a40f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a40f-113">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a40f-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="2a40f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a40f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a40f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a40f-115">Not supported.</span></span> |
| <span data-ttu-id="2a40f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a40f-116">Application</span></span>                            | <span data-ttu-id="2a40f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a40f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a40f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a40f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2a40f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a40f-119">Request headers</span></span>

| <span data-ttu-id="2a40f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2a40f-120">Name</span></span>          | <span data-ttu-id="2a40f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a40f-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2a40f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a40f-122">Authorization</span></span> | <span data-ttu-id="2a40f-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="2a40f-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a40f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a40f-124">Request body</span></span>

<span data-ttu-id="2a40f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a40f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a40f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a40f-126">Response</span></span>

<span data-ttu-id="2a40f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a40f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a40f-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2a40f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a40f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a40f-130">Request</span></span>

<span data-ttu-id="2a40f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a40f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2a40f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a40f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric_from_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric/$ref
```
# <a name="c"></a>[<span data-ttu-id="2a40f-133">C#</span><span class="sxs-lookup"><span data-stu-id="2a40f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a40f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a40f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a40f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a40f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2a40f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a40f-136">Response</span></span>

<span data-ttu-id="2a40f-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2a40f-137">The following is an example of the response.</span></span>

> <span data-ttu-id="2a40f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a40f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
