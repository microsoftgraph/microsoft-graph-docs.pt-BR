---
title: Excluir educationAssignment
description: Excluir uma atribuição existente. Somente os professores de uma aula podem excluir atribuições.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c1846f61884b35c6a8f460615aaacd441aabfd38
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416552"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="fb154-104">Excluir educationAssignment</span><span class="sxs-lookup"><span data-stu-id="fb154-104">Delete educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb154-105">Excluir uma atribuição existente.</span><span class="sxs-lookup"><span data-stu-id="fb154-105">Delete an existing assignment.</span></span> <span data-ttu-id="fb154-106">Somente os professores de uma aula podem excluir atribuições.</span><span class="sxs-lookup"><span data-stu-id="fb154-106">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb154-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb154-107">Permissions</span></span>

<span data-ttu-id="fb154-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb154-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fb154-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb154-110">Permission type</span></span>                        | <span data-ttu-id="fb154-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb154-111">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="fb154-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb154-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb154-113">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb154-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="fb154-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb154-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb154-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb154-115">Not Supported.</span></span>                                          |
| <span data-ttu-id="fb154-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb154-116">Application</span></span>                            | <span data-ttu-id="fb154-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb154-117">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="fb154-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb154-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fb154-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb154-119">Request headers</span></span>

| <span data-ttu-id="fb154-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb154-120">Header</span></span>        | <span data-ttu-id="fb154-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fb154-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="fb154-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb154-122">Authorization</span></span> | <span data-ttu-id="fb154-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb154-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb154-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb154-125">Request body</span></span>

<span data-ttu-id="fb154-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fb154-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb154-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb154-127">Response</span></span>

<span data-ttu-id="fb154-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb154-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb154-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb154-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb154-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb154-131">Request</span></span>

<span data-ttu-id="fb154-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb154-132">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fb154-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb154-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fb154-134">C#</span><span class="sxs-lookup"><span data-stu-id="fb154-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fb154-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb154-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fb154-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fb154-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="fb154-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb154-137">Response</span></span>
<span data-ttu-id="fb154-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fb154-138">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
