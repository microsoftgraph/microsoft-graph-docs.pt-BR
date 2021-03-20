---
title: Excluir educationCategory
description: Exclua uma categoria existente.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4bf5777ee48f4701a3a0ae29f1da9b9f9ab26269
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951694"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="c6b2e-103">Excluir educationCategory</span><span class="sxs-lookup"><span data-stu-id="c6b2e-103">Delete educationCategory</span></span>

<span data-ttu-id="c6b2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6b2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6b2e-105">Exclua uma categoria existente.</span><span class="sxs-lookup"><span data-stu-id="c6b2e-105">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6b2e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6b2e-106">Permissions</span></span>

<span data-ttu-id="c6b2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6b2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c6b2e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6b2e-109">Permission type</span></span>                        | <span data-ttu-id="c6b2e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6b2e-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="c6b2e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6b2e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c6b2e-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6b2e-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="c6b2e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6b2e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6b2e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6b2e-114">Not Supported.</span></span>                                          |
| <span data-ttu-id="c6b2e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6b2e-115">Application</span></span>                            | <span data-ttu-id="c6b2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6b2e-116">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="c6b2e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6b2e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c6b2e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6b2e-118">Request headers</span></span>

| <span data-ttu-id="c6b2e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6b2e-119">Header</span></span>        | <span data-ttu-id="c6b2e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c6b2e-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="c6b2e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6b2e-121">Authorization</span></span> | <span data-ttu-id="c6b2e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6b2e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6b2e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6b2e-124">Request body</span></span>

<span data-ttu-id="c6b2e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c6b2e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6b2e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6b2e-126">Response</span></span>

<span data-ttu-id="c6b2e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6b2e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6b2e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6b2e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6b2e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6b2e-130">Request</span></span>

<span data-ttu-id="c6b2e-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6b2e-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c6b2e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6b2e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment_2"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
# <a name="c"></a>[<span data-ttu-id="c6b2e-133">C#</span><span class="sxs-lookup"><span data-stu-id="c6b2e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6b2e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6b2e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6b2e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6b2e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6b2e-136">Java</span><span class="sxs-lookup"><span data-stu-id="c6b2e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c6b2e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6b2e-137">Response</span></span>

<span data-ttu-id="c6b2e-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c6b2e-138">The following is an example of the response.</span></span> 

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


