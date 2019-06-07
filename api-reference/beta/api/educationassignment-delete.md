---
title: Excluir educationAssignment
description: Excluir uma atribuição existente. Somente os professores de uma aula podem excluir atribuições.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 10a66116b9fb3443cce72641fd8ffb7f63d6fee0
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750035"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="6f466-104">Excluir educationAssignment</span><span class="sxs-lookup"><span data-stu-id="6f466-104">Delete educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f466-105">Excluir uma atribuição existente.</span><span class="sxs-lookup"><span data-stu-id="6f466-105">Delete an existing assignment.</span></span> <span data-ttu-id="6f466-106">Somente os professores de uma aula podem excluir atribuições.</span><span class="sxs-lookup"><span data-stu-id="6f466-106">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f466-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f466-107">Permissions</span></span>

<span data-ttu-id="6f466-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f466-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6f466-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f466-110">Permission type</span></span>                        | <span data-ttu-id="6f466-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f466-111">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="6f466-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f466-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f466-113">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f466-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="6f466-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f466-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f466-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f466-115">Not Supported.</span></span>                                          |
| <span data-ttu-id="6f466-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f466-116">Application</span></span>                            | <span data-ttu-id="6f466-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f466-117">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="6f466-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f466-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6f466-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f466-119">Request headers</span></span>

| <span data-ttu-id="6f466-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f466-120">Header</span></span>        | <span data-ttu-id="6f466-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6f466-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="6f466-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f466-122">Authorization</span></span> | <span data-ttu-id="6f466-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f466-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f466-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f466-125">Request body</span></span>

<span data-ttu-id="6f466-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6f466-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f466-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f466-127">Response</span></span>

<span data-ttu-id="6f466-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f466-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f466-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f466-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f466-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f466-131">Request</span></span>

<span data-ttu-id="6f466-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f466-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
### <a name="response"></a><span data-ttu-id="6f466-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f466-133">Response</span></span>
<span data-ttu-id="6f466-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6f466-134">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

#### <a name="sdk-sample-code"></a><span data-ttu-id="6f466-135">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="6f466-135">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="6f466-136">C#</span><span class="sxs-lookup"><span data-stu-id="6f466-136">C#</span></span>](#tab/cs)

[!INCLUDE [sample-code](../includes/delete_educationassignment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6f466-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="6f466-137">Javascript</span></span>](#tab/javascript)

[!INCLUDE [sample-code](../includes/delete_educationassignment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
