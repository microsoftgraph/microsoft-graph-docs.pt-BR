---
title: Excluir educationCategory
description: Excluir uma categoria existente.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a1a74d0755dae8c83a62a7acf92cd34ef0245d1a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002489"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="4ad52-103">Excluir educationCategory</span><span class="sxs-lookup"><span data-stu-id="4ad52-103">Delete educationCategory</span></span>

<span data-ttu-id="4ad52-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ad52-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ad52-105">Excluir uma categoria existente.</span><span class="sxs-lookup"><span data-stu-id="4ad52-105">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ad52-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ad52-106">Permissions</span></span>

<span data-ttu-id="4ad52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ad52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4ad52-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ad52-109">Permission type</span></span>                        | <span data-ttu-id="4ad52-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ad52-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="4ad52-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ad52-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ad52-112">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ad52-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="4ad52-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ad52-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ad52-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ad52-114">Not Supported.</span></span>                                          |
| <span data-ttu-id="4ad52-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ad52-115">Application</span></span>                            | <span data-ttu-id="4ad52-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ad52-116">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="4ad52-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ad52-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4ad52-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ad52-118">Request headers</span></span>

| <span data-ttu-id="4ad52-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ad52-119">Header</span></span>        | <span data-ttu-id="4ad52-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4ad52-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="4ad52-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ad52-121">Authorization</span></span> | <span data-ttu-id="4ad52-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ad52-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ad52-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ad52-124">Request body</span></span>

<span data-ttu-id="4ad52-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ad52-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ad52-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ad52-126">Response</span></span>

<span data-ttu-id="4ad52-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ad52-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ad52-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ad52-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ad52-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ad52-130">Request</span></span>

<span data-ttu-id="4ad52-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ad52-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4ad52-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ad52-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
# <a name="c"></a>[<span data-ttu-id="4ad52-133">C#</span><span class="sxs-lookup"><span data-stu-id="4ad52-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ad52-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ad52-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ad52-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ad52-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4ad52-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ad52-136">Response</span></span>

<span data-ttu-id="4ad52-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4ad52-137">The following is an example of the response.</span></span> 

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


