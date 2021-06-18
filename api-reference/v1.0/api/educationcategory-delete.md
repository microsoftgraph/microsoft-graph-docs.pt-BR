---
title: Excluir educationCategory
description: Exclua uma categoria existente.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ba6a68358f91e2f965bb5fe8a39145ee20295d93
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992860"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="9081d-103">Excluir educationCategory</span><span class="sxs-lookup"><span data-stu-id="9081d-103">Delete educationCategory</span></span>

<span data-ttu-id="9081d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9081d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9081d-105">Excluir uma categoria [existente](../resources/educationcategory.md).</span><span class="sxs-lookup"><span data-stu-id="9081d-105">Delete an existing [category](../resources/educationcategory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9081d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9081d-106">Permissions</span></span>

<span data-ttu-id="9081d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9081d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9081d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9081d-109">Permission type</span></span>                        | <span data-ttu-id="9081d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9081d-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="9081d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9081d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9081d-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9081d-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="9081d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9081d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9081d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9081d-114">Not Supported.</span></span>                                          |
| <span data-ttu-id="9081d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9081d-115">Application</span></span>                            | <span data-ttu-id="9081d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9081d-116">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="9081d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9081d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9081d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9081d-118">Request headers</span></span>

| <span data-ttu-id="9081d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9081d-119">Header</span></span>        | <span data-ttu-id="9081d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9081d-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="9081d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9081d-121">Authorization</span></span> | <span data-ttu-id="9081d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9081d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9081d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9081d-124">Request body</span></span>

<span data-ttu-id="9081d-125">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="9081d-125">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9081d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9081d-126">Response</span></span>

<span data-ttu-id="9081d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9081d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9081d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9081d-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9081d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9081d-130">Request</span></span>

<span data-ttu-id="9081d-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9081d-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9081d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9081d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment_2"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/classes/c42f493f-42b4-4e7d-8148-af894cbc518b/assignmentCategories/b93d3b6b-360c-45c0-8764-e8bb622a9504
```
# <a name="c"></a>[<span data-ttu-id="9081d-133">C#</span><span class="sxs-lookup"><span data-stu-id="9081d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9081d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9081d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9081d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9081d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9081d-136">Java</span><span class="sxs-lookup"><span data-stu-id="9081d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9081d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9081d-137">Response</span></span>

<span data-ttu-id="9081d-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9081d-138">The following is an example of the response.</span></span> 

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
  "description": "Delete educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


