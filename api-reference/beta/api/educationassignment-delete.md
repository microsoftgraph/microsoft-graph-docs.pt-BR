---
title: Excluir educationAssignment
description: Excluir uma atribuição existente. Somente os professores de uma aula podem excluir atribuições.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 39d26a7fdc20ec7a28e89d1186733821f5189850
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436176"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="3c6f0-104">Excluir educationAssignment</span><span class="sxs-lookup"><span data-stu-id="3c6f0-104">Delete educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c6f0-105">Excluir uma atribuição existente.</span><span class="sxs-lookup"><span data-stu-id="3c6f0-105">Delete an existing assignment.</span></span> <span data-ttu-id="3c6f0-106">Somente os professores de uma aula podem excluir atribuições.</span><span class="sxs-lookup"><span data-stu-id="3c6f0-106">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c6f0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c6f0-107">Permissions</span></span>

<span data-ttu-id="3c6f0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c6f0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3c6f0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c6f0-110">Permission type</span></span>                        | <span data-ttu-id="3c6f0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c6f0-111">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="3c6f0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c6f0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c6f0-113">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c6f0-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="3c6f0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c6f0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c6f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c6f0-115">Not Supported.</span></span>                                          |
| <span data-ttu-id="3c6f0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c6f0-116">Application</span></span>                            | <span data-ttu-id="3c6f0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c6f0-117">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="3c6f0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c6f0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3c6f0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c6f0-119">Request headers</span></span>

| <span data-ttu-id="3c6f0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c6f0-120">Header</span></span>        | <span data-ttu-id="3c6f0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3c6f0-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="3c6f0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c6f0-122">Authorization</span></span> | <span data-ttu-id="3c6f0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c6f0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c6f0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c6f0-125">Request body</span></span>

<span data-ttu-id="3c6f0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c6f0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c6f0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c6f0-127">Response</span></span>

<span data-ttu-id="3c6f0-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c6f0-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c6f0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c6f0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c6f0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c6f0-131">Request</span></span>

<span data-ttu-id="3c6f0-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c6f0-132">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3c6f0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c6f0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c6f0-134">C#</span><span class="sxs-lookup"><span data-stu-id="3c6f0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c6f0-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c6f0-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c6f0-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3c6f0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="3c6f0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c6f0-137">Response</span></span>
<span data-ttu-id="3c6f0-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c6f0-138">The following is an example of the response.</span></span> 


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
