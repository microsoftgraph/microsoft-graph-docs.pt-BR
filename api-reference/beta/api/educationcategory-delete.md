---
title: Excluir educationCategory
description: Excluir uma categoria existente.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2ae8d378760989b13e9597e86be01a2c5a6140cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427071"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="68b28-103">Excluir educationCategory</span><span class="sxs-lookup"><span data-stu-id="68b28-103">Delete educationCategory</span></span>

<span data-ttu-id="68b28-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="68b28-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68b28-105">Excluir uma categoria existente.</span><span class="sxs-lookup"><span data-stu-id="68b28-105">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="68b28-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="68b28-106">Permissions</span></span>

<span data-ttu-id="68b28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68b28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68b28-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68b28-109">Permission type</span></span>                        | <span data-ttu-id="68b28-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68b28-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="68b28-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68b28-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="68b28-112">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68b28-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="68b28-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68b28-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68b28-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68b28-114">Not Supported.</span></span>                                          |
| <span data-ttu-id="68b28-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68b28-115">Application</span></span>                            | <span data-ttu-id="68b28-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68b28-116">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="68b28-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68b28-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="68b28-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68b28-118">Request headers</span></span>

| <span data-ttu-id="68b28-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="68b28-119">Header</span></span>        | <span data-ttu-id="68b28-120">Valor</span><span class="sxs-lookup"><span data-stu-id="68b28-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="68b28-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="68b28-121">Authorization</span></span> | <span data-ttu-id="68b28-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68b28-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68b28-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68b28-124">Request body</span></span>

<span data-ttu-id="68b28-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="68b28-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68b28-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="68b28-126">Response</span></span>

<span data-ttu-id="68b28-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68b28-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68b28-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68b28-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="68b28-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68b28-130">Request</span></span>

<span data-ttu-id="68b28-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="68b28-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="68b28-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="68b28-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
# <a name="c"></a>[<span data-ttu-id="68b28-133">C#</span><span class="sxs-lookup"><span data-stu-id="68b28-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68b28-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68b28-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68b28-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68b28-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="68b28-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="68b28-136">Response</span></span>

<span data-ttu-id="68b28-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="68b28-137">The following is an example of the response.</span></span> 

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
